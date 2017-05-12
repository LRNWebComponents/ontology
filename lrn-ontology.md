# lrn Learning Ontology

This is intended to give users a guide to understanding the hierarchy of LRN components, their use-cases, properties and relation to other elements.
## behaviors
https://github.com/LRNWebComponents/lrnsys-behaviors contains the behaviors that you can mix into elements. lrn elements are there to abstract instructional / learning connotations away from design. The lrn elements will all implement the design elements that make sense. For this reason, all lrn elements will implement the lrnsys-behaviors for DisplayBehaviors. Not a developer? Then don't worry about this part. Just know it helps standardize and speed up the implementation of new instructional components in a variety of designs and styles.

(feedback that needs to find a home / be hashed out)
#1: Reminder icon for "Photograph Drawing-in-Progress Now!"
Why important? Quite literally, if a student forgets to stop and take the image at the designated stage of completion and proceeds to draw further, the moment is forever lost (and they lose points).
Example: Three layer drawing. "...if you want to use the salt technique you may use it on this layer. Let this layer dry and then take one in-process photo showing all four edges of the paper." <NEED ICON RIGHT HERE>" The second layer will provide..."
Beyond the immediate need, thinking about web component taxonomy. The instructional function is to alert or remind. Attention grabbing. We can talk that through at some point...
Other varieties of the same idea are "Photograph Completed Drawing" and "Photograph Drawing Detail". I would want the option of associating text to those; so, a symbolic  icon with an optional legend where I can specify how many images. That would be very helpful in a course like this. By using color and slight variation on the symbology of the icon itself, they would consistently signal the type of photo(s) to be taken at that point in the process and the min-max range of how many to take.
One last variation would be a (generic drawing) + title (text)....for other types of drawing activities in the course where she is asking for something unique but a "catch-all" reminder icon would suit it.
#1: Sidebar support (already discussed as aside)


Important but less so

#2 Drawing Examples visual treatment
Why important? Students really need to see a small handful of these, perhaps 3-5 at most at a given time.
Most often would be a small gallery in context, but would need to be flexible enough to be a single example if that is all we have.
Many were specified during authoring; alas, few came to be created. I will want some kind of component treatment for these in the fall (I will have examples from the summer pilot).
Frankly don't care/don't want these to "portal" into a larger gallery (little to no instructional value to that). All about specificity in context. File drawer might make good sense interface-wise.
Web component taxonomy thoughts: visual example.
#3 Image of Required Tools and Supplies w/ associated text list
Why important? Most helpful when delineated at the assignment level (very specific subset). Bear in mind, these are non-majors for whom many supplies are quite unfamiliar (a picture is worth a thousand words, but a picture PLUS words is better yet)
That said, same item used for a whole module (three assignments, what you will need for the next two weeks of your life) or the whole course (orientation checklist)
Thus, this page component would be used 15 times (for assignments), 5 times (for modules), and 1 time for the course as a whole...21 times +  in ART 020 alone.
#4 Minimum Time Required icon
Why important? Anna and Lori both emphasize this as an important consideration for students to learn to take stock of. Simple clock icon with associated text would do it.
Just by having two colors (and maybe a larger and smaller version of the icon), I could signal what the assignment as a whole will require at a minimum, and then intersperse time required for major sub-portions
#5 Questions to Consider panel
Visual call out of self-reflective questions not answered or submitted

Not critical but would like to have it someday

#6 Written Reflection panel
They write briefly for every assignment submission; minimally this should be a callout treatment within the page.
For ART 020, I don't need it to be any more than that (they use an assignment-specific Word template to submit images and the Reflection into Canvas; questions to answer are already there)
But, Studio courses might use this base plus an in-place completion (like you did for Joel/Peter)

#7 Book cover icon for readings
I can practically see Keith rolling his eyes at this and ranting about "sustainability"...whatever...with two books in play in this course, it would be a nice touch to have an image of each
New edition, replace one file, voila. Not a big deal.
#8 Written Source Citation page component
Just a page-bottom element; non-crucial, but begs for visual treatment to set it apart from other things
Lori has been providing these to indicate the sources she has relied upon in authoring

## lrn-activities
- a list of lrn-activity tags
- title (example: Required readings, steps to completion, etc)
- optional (optional boolean)
- url (optional, string, source to ajax load and template stamp lrn-activity tags)
- `<content>` made up of lrn-activity tags
## lrn-activity
- an individual activity to engage in
- title (example: Read chapter 1, Watch this video)
- url (optional, string, link to a place to engage in this activity)
- optional (optional boolean)

## lrn-lesson
- a container relating pages together
- title
- (multiple)lrn-competencies
- (multiple)lrn-page

## [lrn-page](https://github.com/LRNWebComponents/lrn-page)
- a page of instruction, simple wrapper element for quantification purposes

## [lrn-content](https://github.com/LRNWebComponents/lrn-content)
- a simple content element to indicate that this area is educational content. It's a wrapper that provides a title and then prints content so it's a useful way of offsetting material. This could be used just below lrn-page or multiple implementations of this in a single page to illustrate that there are multiple concepts / unique groupings of content.
- title
- `<content>` for body of everything

## lrn-material-list
- a list of multiple lrn-material to display them together
- title
- innerHTML (prior to presenting the materials needed)
- (multiple)lrn-material

## lrn-material
- a material needed to complete an objective in the course
- example: You will need a paint brush, toothpick, and slate to accomplish this
- title eg; Chalk
- details (optional) eg; Buy white and yellow chalk
- image (optional) eg; pieces of chalk
- icon (optional) eg; none
- url (optional) eg; link to university art supply vendor (others: go buy this book from ___ , go use codepen)

## [lrn-vocab](https://github.com/LRNWebComponents/lrn-vocab)
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
- quotation from a source / person
- quote
- attribution

## [lrn-aside](https://github.com/LRNWebComponents/lrn-aside)
- additional / associated information
- label
- `<content>`

## lrn-procedures
- steps to complete something, listing of tasks to accomplish
- (multiple)lrn-procedure
- type (number,bullet,required, optional)
## lrn-procedure
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
## [lrn-assignment](https://lrnwebcomponents.github.io/lrndesign-assignment/components/lrndesign-assignment/)
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
