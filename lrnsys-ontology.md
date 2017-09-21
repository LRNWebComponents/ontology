# lrnsys ontology
These are components that help glue the experience together. They generally aren't used by themselves as they are at the atomic level but are used in lrn and lrndesign components in order to create consistent behaviors and experiences downstream.
## [lrnsys-layout](https://github.com/LRNWebComponents/lrnsys-layout)
- Provide reusable layout widgets and elements for building systems
- Dialogs, drawers, collapselists, etc

## [lrnsys-behaviors](https://github.com/LRNWebComponents/lrnsys-behaviors)
- provides behaviors to be implemented by lrn and lrndesign components that desire object consistency across elements
- useful for building new lrn components that have a display connotation (for example)

## [lrnsys-button](https://github.com/LRNWebComponents/lrnsys-button)
- provide a consistent and accessible button with link, hover, icon and color capabilities
- Wrapper on top of standard paper-button + a tag functionality with support for iron-icon
- Useful for building interfaces and wiring up all "buttons" to present in a drop in accessible, well styled, and visually matching manner
## lrnsys-lti
- provide a tag that can do LTI launches for data, basically a glorified OAuth and iframe wrapper (woo)
## lrnsys-pdf
- Fork of https://www.webcomponents.org/element/IngressoRapidoWebComponents/pdf-browser-viewer
- Provide a way of visualizing a pdf in context
## lrnsys-lazyload
- Fork of the one that does that
- lazy load images as you get to them
## lrnsys-beacon
- a method of triggering an xAPI / caliper event
- activator (javascript callback to determine when to fire / event listener)
## [lrnsys-randomimage](https://github.com/LRNWebComponents/lrnsys-randomimage)
- add collection of images to a pool for random display
- use as base for a free writing, random prompt generation, etc. 
- eventually try to make it also include random text, random math, random sound, video clip, etc. 

## lrnsys-xapi
- an xapi statement generator
- callback location
```
<lrn-xapi callback="whatever.com/xapi">
{
	"verb": "viewed",
	"actor": {
		"mbox": "btopro@some.place",
		"name": "btopro"
	},
	"authority"...
	"object"...
}
</lrn-xapi>
```
## lrnsys-nodetree
- a fork of https://www.webcomponents.org/element/vpusher/paper-tree?code=9c7226331a20915bea54
- a hierarchy that can be collapsed and expanded by passing it a simple json array
## lrnsys-randomimage
- input a pool of images
- generates a random selection from the pool
## image-inspector
- input a src for image
- zoom in, zoom out, rotate right, rotate left, mirror, and show image in new window
