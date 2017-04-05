# Resources

## I know nothing about web components, where should I start?

- What exactly is Polymer?

This confuses lots of people at first. You might have heard the term 'Web Components' or 'Custom Elements' before, Polymer helps you make these.  Web Components and Custom Elements are not competeing technologies to Polymer, they are actual specs:

  - [Custom Elements Spec](https://www.w3.org/TR/custom-elements/)
  - [Web Components Spec](https://github.com/w3c/webcomponents)
  
Custom Elements spec allows you to define your own custom HTML tags / DOM elements. You're browser will allow you to define a tag called `flag-icon` and if you place `<flag-icon country="nl"></flag-icon>`, it will know how to interpert it.

The Web Components spec is meant to define how we as developers are going to manage the creation of Custom Elements.  They are made up of four individual specs that will work together:
  
  - Shadow Dom
  - Custom Elements
  - HTML Imports
  - HTML Templates

- Here is a great talk by Rob Dodson talking about what the development process looks like when building web components with Polymer: [End to End with Polymer](https://www.youtube.com/watch?v=1f_Tj_JnStA)

- Once you get the general concept you're going to want to start building something. There is a really good [getting started tutorial](https://www.polymer-project.org/1.0/start/first-element/intro) on the Polymer website.

- Now that you kind of understand how the Polymer world works you're going to dive into watching as many Polycasts videos that you possibly can.  Starting with these (note: some of these videos are span different versions, the syntax might slightly differ from the current version but the concepts are universal):

  - [Polymer CLI: Getting Started -- Polycasts #48](https://youtu.be/pj2lmXVa84U)
  - [Give your element an API -- Polycasts #16](https://youtu.be/7jolqbtIdiY?list=PLNYkxOF6rcIDdS7HWIC_BYRunV6MHs5xo)
  - [Accessible Components: Screen readers -- Polycasts #50](https://www.youtube.com/watch?v=Lktz1KXbTOU)
  - [Extending Native Elements -- Polycasts #15](https://youtu.be/OV8BvxpNQOs)
  - [Theming Elements -- Polycasts #17](https://youtu.be/omASiF85JzI)

- Now join the [polymer.slack.com](polymer.slack.com)
