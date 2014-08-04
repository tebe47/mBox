mBox
====

**Please note: I've abandoned this project and moved to jQuery. There won't be any more updates.**

**If you liked mBox you will love jBox: http://stephanwagner.me/jBox**


How to use
----------

A very basic mBox could look like this:

	var myMBox = new mBox({
    	content: 'This is a very basic mBox. Click anywhere to close.'
	});
	myMBox.open();

The option attach helps you adding the open and close-events to your elements.
In following example, the element with id myMBox will open and close your mBox:

	new mBox({
		content: 'This mBox will open when clicking on an element with id="myBox".',
		attach: 'myMBox'
	});

To attach a tooltip to an element use mBox.Tooltip:
	
	new mBox.Tooltip({
		content: 'Default tooltip.',
		attach: 'myTooltip1'
	});
	
If you want your tooltips to open with mouseclick instead, set the option event back to click:

	new mBox.Tooltip({
		content: 'This tooltip opens on mouseclick.',
		attach: 'myTooltip2',
		event: 'click'
	});
	
To open a modal dialog use mBox.Modal:
	
	new mBox.Modal({
		title: 'My modal dialog',
		content: 'This is a simple modal dialog window.',
		attach: 'myModalDialog1'
	});

Use mBox.Notice to show a notice to your visitors.

	new mBox.Notice({
		content: 'This is a default notice'
	});
