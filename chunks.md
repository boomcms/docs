---
currentMenu: chunks
---

# Chunks

An important concept to understand at the core of BoomCMS and its editing environment are page chunks.

Chunks define an editable area of the page which can be interacted with by users in the editing environment to change the content of a page.

Clicking on a chunk when in the editor will allow the content in that chunk to be edited.
There are many different types of chunks which can be defined within a page template and the editing interface with which a user is presented will depend on the type of chunk.

If a chunk doesn't contain any content then it will only appear to CMS users.

## Text
Text chunks define an area of editable page text and are edited with the WYSIWYG editor.

## Feature
Feature chunks provide a way of linking to (or featuring) another page within the site.
It cannot be used to link to an external URL.
When a feature chunk is edited it will present the user with the page tree with which to select a page to feature.

Depending on how the template is created a feature chunk could be used to display any chunks associated with the featured page or list the child pages.

## Asset
Asset chunks are a way of linking to assets (images, videos, documents).
Depending on the template setup it may be possible to add a link and associated text to appear with the asset.
In order to appear in the site an asset chunk must have an asset set regardless of whether any text or link is defined.

## Slideshow
Slideshows essentially behave as a collection of asset chunks.
Each slide must have an asset defined but may also have a link and text associated with it.
If the slideshow doesn't contain any slides with assets then it won't appear in the site.

## Link
A link chunk can be used to define any type of link including external URLs or email links.

## Linkset
As above expect multiple links can be added.
A linkset must contain at least one link to appear in the site.

## Time
A time chunk can be used to set a time and / or date.
The editing interface also provides the ability to set which date / time format to use.
Change the format can be used so that only the date is visible, only the time, or both.

## Location
A location chunk allows a location, specifically a latitude and longitude, to be saved.
A location can be saved with some associated text to present a human readable address.
In order to select a latitude or longitude editors may search by address or select a point on a map.

## HTML
A HTML chunks allows arbitrary HTML to be inserted into a page.
These can be useful to allow editors to insert JavaScript widgets into a pre-determined area of a template which is in keeping with the site's layout.
