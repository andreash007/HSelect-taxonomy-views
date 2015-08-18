# HSelect-taxonomy-views
The small script to convert original Taxonomy term select list with hierarchy to multi step widget.

Original post is here https://www.drupal.org/node/1758844#comment-6418926

It transforms a select list to a multiple select list with sub categories.
You need to configure Taxonomy Select to display your list like this:

Cat 1
-Subcat 11
-Subcat 12
Cat 2
-Subcat 21
-Subcat 22

This workaround use the dash separator to parse the vocabulary structure; 
I tweaked it a bit to make it work on most browsers; 
mostly the "selected" part and wrapped it up in a Drupal behavior for those ajax views.

Voila; feel free to use it by changing the jQuery selector #edit-field-categories to your liking. 
Load the javascript on your Drupal either via template (drupal_add_js(file.js) or <script/>) or via .info file.
