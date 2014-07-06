perchsnippets
=============
# Overview
Sublime Text 2 snippets for [Perch CMS](http://grabaperch.com) projects. Currently includes HTML templating tags and region creation / custom region array functions. I will be adding triggers for most of the major apps in the coming weeks, beginning with Blog and Forms.

## TabTriggers

Tag | TabTrigger|Details
| ------------- |-------------|---|
`<perch:after>`|perchafter|
`<perch:before>`|perchbefore|
`<perch:content>`|perchcontent|
`<perch:error>`|percherror|
`<perch:every>`|perchevery|
`<perch:form>`|perchform|Also includes `<perch:input>` and `<perch:label>` tags for faster form creation
`<perch:if>`|perchif|
`<perch:else>`|perchifelse|
`<perch:input>`|perchinput|
`<perch:noresults>`|perchnoresults|
`<perch:repeater>`|perchrepeater|
`<perch:showall>`|perchshowall|
`<perch:template>`|perchtemplate|

Function | TabTrigger|Details
| ------------- |-------------|---|
`<?php perch_content(''); ?>`|perchregion|
`<?php perch_content_custom('', array()); ?>`| perchregioncustom|

## Installation and Use

These snippets are for Sublime Text 2 and are sorted into folders, currently one for template tags and one for content functions so that you can easily pick out the ones you want. 


1. Copy the Perch Snippets folder into the `/Packages/User` folder, which can be accessed easily through `Preferences` > `Browse Packages`. 
2. Relaunch Sublime Text.
3. Enjoy.

