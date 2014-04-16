Notice
======
I'm sorry to inform you, that as of January 2014, I've abandoned the mBox and mForm projects.
I was waiting for a new version of MooTools, but it seems that the community lost interest in the further development of the framework. Currently, I'm working on jBox and jForm, which are clones from mBox and mForm written in jQuery.


mBox
----

mBox is a powerful library, helping you to easily create tooltips, modal windows, notice messages and more.

Demo: http://htmltweaks.com/mBox

Docs: http://htmltweaks.com/mBox/Documentation

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

Those examples show only the very basic usage of mBox.

Read the Documentation at http://htmltweaks.com/mBox/Documentation to see the many options and events you can set to customize your mBoxes.
