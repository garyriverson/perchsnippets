perchsnippets
=============
# Overview
Sublime Text snippets for [Perch CMS](http://grabaperch.com) projects. Currently includes HTML templating tags and region creation / custom region array functions. 

## Content

Tag | Trigger|Details
| ------------- |-------------|---|
`<perch:after>`|perchafter|
`<perch:before>`|perchbefore|
`<perch:blocks>`|perchblocks|Creates blocks group
`<perch:block>`|perchblock|Creates block
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

Tag | Trigger|Details
| ------------- |-------------|---|
`<perch:form>`|perchform|Also includes `<perch:input>` and `<perch:label>` tags for faster form creation
`---`|perchformex|Creates [example form](http://docs.grabaperch.com/docs/form/template-tags/).
`<perch:label>`|perchlabel|Label tag with attributes.
`<perch:error>`|percherror|Creates error tag with attributes.
`<perch:input>`|perchinput|Creates input element with default attributes.
`<perch:input type="text">`|perchinputtext|Creates input element of type text 
`<perch:input type="email">`|perchinputemail|Creates input element of type email
`<perch:input type="url">`|perchinputurl|Creates an input element of type url in your form. This will validate to require a protocol.
`<perch:input type="range">`|perchinputrange|Includes min, max and step attributes; creates html5 widgets.
`<perch:input type="number">`|perchinputnum|Like range, includes min, max and step attributes.
`<perch:input type="date">`|perchinputdate|Creates date input, accepts YYYY-MM-DD format. 
`<perch:input type="datetime">`|perchinputdatetime|Creates datetime input, accepts YYYY-MM-DD HH:MM format.
`<perch:input type="month">`|perchinputmonth|Creates month input, accepts YYYY-MM format.
`<perch:input type="week">`|perchinputweek|Accepts a year and week number YYYY-WNN e.g. 2011-W23 (W is literal)
`<perch:input type="color">`|perchinputcolor|Accepts a hex color;displays as html5 colorpicker in some browsers.
`<perch:input type="textarea">`|perchinputtextarea|Creates a textarea.
`<perch:input type="select">`|perchinputselect|Creates a select list; includes the options attribute.
`<perch:input type="radio">`|perchinputradio|Creates a radio input.
`<perch:input type="checkbox">`|perchinputcheck|Creates a checkbox; the value set will be checked by default.
`<perch:input type="image">`|perchinputimage|Creates an image input with all possible attributes.
`<perch:input type="file">`|perchinputfile|Creates a file input
`<perch:input type="hidden">`|perchinputhidden|Creates a hidden field.
`<perch:input type="submit">`|perchinputsubmit|Creates a submit field. Includes value attribute, which becomes the text displayed on the submit button.

##Blog
Output | Trigger | Details
|---|---|---|
`<?php perch_blog_author(perch_get('author')); ?>` |perchblogauthor |Display a blog post's author
`<?php perch_blog_authors(); ?>` |perchblogauthors| Displays list of blog authors
`<?php perch_blog_author_for_post(perch_get('s')); ?>`|perchblogpostauthor|Displays author of a post
`<?php perch_blog_categories(); ?>`|perchblogcat|Outputs a list of categories set up for the blog.
`<?php perch_blog_category(perch_get('cat')); ?>`|perchblogcattitle|Outputs the title of a category
`<?php perch_blog_date_archive_years(); ?>` |perchblogarchiveyears | Displays a list of years and the count of the number of posts in each year.
`<?php perch_blog_date_archive_months(); ?>`|perchblogarchivemonths|Displays a list of years, and then months nested within those years, along with post counts.
`<?php perch_blog_post_categories(perch_get('s')); ?>` |perchblogpostcats|Display the categories for a given blog post.
`<?php perch_blog_post_comment_form(perch_get('s')); ?>`|perchblogcommentform|Display a comment form for the given post.
`<?php perch_blog_post_comments(perch_get('s')); ?>`|perchblogcomments | Displays comments for a given post.
`<?php perch_blog_post_field(perch_get('s'), 'postTitle'); ?>`|perchblogpostfield|Output a single field (such as the title) from a blog post. 
`<?php perch_blog_post_tags(perch_get('s')); ?>`|perchblogposttags|Displays the tags for a given post.
`<?php perch_blog_post(perch_get('s')); ?>`|perchblogpost|Displays a single post.
`<?php perch_blog_recent_posts(10); ?>`|perchblogrecentposts|Get a list of the most recent blog posts.
`<?php perch_blog_section(perch_get('section')); ?>`|perchblogsection|Output the section.
`<?php perch_blog_sections(); ?>`|perchblogsections|Output a list of sections set up for the blog.
`<?php perch_blog_tag(perch_get('tag')); ?>`|perchblogtag|Output the title of a tag.
`<?php perch_blog_tags(); ?>`|perchblogtags|Display a list of tags used across all blog posts.

##Comments
Output | Trigger | Details
|---|---|---|
`<?php perch_comment(4); ?>`|perchcomment|Display a single comment
`<?php perch_comments_count('itemid123'); ?>`|perchcommentcount|Display count of comments on an item
`<?php perch_comments_form('product123', 'Elasticated garden yoga pants'); ?>`|perchcommentsform|Outputs a comment form
`<?php perch_comments('product123'); ?>`|perchcomments|Displays all comments for a given item id
`N/A`|perchcommentformtemplate|Outputs [example comment form](http://docs.grabaperch.com/addons/comments/template-tags/) template
`N/A`|perchcommentlisttemplate|Outputs [example comment listing](http://docs.grabaperch.com/addons/comments/template-tags/) template

##Mailchimp
`<?php perch_mailchimp_form('subscribe.html'); ?>`|perchchimpadd|Add a subscriber
`<?php perch_mailchimp_campaigns(); ?>`|perchchimparchive|Display a campaign archive

## Functions
Output | Trigger|Details
| ------------- |-------------|---|
`<?php include($_SERVER['DOCUMENT_ROOT'].'/perch/runtime.php');?>`|perchruntime|Creates an include for the runtime from the root of the server
`<?php perch_content(''); ?>`|perchregion|Creates new content region
`<?php perch_content_custom('', array()); ?>`|perchregioncustom|Creates new custom content region
`<?php perch_pages_navigation(); ?>`|perchnavtree|Outputs navigation tree of pages that exist (are editable) in Perch.
`<?php perch_pages_navigation(array('levels' => 1,)); ?>`|perchnavtreetop|Outputs top level of navigation tree.
`<?php perch_page_modified(array('format' => '%d %B %Y, %H:%M',));?>`|perchnavmod|Outputs the date the page was last updated; formatted using [strftime](http://php.net/strftime) codes.
`<?php perch_pages_breadcrumbs(); ?>`|perchnavcrumbs|Outputs a breadcrumb trail for the current page.
`<?php perch_pages_next_page(); ?>`|perchnavnext|Outputs details of the next page in the navigational hierarchy. 
`<?php perch_pages_previous_page(); ?>`|perchnavprev|Outputs details of the previous page.
`<?php perch_pages_parent_page(); ?>`|perchnavparent|Outputs details of the current page's parent page.

## Installation and Use

These snippets are for Sublime Text 2 or 3 and are sorted into folders, so that you can easily pick out the ones you want. 


1. Copy the Perch Snippets folder into the `/Packages/User` folder, which can be accessed easily through `Preferences` > `Browse Packages`. 
2. Relaunch Sublime Text.
3. Enjoy.

