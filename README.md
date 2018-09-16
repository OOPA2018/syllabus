---
layout: default
permalink: /
---

#WORK IN PROGRESS

# <img src="assets/logo.png" alt="class logo" class="logo"/> Object-Oriented Programming with Applications syllabus

***Acknowledgement: This is a fork of https://github.com/advanced-js/syllabus. If you are a teacher or interested in the design of the course, see the [meta](https://github.com/advanced-js/syllabus/blob/gh-pages/meta.md) document.***

* **Course:** [MATH11152](http://www.drps.ed.ac.uk/18-19/dpt/cxmath11152.htm)
* **Lecturer:** Witold Gawlikowicz, [v1wgawli@ed.ac.uk](mailto:v1wgawli@ed.ac.uk)

## Course Description

It is a fast paced course starting from C#/.NET basics and quickly moving to more advanced object-oriented concepts and applications spanning numerical methods, computational mathematics and quantitative finance. 

While it's an assignment-only course, the workload is still quite high and every year a few students fail this course. You will need to make sure you work through the tutorial sheets and lecture material regularly to clear-up any doubts as they come up and make the most of the teaching staff's help before heading off to work on the main project during the winter teaching vacation.

Computers are provided in the lab, though you are encouraged to bring a laptop for in-class exercises.

## Prerequisites

* At least one semester of an undergraduate course dedicated to programming (in any language). Understanding of flow control, methods/functions and some basics of data structures. This requirement is for both UG students and PGT students from MSc programmes other than MSc Computational Mathematical Finance.

## Course Overview

We will dive into the nuances of JavaScript, how prototypal inheritance compares to classical inheritance, and how this can be used to build dynamic and complex web applications.  Modern tools like jQuery and BackboneJS will be discussed, but students will learn the building blocks of these frameworks and after this course be able to understand what is happening under the hood.  The focus will be on development for browsers, though most applies to other systems like Node.js, Phonegap, etc.  Topics covered include:

* Encapsulation, closures and scope
* Classical vs. prototypal inheritance
* The event loop
* AJAX and JSONP
    * local
    * remote (e.g. Foursquare)
* Creating MVC-style models (a'la Backbone.js) from scratch
* Test- and Pseudocode-Driven Development

Topics will be demonstrated through live-code examples/slides, available at [advanced-js.github.io/deck](http://advanced-js.github.io/deck/).  Additional exercises will completed in-class.

See [this interview](https://web.archive.org/web/20140306162909/http://blog.masterstreet.com/2013/09/05/interview-with-aidan-feldman-instructor-at-nyu-scps/) for more background.

## Homework/Projects

All assignments are listed within the [Course Outline](#course-outline).

### Workflow

If you're using GitHub Desktop, these general instructions will help:

* <https://guides.github.com/activities/forking/>
* <https://help.github.com/desktop/guides/contributing/>

Enabling `Edit`->`Automatically Sync after Committing` is recommended. Here are the steps:

1. Fork the repository for the exercise/project (found under [github.com/advanced-js](https://github.com/advanced-js)).
1. Clone the repository to your computer.
1. Open the `index.html` file in a browser and open the Developer Tools.
1. Modify the files to complete your solution.
1. Refresh the `index.html` page to see the results, and repeat.
1. Make sure all of your code is committed.
1. Push/sync up to GitHub.
1. [Create a pull request](https://help.github.com/articles/creating-a-pull-request/) on the original repository. All assignments are due at the start of the following class, unless otherwise specified.
1. You can continue to push fixes and improvements until the close date (listed in Classes) – just add a comment in the pull request to let me know it's been updated.

When the pull request is created, you should see a message saying that "the Travis CI build is in progress" – this means that your solution is being automatically checked for syntax errors.  If this "build" ends up failing (which will show a red "X"), click through the "details" link and scroll to the bottom to see what the errors were.  Per the [requirements](#requirements) below, please fix the issues and push up the changes.

Feedback will be given in the pull request, so please respond with your thoughts and questions!  You are welcome to open the pull request early as a work-in-progress if you are stuck and want to ask a question.  Note that your solution will also be live at `http://USERNAME.github.io/EXERCISE`.

### Requirements

These apply to real life, as well.

* [Travis CI](https://docs.travis-ci.com/) build should pass, which includes:
    * All HTML files should pass [W3C Markup Validation](http://validator.w3.org).
    * All written JS should pass [JSHint](http://jshint.com).
* Must apply "good programming style" learned in class
    * Functions should be "short" (see [Sandi Metz's rules for developers](https://robots.thoughtbot.com/sandi-metz-rules-for-developers)).
    * Optimize for readability.
        * ["Programs must be written for people to read, and only incidentally for machines to execute." -Harold Abelson](https://www.goodreads.com/quotes/9168-programs-must-be-written-for-people-to-read-and-only)
    * Avoid using anonymous callbacks within other functions, especially if the callback is more than one or two lines.
    * For projects, use Object-Oriented Programming.
* Any borrowed code must be properly [annotated](#instructor).

## Course Outline

### Class 1

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Are you new to front-end web development? Here&#39;s a secret: no one else really knows what they&#39;re doing either.</p>&mdash; Nicolas (@necolas) <a href="https://twitter.com/necolas/status/291978260433219584">January 17, 2013</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

1. Introduction
    * Put name on sticky note on back of monitor
    * Discuss what the class is going to cover
    * Everyone introduce themselves
        * Name
        * What you "do"
        * What are your goals for the class?
        * What's something in JS (or technology) you worry that your peers understand but you don't?
1. Setup
    * How many people are comfortable with Git/GitHub?
    * Install [GitHub Desktop](https://desktop.github.com/)
        * If you are comfortable with Git already, you can skip this.
    * Sign up for GitHub
1. GitHub workflow
    * Walk through [workflow](#workflow)
    * Create pull request on [students repository](https://github.com/advanced-js/students)
1. Explain how slides work
1. Get through `countdown_exercise` slide
1. Talk through [requirements](#requirements)

#### Homework

* Join [the chat room](https://gitter.im/advanced-js/syllabus).
* [Set up your GitHub profile.](https://github.com/settings/profile)
* Access [NYU Classes](https://newclasses.nyu.edu) page, where grades will be posted.
    * [Documentation](https://wikis.nyu.edu/display/nyuclasses/Student+Quick-Start)
* Read [JavaScript Garden](http://bonsaiden.github.io/JavaScript-Garden/).
* Finish up and submit [echo](https://github.com/advanced-js/echo) and [countdown](https://github.com/advanced-js/countdown) exercises.
* Complete [blink](https://github.com/advanced-js/blink) exercise.

### Class 2

1. Look at various approaches for `countdown()`
    * Show recursive solution
1. Developer Tools walkthrough
    * Elements (HTML)
    * Console (JS)
    * Scripts (JS)
1. Pair program to build [Memory v1](https://github.com/advanced-js/memory) (see [pairing tips](#pairing-tips))
1. Cover OOP, though "oop_inheritance" slide
    * [Encapsulation example](http://jsbin.com/baqopu/1/edit?css,js,output)
    * Look at [Backbone.js Events](http://backbonejs.org/docs/backbone.html)

#### Homework

* Read [Mozilla's Introduction to Object-Oriented Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript)
* [OOP exercise](https://github.com/advanced-js/oop), through V2
* [Memory v2](https://github.com/advanced-js/memory#v2) (individual)

### Class 3

1. Code review Memory
1. Get through [`oop_inheritance`](http://advanced-js.github.io/deck/examples/oop_inheritance/) slide
1. Cover automated testing
    * Build up a test framework from scratch
    * Examples in QUnit
        * [Simple](http://jsbin.com/woqusi/edit?html,js,output)
        * [Classes](http://jsbin.com/nukamun/edit?js,output)
        * [QUnit documentation](http://qunitjs.com/)
    * Other frameworks
1. Cover AJAX/CORS/JSONP ([files](https://github.com/advanced-js/deck/tree/gh-pages/demos/ajax))
    * Network tab in Developer Tools

#### Homework

* Read [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)
* Complete [OOP exercise](https://github.com/advanced-js/oop) through V4.
* [Memory V3](https://github.com/advanced-js/memory#v3)

### Class 4

1. Finish slides
1. Getting Serious example
    * Quick intro to Backbone.js
        * [Boilerplate](http://jsbin.com/IGivato/1/edit?html,js,output)
        * Click the Box [example app](http://jsbin.com/IGivato/5/edit?css,js,output)
        * TDD?
1. Multiple async
    * [Promises](https://github.com/advanced-js/deck/tree/gh-pages/demos/ajax/promises)/[jQuery.Deferred](http://api.jquery.com/jQuery.Deferred/)
    * Possibly show [async](https://github.com/caolan/async#control-flow-1) library?

#### Homework

* [Learn about AJAX](https://github.com/advanced-js/deck/tree/gh-pages/demos/ajax#readme)
* [Mashup](https://github.com/advanced-js/mashup)
* Improve your previous assignments

### Class 5

1. Present and code review Mashup projects
1. Possible topics (vote?):
    * Node.js
        * Server "Hello World" (from [Node.js homepage](http://nodejs.org/))
            * [HTTP module docs](http://nodejs.org/api/http.html)
        * HTTP requests
            * [Status codes](http://pretty-rfc.herokuapp.com/RFC2616#status.codes)
            * Headers
        * CommonJS?
    * [Regular Expressions](https://github.com/advanced-js/deck/tree/gh-pages/demos/regex.html)
        * Convert live input from a text area, e.g.
            * Link Twitter handles
            * Substitute select words for emoji, using [emoji-css](http://afeld.github.io/emoji-css/)
    * Object-Oriented design
    * [Code Retreat](http://coderetreat.org/facilitating/structure-of-a-coderetreat) – possible "problems":
        * [Game of Life](http://coderetreat.org/gol)
        * Tic Tac Toe

## Resources


### Tools

* code validation: [JSLint](http://jslint.com) / [JSHint](http://jshint.com)
* debugging:
    * [Chrome Developer Tools](https://developer.chrome.com/devtools/index)
        * [Official debugging tutorial](https://developer.chrome.com/extensions/tut_debugging)
        * Tutorial: [JavaScript Diagnosis](http://www.macwright.org/2015/03/10/javascript-diagnosis.html)
    * [Firefox Developer Edition](https://www.mozilla.org/en-US/firefox/developer/)
* sharing code snippets: [gist.github.com](https://gist.github.com/)
* asking questions: [Stack Overflow](http://stackoverflow.com/)

#### GitHub

* Git and GitHub
    * [Official GitHub Help](https://help.github.com/)
    * [Recommended resources](http://hackerhours.org/resources.html#github)
* GitHub Pages
    * [Official site](https://pages.github.com/)
    * [Thinkful guide](http://www.thinkful.com/learn/a-guide-to-using-github-pages/)

#### HTML/CSS/JS Sandboxes

* [JS Bin](http://jsbin.com/) (recommended)
* [bl.ocks.org](http://bl.ocks.org/)
* [Cloud9](https://c9.io/)
* [CodePen](http://codepen.io/pen/)
* [JSFiddle](http://jsfiddle.net/)
* [Mozilla Thimble](https://thimble.mozilla.org)
* [Plunker](http://plnkr.co/)
* [rawgithub.com](http://rawgit.com/)

#### Frameworks

* Framework comparison: [TodoMVC](http://todomvc.com)
* [Testing](https://coderwall.com/p/ntbixw)


## Grading

* Exam - 0% (this is an assignment-only course)
* Assignment 1 - 5%
* Assignment 2 - 15%
* Final Project – 80%

## Statements on Plagiarism


