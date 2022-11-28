# thirty-day-challenge-blog

## Goals:

Create a static blog that allows for studying via a _hopefully_ simple flash card system.

## Log:

11/28/2022 - The 30-Day Coding challenge Starts!

Currently following a Create a Blog course by freeCodeCamp.org - https://www.youtube.com/watch?v=Aj7HLsJenVg

The plan is today follow the course and on the following days rebuild it.

Current Tech:
Uses Swiper, an API for slides.

## Notes

### Nav - Index

When creating the nav bar, the list elements are placed inside a div(#menu) in order to make menu easier to manipulate into and out of mobile view (responsive).

Elements that are to be removed depending on size is given a hidden class. For example screen-lg-hidden is used to hidden the sign up option from the menu when the screen is large. A bigger sign up button is already visible when the screen is of proper size.

### Nav - CSS

To create variables in CSS:
--variable-name: someProperty

Wrap variables in :root{} to give the variables global scope in the css file.

To make font sizing easier, the html (document) font-size is set to 10px. Thus, to get 16px, it is simply 1.6rem.
Font-size is then changed to 62.5%, which is the same as 10px. This is done so that the page zooms more constantly, but its not mandoratory.

## Shortcuts

Ctrl + b toggles the left menu in VsCode.
Alt + b duplicates lines in vscode.
