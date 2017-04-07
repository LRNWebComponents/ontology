# LRN Ontology
A simple design language for expressing education concepts based on [webcomponents](http://webcomponents.org) and [atomic design](http://atomicdesign.bradfrost.com/table-of-contents/).

# Guiding Principles
* Atomic Design. LRN focuses on the molecule and organism level
* Design is abstracted from Instruction
* Accessibility, elements should be to the highest degrees of accessibility
* Readability at a glance, elements should be able to be understood by looking at them
* Instruction will use Design & have a default method of visualization
* This should work for visually communicating a course on a completely static html page
* Stay at the molecule / organism level (instructionally). Example: Assignment, Term
* Simple naming convention to allow for more to be added easily
* 0 hierarchy connotation in tags (for example: lrn-assignment not lrn-instruction-assignment)
* Stick to stock webcomponents capabilities as much as possible when creating design components

# Guiding Questions
* How are we improving potential learning outcomes for learners?
* How are we making faculty lives easier?
* How are we making instructional designers' lives easier?
* Are we improving design, context, clarity, and accessibility of our resources with this decision?

# Who LRN is for
**Students** who want a cohesive visual experience across solutions

**Instructors** who want simple, readable HTML to express their teaching

**Instructional Designers** who want expressive HTML to help meet course objectives

**Developers** who want to build learning technologies to an open standard across design specifications

---
The LRN Ontology is broken down into four families:
## lrn
This is what people would add into an html field. It's the instructionally focused element, told to render a certain way. Examples would be readable by the lay-person such as `<lrn-assignment label="Assignment 1">` or 
```
<lrn-lesson number="1" label="Introduction to Polymer" icon="myicon.png">
```
These elements have no connotation of design on their own and so each needs to utilize a lrndesign such as `design="card"` attribute in order to be presented to users.
## lrndesign
This is for the visual representation of an instructional concept (because instruction needs designed). This makes the instructional component visually make sense to end users. Examples of this would be things like `<lrndesign-card>` or `<lrndesign-imagegallery>`. lrndesign components COULD be used on their own to represent information though the preference is towards supplying visualization to items in an instructionally significant manner. For example, instead of an imagegallery, using a 

```
<lrn-examples display="imagegallery">
{<img tags in here/>}
</lrn-examples>
``` 

in order to provide examples or highlight instructional resources in some manner.
lrndesign is also where we provide designed wrappers for html element architypes. For example, a `<blockquote>` tag has a matching `<lrndesign-blockquote>` tag which wraps and expands the utility of `<blockquote>`. This would then be implemented in a `<lrn-quote>` tag, abstracting the design options away from the significance of the tag semantically. This can get confusing when it comes to in page elements like aside, blockquote and p tags so having a consistent hueristic for defining and implementing them is critical. 
## lrnsys
These elements are for providing systematic design integrations as well as reusable elements across other design components. These are things that aren't really designed to work on their own but to help inform the usage of other components. Examples of this would be a `<lrnsys-progress>` which could visualize data about progression or `<lrnsys-contextmenu>` which could provide a standard way of presenting contextual menu items. These are structural atoms that wouldn't be used on their own.
## hax
HAX is short for Headless Authoring eXperience. This is an initative on the part of LRN developers to make the web natively a platform for authoring instead of wrapping additional layers around editing and modifying the web via other systems. HAX is tangentially related to LRN because all `<lrn>` components will have support for HAX, paving the way for more solutions to use HAX on their own. By being headless, the authoring experience won't be tied to a single solution so we can improve the web as a whole.
## oer
OER is short for Open Educational Resources. It's a movement in education to make material free, open, and generally more accessible then it had been in the past. By encouraging instructors to produce educational materials in the open, others can learn beyond those paying for formalized education. The oer tag will be used to implement and mix the [OER Schema ontology](http://oerschema.org) into resources. The idea is to do so in such a way that end-users aren't aware they are tagging things with pedagogically significant metadata tags, but that they are building meaningful interfaces which happen to have this wired up already.
