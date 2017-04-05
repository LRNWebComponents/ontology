# Resources

## What exactly is Polymer?

Polymer is library that helps you make production ready web components today! Polymer helps to ease some of the pain points around creating custom web components before the browsers have fully implimented the specs.  It has some tools, polyfills, helper functions, and syntastical sugar.  Kind of like jQuery for web components.

## Ok, what are web components?

This confuses lots of people at first. You might have heard the term 'Web Components' or 'Custom Elements' before, Polymer helps you make these.  Web Components and Custom Elements are not competeing technologies to Polymer, they are actual specs:

  - [Custom Elements Spec](https://www.w3.org/TR/custom-elements/)
  - [Web Components Spec](https://github.com/w3c/webcomponents)
  
Custom Elements spec allows you to define your own custom HTML tags / DOM elements. You're browser will allow you to define a tag called `flag-icon` and if you place `<flag-icon country="nl"></flag-icon>`, it will know how to interpert it.

The Web Components spec is meant to define how we as developers are going to manage the creation of Custom Elements.  They are made up of four individual specs that will work together:
  
- Shadow Dom
- Custom Elements
- HTML Imports
- HTML Templates

## No, that's ok I use Angular / React / Vue / Ember / Backbone / Knockout / Riot / Wordpress / Drupal / Jeckyll / Rails / Laravel / concreate5 / hand crafted HTML ...(page 1 of 10,000).  I don't need Web Components.

That's the beauty of web components, you can use them with everything! So hears the methodology, you can use web components for as much or as little of your web interface as you want.

## Ok I'm on board. Now what?

- Here is a great talk by Rob Dodson talking about what the development process looks like when building web components with Polymer: [End to End with Polymer](https://www.youtube.com/watch?v=1f_Tj_JnStA)

- Once you get the general concept you're going to want to start building something. There is a really good [getting started tutorial](https://www.polymer-project.org/1.0/start/first-element/intro) on the Polymer website.

- Now that you kind of understand how the Polymer world works you're going to dive into watching as many Polycasts videos that you possibly can.  Starting with these (note: some of these videos are span different versions, the syntax might slightly differ from the current version but the concepts are universal):

  - [Polymer CLI: Getting Started -- Polycasts #48](https://youtu.be/pj2lmXVa84U)
  - [Give your element an API -- Polycasts #16](https://youtu.be/7jolqbtIdiY?list=PLNYkxOF6rcIDdS7HWIC_BYRunV6MHs5xo)
  - [Accessible Components: Screen readers -- Polycasts #50](https://www.youtube.com/watch?v=Lktz1KXbTOU)
  - [Extending Native Elements -- Polycasts #15](https://youtu.be/OV8BvxpNQOs)
  - [Theming Elements -- Polycasts #17](https://youtu.be/omASiF85JzI)

- Now join the [polymer.slack.com](polymer.slack.com)
