# WP-Custom-Meta-Quick-Bulk-Update

[![License](http://img.shields.io/badge/License-MIT-blue.svg)](http://opensource.org/licenses/MIT)

### Allows custom meta values for update Wordpress' quick and bulk update functions

***
### [→ Get the Code ←](https://raw.githubusercontent.com/gst4158/WP-Custom-Meta-Quick-Bulk-Update/master/quickedit.php)
***

Installation
------------
Include the file and make updates to post type names for the post columns and other custom meta updates


Detailed Explaination
-----------

How does it work? 

* Create a blank column and unset it so we can add the meta field to quick/bulk edit

* Use WP's add_action hooks for 'quick_edit_custom_box' and 'quick_edit_custom_box' to create an editable metabox. Could be expanded to include checkboxes, selects, etc.

* Use WP's add_action hook 'save_post' to update each meta value. Checks to make sure the logged in user can edit post and if the value has changed.
