# Problem Statement
Given a pre-constructed webpage, clean up the code within the html and css files to make it accessible while maintaining the same layout/design of the original page and allowing for future developers to quickly and easily follow/update the code layout.

You can see the webpage I have edited [here](https://thadkingcole.github.io/code_refactor)

## Required Tasks
- [x] [semantic HTML elements added where appropriate](#HTML-Semantics)
- [x] [structure of HTML elements follows a logical flow](#HTML-Structure)
- [x] [image elements have alt attributes](#Alt-Image-Attributes)
- [x] [heading attributes fall in sequential order](#Headings)
- [x] [added a concise, descriptive title](#Page-title)

## Additional Tasks
- [x] [maintained the page layout/design the same throughout](#maintain-page-layout/design)
- [x] [added comments to HTML and CSS files](#comments)
- [x] [fixed broken links](#links)
- [x] [consolidated some CSS styling where appropriate](#CSS-consolidation)
- [x] create and edit a high quality readme.md for this project
- [x] [Make HTML & CSS files w3 style compliant](#style-compliant)



# Explanations
## HTML Semantics
The original HTML code had a number of div tags with IDs the same as semantic HTML elements such as header and footer. To improve code readability, div tags corresponding to a semantic HTML element were changed to that element. For example:
```html
<div id="header"></div>
```      
was changed to
```html
<header></header>
```
[task list](#required-tasks)

---

## HTML Structure
Since HTML semantic tags were chosen to be used, I implemented them with the following layout:
```
| header  |   nav |
| --------------- |
|      photo      |
| --------------- |
| section | aside |
| article |  div  |
| article |  div  |
| article |  div  |
| --------------- |
|      footer     |
```
[task list](#required-tasks)

---

## Alt Image Attributes
In order to improve accessibility, appropriate alt attributes were added to all img tags.

[task list](#required-tasks)

---

## Headings
Heading elements were reassigned to a sequential order to help differentiate headers within the different sections of the website. Although this can be done easily enough in CSS, I chose to utilize different header tags for each section to make the common styling to multple headers easier to edit within the CSS. The following was chosen as the section - header layout.
- header = h1
- section = h2
- aside = h3
- footer = h4

[task list](#required-tasks)

---

## Page Title
"HoriSEOn Marketing" was chosen as the title for the page. This title is visible on the tab of the page.

[task list](#required-tasks)

---

## Maintain Page Layout/Design
With all the changes being made to the code, it was important to ensure that the page looked identical to when I started since the design/layout of the page was not considered to need any changes. 

To see for yourself, commare the look of the current index.html to the one listed earliest in its history.

[task list](#required-tasks)

---

## Comments
HTML and CSS files both had no comments when I started. In HTML, I added comments to the start of different sections. I did the same in CSS while also explaining what some of the CSS was doing if not intuitively obvious based on the syntax.

[task list](#required-tasks)

---

## Links
One of the links in the nav bar at the top right of the page was broken when I started. This was due to all the links referencing  IDs of the same name, and in one case that id did not exist. That ID was added to the appropriate place in the page so that the broken link now works.

[task list](#required-tasks)

---

## CSS Consolidation
There were a number of repeated stylings and a number of extra IDs/classes that were broken down to smaller than necessary elements. IDs/classes that could be better grouped were combined, and repeated stylings were combined where it made since. Overall, the CSS file was reduced from 200 lines to 150!

[task list](#required-tasks)

---

## Style Compliant
Although not required to edit how a webpage looks, it is important to follow industry standard style guides since it is likely that I will not be the only one to look at my code. For this project, I followed the [w3schools style guide](#https://www.w3schools.com/html/html5_syntax.asp). The given HTML and CSS files were already mostly compliant, but the following changes were made to improve style compliance:
- [x] change indent size from 4 spaces to 2 spaces on both HTML and CSS files.
- [x] set the viewport 

[task list](#required-tasks)