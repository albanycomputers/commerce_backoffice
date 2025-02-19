# Commerce Back Office
Provides the backoffice functionality present in Commerce Kickstart v2.

Contains three submodules: commerce_backoffice_product, commerce_backoffice_order, commerce_backoffice_content.


## Initial version
This a port of the Drupal version 7.x-1.6

## Compatibility notes:


## Requirements:
Commerce Backoffice Product
---------------------------
- Inline Entity Form
- Views Megarow
- Views Bulk Operations

Commerce Backoffice Order
-------------------------
- Date
- EVA
- Views Megarow
- Views Bulk Operations

Commerce Backoffice Order
-------------------------

## Installation:
Install this module using the official Backdrop CMS instructions at https://docs.backdropcms.org/documentation/extend-with-modules

## Documentation:
### Commerce Backoffice Product
Provides a better experience for stores using nodes as product displays for grouping product variations (commerce_product entities).

The node/add screen is now split into two tabs, "Create content" (ordinary node types), and "Create product" (product display node types).
The products view is now a view of nodes, showing product displays. Contains special exposed filters for filtering by product display type, and product display categories.
Uses the megarow pattern to provide a "Quick Edit" link in the view, that shows all product variations for that product display, right underneath the triggering row. The status and price can be modified directly.
Modifies the "Content types" screen by adding additional help text for understanding product displays, and adds a column to the table that indicates whether the node type is a product display node type*.
Disables the Commerce-provided "Product types" UI, and provides a custom "Product variation types" UI that contains additional help text, hides fields that are not used by the Inline Entity Form (help, description for each type), and provides the ability to create a matching node type for each created product variation type.

* - Every node type with a product reference field is considered a product display node type.

### Commerce Backoffice Order
Provides a better order management experience.

The order view has been redesigned for better usability, and contains exposed filters for the order status and creation date.
Provides rules-powered bulk operations for modifying the order statuses.
Uses the megarow pattern to provide a "Quick Edit" link in the view, that shows the line items, customer information, payments, recent messages (if Commerce Message is enabled). Allows the admin to add a new message or change the order status.


### Commerce Backoffice Content
Provides views for managing content (excluding all product display types, and their categories) and comments.

## TODO - Add documentation
Additional documentation is located in the Wiki: https://github.com/backdrop-contrib/commerce_backoffice/wiki

## Issues:
Bugs and Feature requests should be reported in the Issue Queue: https://github.com/backdrop-contrib/commerce_backoffice/issues


## Current Maintainer(s):
- [Steve Moorhouse (albanycomputers)] (https://github.com/albanycomputers)
- Seeking additional maintainers and contributors.

## Credits:

[Drupal Commerce Backoffice] (https://www.drupal.org/project/commerce_backoffice)

## Sponsorship:
- [Albany Computer Services] (https://www.albany-computers.co.uk)
- [Albany Web Design] (https://www.albanywebdesign.co.uk)
- [Albany Hosting] (https://www.albany-hosting.co.uk)

## License
This project is GPL v2 software. See the LICENSE.txt file in this directory for complete text.
