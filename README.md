# What is it

This script is based on Jon Hicks original [SaveLayersAsPNG][SaveLayersAsPNG] script
which exports the top layers one by one.

When you're working on some big UI designs, you usually have lots of layers and sublayers, things that have to always stay visible, or some more complex scenarios.
This script will export layers recursively based on some flags at the end of the layer name.

# Layer flags

You can add a special flag at the end of a layer to control it's rendering:

* **`(+)` - always visible** - good for backgrounds, headers and footers, ...
	
* **`(-)` - ignore layer**

* **`(~)` - popup layer** - useful for overlays and popups, the script will export once with the layer hidden, and once visible.

* *no flag* - 

# Example

![](https://github.com/cri5ti/ai-layers-export/raw/master/sample/overlay.png)

![](https://github.com/cri5ti/ai-layers-export/raw/master/sample/layers.png)

## Exported files:

	acme-home-hovering-(~).png
	acme-home-popup-(~).png
	acme-home.png
	acme-product-big-(~).png
	acme-product.png

![](https://github.com/cri5ti/ai-layers-export/raw/master/sample/export/acme-home-hovering-\(~\).png)
![](https://github.com/cri5ti/ai-layers-export/raw/master/sample/export/acme-home-popup-\(~\).png)
![](https://github.com/cri5ti/ai-layers-export/raw/master/sample/export/acme-home.png)
![](https://github.com/cri5ti/ai-layers-export/raw/master/sample/export/acme-product-big-\(~\).png)
![](https://github.com/cri5ti/ai-layers-export/raw/master/sample/export/acme-product.png)

[SaveLayersAsPNG]: http://www.hicksdesign.co.uk/journal/illustrator-exporting-layers-to-png