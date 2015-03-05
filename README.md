# jQuery Form Conditionals 1.0.0
Copyright (c) 2015 n7 Studios

## About

jQuery Form Conditionals is a small jQuery Plugin which allows you to specify data attributes on your form field inputs to show/hide DOM elements based on the form field input's value.

## Installation

 Add jQuery and this Plugin to your web page:

`<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
<script src="jquery.form-conditionals-min.js"></script>`

Specify an ID on the DOM element you want to control:

`<div id="example">Hello, world!</div>`

Specify data attributes on your form field input:

`<input type="checkbox" name="test" data-conditional="example" />`

By default, the DOM ID matching data-conditional will display when the form field has a positive value.
If you want to hide the DOM element when the form field has a positive value, use:

`<input type="checkbox" name="test" data-conditional="example" data-condition-display="false" />`

Initialise the plugin in JS:

`<script>
jQuery(document).ready(function($) {
	$('input,select').conditional();
});
</script>`

