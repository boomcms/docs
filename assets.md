---
currentMenu: assets
---

# Assets

Images, documents, and other website assets can be managed via the BoomCMS Asset Manager.
Site assets are inserted into pages via the Asset Picker which provides a more simplified interface for uploading and browsing assets.
Both the Asset Manager and Asset Picker are available to users who have the **manage_assets** role.

## Asset Metadata

Assets can be search searched and filtered across many metadata fields including:

* A title and description
* File size
* File type
* The number of times an asset has been downloaded by a site visitor
* When the asset was uploaded
* A simple tagging system

## Image editing

The asset manager features a simple image editing interface which supports rotating and cropping images.

## Image resizing

Height and width parameters can be added to asset URLs in order to resize images automatically.
This can be used by template developers to ensure that the correct size image is always available.
Resized images are cached to reduce loading times.

The format for asset URLs is:

```
/asset/view/<id>/<width>/<height>
```