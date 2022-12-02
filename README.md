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

transform:scale(0); makes the menu (or property) unclickable.

To target a child of an element in CSS, use >.
For example:
.menu > .list{}
targets elements with the list class that are childs of the menu parent class.

## JavaScript Events

Use this function to catch errors while coding:

const selectElement = (selector) => {
const element = document.querySelector(selector);
if (element) return element;
throw new Error(
`Something went wrong, make sure that ${selector} exists or is typed correctly.`
);
};

## Shortcuts

Ctrl + b toggles the left menu in VsCode.
Alt + b duplicates lines in vscode.

## Closing Remarks

Overall, this tutorial is a good at showing how to build a website.

The tutorial fully utilitizes CSS variables to create a very consistent color theme.

The CSS is divided by sections such as a nav, blog, posts, etc. This makes it a bit more managable.

However, I feel that using SASS would be a great benefit. Using variables is easier, and you can subdivide each section allowing you to easily focus on the area of interest.

In terms of the HTML, the class names are fairly consisent. This opens the ability of manipulating styles via JavaScript by changing class names. I believe this is the reason why there is such emphasis on class versus id's.

The SwiperJS works great, and is fairly easy to implement. Definitely a good tool to have.

The main shining star is the overall mobile-first design approach. Each section has its respective grid container whose contents is display: flex. This makes moving elements around when it comes to responsive design much easier. Using flex for the entire document makes it difficult to rearrange.
