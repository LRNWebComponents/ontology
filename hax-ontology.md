# HAX ontology
The HAX ontology are components that can be used to build a headless authoring user experience where the browser is actually the production platform in context. HAX defines data types and how they can be modified so that LRN components (or any webcomponent) that implements a hax attribute can map it's fields to how to edit those fields. This is not LRN specific but we are keeping it in mind since certain components won't go into LRN that will go into this (which then LRN will use natively for editing experience).

## hax-contextmenu
- Fork of https://www.webcomponents.org/element/Link2Twenty/l2t-context-menu
- Contextual / right click based menu

## hax-drag
- fork of https://www.webcomponents.org/element/ergo/polymer-dragula/demo/demo/demo2.html?code=ea16c156042c84e34167
- Drag and drop listings / behaviors

## hax-editable
- attributes { type (text, date, media, video, wysiwyg), options () }
- a fork of https://www.webcomponents.org/element/miztroh/wysiwyg-e for html mode there for example
- breaks out into sub-elements like editable-media, editable-text
