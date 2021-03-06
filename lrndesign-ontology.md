# Design ontology
This is a listing of design components supported in lrn core. These are element agnostic and could be used as a stand alone with thier properties populated directly. These are all prefixed as lrn-design since this is the design side of the learning components. These names are draft and subject to change / enhancement.
## [lrndesign-abbreviation](https://github.com/LRNWebComponents/lrndesign-abbreviation/)
- A simple wrapper for an abbr tag to improve design flexibility
## [lrndesign-blockquote](https://github.com/LRNWebComponents/lrndesign-blockquote)
- A simple wrapper for blockquote to improve design flexibility and ensure a citation exists for the quote
## [lrndesign-contentblock](https://github.com/LRNWebComponents/lrndesign-contentblock)
- a simple content block that has a number of options for being presented

## lrndesign-materialwordart
- fork / based on https://github.com/johnnyboyct/material-word
- Provide a simple way of making cool wordart from letters / words
- *special note: we need to patch something downstream to be able to use this as it doesn't like 2-way data binding to word property :\*
## [lrndesign-card](https://github.com/LRNWebComponents/lrndesign-card)
- Fork of or based off of https://www.webcomponents.org/element/PolymerElements/paper-card and http://materializecss.com/cards.html
- Provide a way of representing an item for overview purposes / having a lot of information in a consistent space
## lrndesign-presentation
- Fork of or based off of https://github.com/ChristianKohler/web-presentation
- Provide a way of presenting a "power-point" style presentation of material to navigate through
## [lrndesign-contentsequencer](https://github.com/LRNWebComponents/lrndesign-contentsequencer)
- Wrapping of https://github.com/googlecodelabs/codelab-components
- Provide a "one page app" feel to a lesson that can function as a stand alone. https://www.youtube.com/watch?v=Dzv4ESis9AA for example describing this
## [lrndesign-contactcard](https://github.com/LRNWebComponents/lrndesign-contactcard)
- A stand alone contact card for presenting information about a person
- Probably useful for profiles and listings of users in a course

## [lrndesign-biocard](https://lrnwebcomponents.github.io/lrndesign-biocard/components/lrndesign-biocard/)
- A "meet your instructor" card for presenting static info about an instructor 
- Includes a button to schedule appointment with instructor, video conference link info, social info, etc. 
## [lrndesign-avatar](https://github.com/LRNWebComponents/lrndesign-avatar)
- fork of / based on https://www.webcomponents.org/element/Abe90/paper-avatar/demo/demo/index.html
- Provide a way of creating an icon for anything. It has support for jdenticon or doing it via letters or an image
## lrndesign-datatable
- fork of / based on https://github.com/Saulis/iron-data-table
- Provide a way of creating a table visualization to information that is sortable
- will have sub-elements of some form, probably iron atoms
## lrndesign-qr
- Fork of https://github.com/educastellano/qr-code
- Provide a way of easily generating a QR code for visualzing anything (most common use-case a link)
## lrndesign-progress
- Fork of https://www.webcomponents.org/element/vguillou/material-progress
- Provide a way of visualizing basic data about A vs B vs C
## lrndesign-chip
- fork of / based on https://www.webcomponents.org/element/WebPaperElements/paper-chip and/or http://bendavis78.github.io/paper-chip/paper-chip/index.html
- Provide a way of creating a small "chip", useful in overviews / "tag" style listings
## lrndesign-image
- Provide a simple wrapper on top of images for more advanced customizations
- Support for multiple output / format options such as..
  - **parallax**
    - fork of / based on https://www.webcomponents.org/element/vguillou/parallax-element/demo/demo/index.html
    - Provide a simple way of doing parallax images
- editor (photoshop thing) https://www.webcomponents.org/element/IngressoRapidoWebComponents/creative-photo-editor
## lrndesign-imagegallery
- Provide simple way of presenting a lot of images in a gallery of different formats
  - **random image presentation**
    - https://www.webcomponents.org/element/kilombo/random-image
  - **carousel**
    - https://www.webcomponents.org/element/annsonn/fancy-carousel?code=97356eb3339f5e4a4521
## [lrndesign-imagecarousel](https://lrnwebcomponents.github.io/lrndesign-imagecarousel/components/lrndesign-imagecarousel/)
- Provides carousel structure for image display 
- Navigate images side to side
## lrndesign-audio
- Ensure we have some control over what the browsers all want to default <audio> to mean
  - **simple**
    - fork of https://www.webcomponents.org/element/gorork/paper-audio-player & https://www.webcomponents.org/element/Link2Twenty/wave-player?code=3857636ac4044fd5743a
    - Simple wrapper on audio tag that's very clean and standardized
