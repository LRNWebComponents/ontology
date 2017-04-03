# lrn Learning Ontology

This is intended to give users a guide to understanding the hierarchy of LRN components, their use-cases, properties and relation to other elements.
# required properties
display: this is reserved for allowing users to define what template to run the tag through for output. Users can describecard as the display for example and know their output will wire the related properties up to a lrndesign-card element.
title: this should be used for the title or an object being presented. Not label or name whenever possible.
## lrn-lesson
- a container relating pages together
- title
- (multiple)lrn-competencies
- (multiple)lrn-page

## lrn-page
- a page of instruction, simple wrapper element for quantification purposes

## lrn-vocab
- vocabulary term
- term
- definition
- optional: know-source(multiple)

## lrn-lecture
- lecture, in place or reference to one in the real world
- title
- link (optional)
- duration (optional)
- date (optional)

## lrn-quote
- called out quote
- quote
- attribution

## lrn-additional
- additional / associated information
- title
- body
- theme
## lrn-steps
- steps to complete something
- (multiple)lrn-step
- type (number,bullet,required, optional)
## lrn-step
- a single step to completion
- text
- icon (optional)
- required / optional flag (optional)
## lrn-objectives
- listing of instructional objectives
- (multiple)lrn-objective
- theme (light,dark,color, etc)
## lrn-objective
- a single instructional objective
- title
- lrn-competency (optional associated competency if gaining a skill here)
- icon (optional)
- description
## lrn-competency
- a new skill expressed to the learner
- title
- description
- (multiple) lrn-xapi
## lrn-examples
- a series of examples of work
- (multiple) lrn-example
## lrn-example
- example work
- a resource that is an example of work to demonstrate expectations / possibilities
- media element of some form (video, img, audio, text)
## lrn-math
- offset mathjax loaded item
- equation (mathjax markdown)
## lrn-code
- offset code block
- language
- theme (light/dark)
- code
## lrn-assignments
- a list of lrn-assignment
- (multiple)lrn-assignment
## lrn-assignment
- an assignment of instruction
- title
- description
- due date (optional)
- {rest of OER ontology}
## lrn-roster
- a list of lrn-course-people
- lrn-course-person
## lrn-person
- someone associated to a course
- roles
- image
- icon
- first-name
- last-name
## lrn-course
- a sequence of course-objects
- title
- description
- instructor(lrn-person)
- machine_name
- number
- icon
- image
- colors
- (multiple)lrn-course-object
## lrn-course-object
- higher level grouping of materials in a course
- type (module,lesson,unit,etc)
- title
- icon
- image
- colors
## lrn-course-section
- organizational element for the offering of a course
- title
- dates
- term / semester (optional)
- lrn-course-person (instructor)
## lrn-knowledge-source
- Knowledge, references to knowledge source of some form
- url
- title
