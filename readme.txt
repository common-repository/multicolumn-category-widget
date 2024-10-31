=== Multicolumn Category Widget ===
Contributors: awelzel
Tags: widget, category
Requires at least: 3.6
Tested up to: 6.6
Stable tag: 1.0.23
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

This widget displays top level categories in multiple columns.

== Description ==

This widget displays top level categories in multiple columns.

After installation, just add the widget to desired sidebar or footer and optionally enter a custom title and the number of columns to be displayed.

By default two columns are used, but you can set any number of columns you like in the backend.

Also see details at <http://arnowelzel.de/wp/en/projects/wordpress/multicolumn-category-widget>.

== Installation ==

1. Extract the contents of the package to the `/wp-content/plugins/multicolumn-category-widget` directory
2. Activate the plugin through the 'Plugins' menu in WordPress

== Frequently Asked Questions ==

= How can I customize the style of the widget? =

All styles can be found in `css/frontend.css`. Since these styles get overwritten when updating the widget, you should add the custom styles to your theme.

= Is it possible to get more translations? =

Generally the widget supports multiple languages - you can use Loco Translate to add more languages, if needed.

If you want to provide a translation in your language which is missing yet, you're welcome to send me the po/mo files for the next update.

= The categories are not displayed in multiple columns, why? =

The layout uses multiple lists which are displayed next to each other using the CSS rule `display:inline-block`.

This means: If there not enough room to display multiple columns (either because the sidebar of the template is too narrow or the available viewport of the device is very small), the browser will eventually fall back to show only a single column. But this is intentional to make sure that the category list is always completely visible - even on smaller screens or on narrow smaller sidebars - and won't break the layout of the template by using more room as available.

In rare cases a template or a plugin changes the default behaviour of the WordPress core function `the_widget()`, which usually outputs widgets with their own CSS classes - in this case you might have to add your own styles based on the rules in `css/frontend.css` but without `.widget_multicolumncategorywidget`. However the better solution would be to check the template and/or other plugins, why the widget specific CSS classes are missing.

== Screenshots ==

1. Configuration options of the widget in the backend
2. Example for the use in the frontend

== Changelog ==

= 1.0.23=
* Updated compatibility information for WordPress 6.6

= 1.0.22=
* Updated compatibility information for WordPress 6.5

= 1.0.21=
* Updated compatibility information for WordPress 6.3

= 1.0.20=
* Updated compatibility information for WordPress 6.0

= 1.0.19=
* Code refactoring
* Updated compatibility information for WordPress 5.5

= 1.0.18 =
* Updated compatibility information for WordPress 4.6

= 1.0.17 =
* Updated compatibility information for WordPress 4.5

= 1.0.16 =
* Added translation for plugin information in the backend (plugin title, description etc.)

= 1.0.15 =
* Modified default frontend styles to avoid bullets in category titles in certain themes (for example Twenty Fifteen).

= 1.0.14 =
* Updated compatibility information for WordPress 4.3

= 1.0.13 =
* Updated compatibility information for WordPress 4.2.3

= 1.0.12 =
* Added placeholder for the category title in the backend configuration options

= 1.0.11 =
* Updated compatibility information for WordPress 4.1.1

= 1.0.10 =
* Proper use of version parameter for frontend styles (plugin version and not WordPress version)

= 1.0.9 =
* Added Russian (thanks Flector)

= 1.0.8 =
* Updated compatibility to support WordPress 4.0

= 1.0.7 =
* Fixed version information

= 1.0.6 =
* Updated translations (German, Italian, French)

= 1.0.5 =
* Updated WordPress compatibility information (3.9.1)
* Added "show post counts" option

= 1.0.4 =
* Updated WordPress compatibility information (3.9)

= 1.0.3 =
* Updated WordPress compatibility information (3.8.3)

= 1.0.2 =
* Fixed a bug in the title output: Standard title was displayed even with a custom title set.

= 1.0.1 =
* Added French and Italian.
* Added translation template (pot).

= 1.0 =
* First release.

== Upgrade Notice ==

= 1.0.17 =
This release adds no new functionality. It's just an update of the compatibility
information for WordPress 4.5.

= 1.0.8 =
This release adds no new functionality. It's just an update of the compatibility
information for WordPress 4.0.

= 1.0.1 =
This release adds new languages (French, Italian) and a translation template (pot).

= 1.0 =
First release.
