# System ontology
The system ontology are components that are reusable in learning systems. These are more functional then design or instructional elements through obviously have implications for the two of them.
## lrnsys-pdf
- Fork of https://www.webcomponents.org/element/IngressoRapidoWebComponents/pdf-browser-viewer
- Provide a way of visualizing a pdf in context
## lrnsys-lazyload
- Fork of the one that does that
- lazy load images as you get to them
## lrnsys-button
- Fork of https://www.webcomponents.org/element/PolymerElements/paper-button
- Button wrapper
## lrnsys-contextmenu
- Fork of https://www.webcomponents.org/element/Link2Twenty/l2t-context-menu
- Contextual / right click based menu
## lrnsys-drag
- fork of https://www.webcomponents.org/element/ergo/polymer-dragula/demo/demo/demo2.html?code=ea16c156042c84e34167
- Drag and drop listings / behaviors
## lrnsys-beacon
- a method of triggering an xAPI / caliper event
- activator (javascript callback to determine when to fire / event listener)
- lrnsys-xapi
## lrnsys-xapi
- an xapi statement generator
- callback location
- <lrn-xapi callback="whatever.com/xapi">
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
