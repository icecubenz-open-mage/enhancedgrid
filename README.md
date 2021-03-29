Enhanced Admin Product Grid for Magento
=======================================

This Magento extension improves the existing Magento admin product management grid. It adds some useful, customizable features to the admin product management grid including new columns and tools.

From the makers of [Sweet Tooth Rewards](http://www.sweettoothrewards.com)

Features
--------
* Full Product Search: Search for products just like a customer would and display the results in the products grid. This is extremely handy when helping a customer find a product. To clear a search filter, click on "Reset Filter".
* Grid Row Highlighter: Highlight a bunch of rows by dragging your cursor over the rows while holding CTRL. Each highlighted row will be checked off. This will apply to all grids (including the catalog grid).
* Catalog Grid Thumbnails/Images: Shows product thumbnail images in the catalog product grid in a very organized and maintainable manor.
* Persistent Catalog Grid Settings: Set the default page size, default sort, default columns to show, etc. The settings will be stored in your Store Config so you can save some time.
* Mass Product Refresh: Loads and saves a bunch of products. This was built to aid in addressing a data inconsistency issue
* Quick Export; Select the export to CSV action from the mass action drop down and it'll create a CSV with all the selected products and send it as a file to your browser.
* Custom Catalog Product Grid Columns: Lets you select which columns you want to see in the catalog product grid. For example, short description, long description, custom attributes, etc. You will also be able to change and quickly view product images thumbnails here.
* Product Image Thumbnail Column: You will be able to view product image thumbnails in a neat column in the catalog grid.
* Date Created Column: Choose to show the "date created" value for a product

Installation Instructions
-------------------------

This module should be fully plug and play. If you're using a custom back-end package/skin, which you're probably not, you should transfer over the layout tbt_enhancedgrid.xml and tbt/enhancedgrid templates folder to your own back-end package/skin. Make sure you clear your cache. Logging in and logging back out may also be required.

When the module is enabled you will see an asterisk "*" beside the Catalog -> Manage Products menu option in the back-end.

Error in config after install for Magento 1.5: If you are still seeing the error "Fatal error: Call to a member function setEntityTypeFilter()" please  go to the releases tab and click on the latest version and use that extension key.

To uninstall/disable: To turn off Enhanced Product Grid modify the app/etc/modules/TBT_Enhancedgrid.xml file and set the 'active' value to 'false'. (note: Turning off module output is not the same thing and it will does not disable the module, rather it just disables output so you're left with a blank product management screen )

Works with Magento 1.3 and up.

Notes
-----

This is an updated and ~maintained version of the original [jayelkaake/enhancedgrid](https://github.com/jayelkaake/enhancedgrid).
Changes from the original:

* Use generated thumbnail in grid: https://github.com/jayelkaake/enhancedgrid/pull/70
* Support Magento 1.9.3 store id in product URL: https://github.com/jayelkaake/enhancedgrid/pull/69
* Fix non-numeric image width: https://github.com/jayelkaake/enhancedgrid/pull/68
* Fix truncated text config: https://github.com/jayelkaake/enhancedgrid/pull/61
* Add translations: https://github.com/jayelkaake/enhancedgrid/pull/60
* Add updated_at column: https://github.com/crysix/enhancedgrid/commit/b9ffb2c0db9e23ed2e4b3d8f367d56d61b2cfb70s
* Remove notifications
* Remove advertisements on expired/outdated domains
* Use the `adminhtml_catalog_product_index` instead of `default`. To prevent JS errors and loading on unintended adminhtml pages. This has the effect of the enhanced grid only working on the catalog product index (which I think is the only place it works anyway but I could be wrong!)

All credit and copyright goes to the original author/s and contributors.
