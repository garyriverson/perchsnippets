perchsnippets
=============
# Overview
Sublime Text 2 snippets for [Perch CMS](http://grabaperch.com) projects. Currently includes HTML templating tags and region creation / custom region array functions. I will be adding triggers for the major apps as I need them in my own projects (or feel like adding them).

__Update (10/13/2014):__ Added forms app snippets. Moved form-related tags into forms folder. Added `<perch:help>` and `<perch:search/>` snippets to Content snippets.

## Content

Tag | TabTrigger|Details
| ------------- |-------------|---|
`<perch:after>`|perchafter|
`<perch:before>`|perchbefore|
`<perch:content>`|perchcontent|
`<perch:else>`|perchifelse|
`<perch:every>`|perchevery|
`<perch:help>`|perchhelp|Creates a block of html help information.
`<perch:if>`|perchif|
`<perch:noresults>`|perchnoresults|
`<perch:repeater>`|perchrepeater|
`<perch:search>`|perchsearch|
`<perch:showall>`|perchshowall|
`<perch:template>`|perchtemplate|

## Forms

Tag | TabTrigger|Details
| ------------- |-------------|---|
`<perch:form>`|perchform|Also includes `<perch:input>` and `<perch:label>` tags for faster form creation
`---`|perchformex|Creates [example form](http://docs.grabaperch.com/docs/form/template-tags/).
`<perch:label>`|perchformlabel|Label tag with attributes.
`<perch:error>`|percherror|Creates error tag with attributes.
Inputs||
`<perch:input>`|perchforminput|Creates input element with default attributes.
`<perch:input type="text">`|perchforminputtext|Creates input element of type text 
`<perch:input type="email">`|perchforminputemail|Creates input element of type email
`<perch:input type="url">`|perchforminputurl|Creates an input element of type url in your form. This wil validate to require a protocol.

`<perch:input type="range">`|perchforminputrange|Includes min, max and step attributes; creates html5 widgets.
`<perch:input type="number">`|perchforminputnum|Like range, includes min, max and step attributes.
`<perch:input type="date">`|perchforminputdate|Creates date input, accepts YYYY-MM-DD format. 
`<perch:input type="datetime">`|perchforminputdatetime|Creates datetime input, accepts YYYY-MM-DD HH:MM format.
`<perch:input type="month">`|perchforminputmonth|Creates month input, accepts YYYY-MM format.
`<perch:input type="week">`|perchforminputweek|Accepts a year and week number YYYY-WNN e.g. 2011-W23 (W is literal)
`<perch:input type="color">`|perchforminputcolor|Accepts a hex color;displays as html5 colorpicker in some browsers.
`<perch:input type="textarea">`|perchforminputtextarea|Creates a textarea.
`<perch:input type="select">`|perchforminputselect|Creates a select list; includes the options attribute.
`<perch:input type="radio">`|perchforminputradio|Creates a radio input.
`<perch:input type="checkbox">`|perchforminputcheck|Creates a checkbox; the value set will be checked by default.
`<perch:input type="image">`|perchforminputimage|Creates an image input with all possible attributes.
`<perch:input type="file">`|perchforminputfile|Creates a file input
`<perch:input type="hidden">`|perchforminputhidden|Creates a hidden field.
`<perch:input type="submit">`|perchforminputsubmit|Creates a submit field. Includes value attribute, which becomes the text displayed on the submit button.

Function | TabTrigger|Details
| ------------- |-------------|---|
`<?php perch_content(''); ?>`|perchregion|
`<?php perch_content_custom('', array()); ?>`|perchregioncustom|

## Installation and Use

These snippets are for Sublime Text 2 or 3 and are sorted into folders, currently one for template tags and one for content functions so that you can easily pick out the ones you want. 


1. Copy the Perch Snippets folder into the `/Packages/User` folder, which can be accessed easily through `Preferences` > `Browse Packages`. 
2. Relaunch Sublime Text.
3. Enjoy.

