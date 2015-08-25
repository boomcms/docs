---
currentMenu: templates
---

# Templates

Templates control the visual representation of the page and what functionality is available.

The template is changed via the 'template' section of the page settings menu.
When a page's template is changed a new [page version](/pages.html) is created and the change must be published before it is visible on the site.

Within the template developers can define editable chunks of content.
For more information about chunks and how they are defined see the [chunks page](/chunks.html).

## Themes

Templates can be grouped and packaged as part of a theme.
Themes provide a way to easily extend and customise a BoomCMS site.

## Helper functions

BoomCMS defines a number of helper functions which can be used by developers while creating templates.

Helper functions are usually defined as static methods in the [BoomCMS\Support\Helpers class](https://github.com/boomcms/boom-core/blob/master/src/BoomCMS/Support/Helpers.php).
However, these functions can use be accessed via variable callbacks defined in the views.
These variables will have the same name as the associated helper method.

For example, if you wanted to call `BoomCMS\Support\Helpers::foo()` you would simply have to use `$foo()` in your templates.

Below is a brief overview of the available Helper methods and their purpose.
For more information about a method's arguments see the [source of the Helpers class](https://github.com/boomcms/boom-core/blob/master/src/BoomCMS/Support/Helpers.php).

Method Name | Shorthand callback | Overview 
----- | ----- | -----
BoomCMS\Support\Helpers::analytics() | $analytics() | Used to insert the site's analytics tracking code only when in production
BoomCMS\Support\Helpers::assetUrl() | $assetURL() | Generates a URL to link to an asset
BoomCMS\Support\Helpers::countPages() | $countPages() | Returns a count of the number of pages which page the given parameters
BoomCMS\Support\Helpers::getPages() | $pagePages() | Returns the pages which match given parameters
BoomCMS\Support\Helpers::next() | $next() | Get the next page in a sequence
BoomCMS\Support\Helpers::prev() | $prev() | Get the previous page in a sequence
BoomCMS\Support\Helpers::getTags() | $getTags() | Get the tags which are applied to a page
BoomCMS\Support\Helpers::getTagsInSection() | $getTagsInSection() | Get the tags which are applied to the children of a page

