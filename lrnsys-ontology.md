# lrnsys ontology
These are components that help glue the experience together. They generally aren't used by themselves as they are at the atomic level but are used in lrn and lrndesign components in order to create consistent behaviors and experiences downstream.
## [lrnsys-behaviors](https://github.com/LRNWebComponents/lrnsys-behaviors)
- provides behaviors to be implemented by lrn and lrndesign components that desire object consistency across elements
- useful for building new lrn components that have a display connotation (for example)
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
- lrnsys-xapi
## lrnsys-xapi
- an xapi statement generator
- callback location
```
<lrn-xapi callback="whatever.com/xapi">
{
	"verb": "viewed",
	"actor": {
		"mbox": "btopro@outlook.com",
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
