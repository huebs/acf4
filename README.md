# Advanced Custom Fields v4.0 Beta

Welcome to the beta repository for Advanced Custom Fields v4.0.
This repository will be temporarily available for beta testing, issue reporting and bug fixing. Once the v4.0 plugin is ready, this repository will be removed and all code will be available on the WWordPress.org website as per usual.


-----------------------

### Overview

Since the recent change of WP's terms and conditions regarding hosting of plugins, the ACF plugin has undergone some BIG changes to adhere to the new rules.
The problem is that ACF includes the 'Premium' code insid ethe free hosted plugin. This is now not allowed and I have had to take out the 'Add-on' code and create seperate plugins for each of the 4 add-ons.

During this proccess, the entire plugin has been re written to use actions and filters instead of nested class structures. Hopefuly, we will see some Performance increases from both PHp and SQL becuase of this!


### Where are the Add-ons?

The addons are currently not available for download. However, over the next few days, I will create a page on the ACF website where you can enter your activation code / login to your account and download the addon files.

Each add-on is now a plugin which will pull updates from the ACF website. Each plugin has also been writen to allow for theme inclusion! Meaning, you don't need to install the plugin, you can simply include it in your functions.php file. Doing this however, will prevent any plugin updates.


### Participate Testing

If you have the time, please participate in this beta testing. The more developers we can get, the quicker this new version can be released!
Please report all issues related to this beta version here on github, not on the ACF support forum.


### New Featues
* [Optimized] Optimize performance by removing heavy class structure and implementing light weight hooks & filters!
* [Fixed] Fix issue with Preview / Draft where preview would not save custom field data - http://support.advancedcustomfields.com/discussion/4401/cannot-preview-or-schedule-content-to-be-published
* [Changed] Remove all Add-on code from the core plugin and separate into individual plugins with self hosted updates
* [Added] Add field group title validation
* [Fixed] Fix WPML issue where get_field_object / get_field find the wrong field
* [Fixed] Fix duplicate functionality - http://support.advancedcustomfields.com/discussion/4471/duplicate-fields-in-admin-doesn039t-replicate-repeater-fields 
* [Added] Add conditional statements to tab field - http://support.advancedcustomfields.com/discussion/4674/conditional-tabs
* [Improved] Improved creating / registering a custom field - Need to ad documnetation - For now, please look at the core/fields/dummy.php file and see how a field is made!
* [Added] Add new Hooks / Filter - Need to add documnetation


### Known Issues
* Any previously registered custom fields will not work. register_field is no longer a function.
* No Add-ons are included in the plugin - these will be released seperatly soon
* Export page is not available
* Add-ons page is not available


### Things to be improved
* Caching - Please feel free to offer any advice for caching in the plugin


### Thank You
A BIG THANK YOU to everyone who can help assist in this new version!