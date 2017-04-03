# construction guidelines for webcomponents
These are some general guidelines for our development of lrn, lrndesign, hax and lrnsys.

- Align with "the platform" but start at Polymer 1.0 until 2.0 reaches higher theshold of adoption
- Ensure `lrn` elements use `LRNBehaviors.DisplayBehaviors` so they have a consistent way of abstracting meaning from design
- Attributes in, Events out
- Always align methods with setters
  - set sets a property and then bubbles up an event to react to / makes a change
  - this helps outside libraries interact nicely with Webcomponents as if they are native elements
- Always look for existing elements to build off of
- Always wrap / encapsulate design elements in lrndesign versions so we can better shift them later if needed
- Always leverage iron- class of elements for atomic level operations
- Always name space lrn elements as having instructional meaning which then implement design
- Always keep lrn elements readable
- Try to align property names across components
- Try to use slot elements for lrndesign components and properties for lrn components
- Anything touching a specific platform should remain name spaced in that specific platform (elmsln-lmsless for example)
- wrap lrndesign elements in hax components when it makes sense
- elements always need to work with or without hax having a backend to talk to
