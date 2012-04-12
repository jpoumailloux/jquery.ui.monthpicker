A Month Picker for [jQuery UI](http://jqueryui.com/)
================================

Why using it?
---

You may be already using [JQuery UI Datepicker](http://jqueryui.com/demos/datepicker/) and are now looking for a Monthpicker. Unfortunately, this is not part of the functionalities of JQuery UI Datepicker.
After some Googling, you will realize two things: you are not alone having a need for a Monthpicker, and most solutions only are relying on dirty hacks on the original JQuery UI Datepicker widget.

Be relieved, you have now found dedicated working and customizable Monthpicker implementation. In the background, it is largely based on JQuery UI Datepicker, which is why it is working so great and looking so nice!
You will notice that the design is very similar to JQuery UI Datepicker, as it uses the same CSS. Hence it is fully compatible with your usual JQuery UI theme!

Demo
---

[Here!](http://jpoumailloux.com/jquery-ui-monthpicker/)

Available settings and their defaults
---

General settings:

	showOn: 'focus', // 'focus' for popup on focus,
	// 'button' for trigger button, or 'both' for either
	showAnim: 'fadeIn', // Name of jQuery animation for popup
	buttonText: '...', // Text for trigger button
	buttonImage: '', // URL for trigger button image
	changeYear: false, // True if year can be selected directly, false if only prev/next
	yearRange: 'c-10:c+10', // Range of years to display in drop-down,
	// either relative to today's year (-nn:+nn), relative to currently displayed year
	// (c-nn:c+nn), absolute (nnnn:nnnn), or a combination of the above (nnnn:-n)
	beforeShow: null, // Function that takes an input field and
	// returns a set of custom settings for the date picker
	onSelect: null, // Define a callback function when a date is selected
	onChangeYear: null, // Define a callback function when the year is changed
	onClose: null, // Define a callback function when the monthpicker is closed
	stepYears: 1, // Number of months to step back/forward
	altField: '', // Selector for an alternate field to store selected dates into
	altFormat: '', // The date format to use for the alternate field
	disabled: false // The initial disabled state

L10N:

	dateFormat: 'mm/yy',
	yearSuffix: '' // Additional text to append to the year in the month headers
	prevText: 'Prev', // Display text for previous month link
	nextText: 'Next', // Display text for next month link
	monthNames: ['January','February','March','April','May','June',
	'July','August','September','October',
	'November','December'], // Names of months for drop-down and formatting
	monthNamesShort: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul',
	'Aug', 'Sep', 'Oct', 'Nov', 'Dec'], // For formatting</pre>

Date Formatting:

	The format can be combinations of the following:
	m  - month of year (no leading zero)
	mm - month of year (two digit)
	M  - month name short
	MM - month name long
	y  - year (two digit)
	yy - year (four digit)
	@ - Unix timestamp (ms since 01/01/1970)
	! - Windows ticks (100ns since 01/01/0001)
	'...' - literal text
	'' - single quote

Alternatives
---

[Luciano Costa](https://github.com/lucianocosta/jquery.mtz.monthpicker) has developed his own implementation from scratch of a Monthpicker.
It is far better than most JQuery UI Datepicker hacks you will find on the internet but it has some severe limitations: it has very limited settings, settings are shared by all instances on the same page...

Ending text
---

Don't hesitate to contribute!

    git clone git://github.com/thebrowser/jquery.ui.monthpicker