# Problem Statement
Given a pre-constructed webpage, clean up the code within the html and css files to make it accessible while maintaining the same layout/design of the original page and allowing for future developers to quickly and easily follow/update the code layout.

You can see the webpage I have edited [here](https://thadkingcole.github.io/code_refactor)

# Required Tasks
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
<hr>

## HTML Structure
Since HTML semantic tags were chosen to be used, I implemented them with the following layout:
```
| header  |   nav |
| --------------- |
|      photo      |
| --------------- |
| section | aside |
| --------------- |
|      footer     |
```
[task list](#required-tasks)
<hr>

## Alt Image Attributes
In order to improve accessibility, appropriate alt attributes were added to all img tags.

[task list](#required-tasks)
<hr>

## Headings
Heading elements were reassigned to a sequential order to help differentiate headers within the different sections of the website. Although this can be done easily enough in CSS, I chose to utilize different header tags for each section to make the common styling to multple headers easier to edit within the CSS. The following was chosen as the section - header layout.
- header = h1
- section = h2
- aside = h3
- footer = h4

[task list](#required-tasks)
<hr>

## Page Title
"HoriSEOn Marketing" was chosen as the title for the page. This title is visible on the tab of the page.

[task list](#required-tasks)
<hr>

## Maintain Page Layout/Design
With all the changes being made to the code, it was important to ensure that the page looked identical to when I started since the design/layout of the page was not considered to need any changes. 

To see for yourself, commare the look of the current index.html to the one in this [commit](#14b8de5991763d99112d8791d4bb5f00d8a7f412)

[task list](#required-tasks)
<hr>

## Comments
HTML and CSS files both had no comments when I started. In HTML, I added comments to the start of different sections. I did the same in CSS while also explaining what some of the CSS was doing if not intuitively obvious based on the syntax.

[task list](#required-tasks)
<hr>

## Links
One of the links in the nav bar at the top right of the page was broken when I started. This was due to all the links referencing  IDs of the same name, and in one case that id did not exist. That ID was added to the appropriate place in the page so that the broken link now works.

[task list](#required-tasks)
<hr>

## CSS Consolidation
There were a number of repeated stylings and a number of extra IDs/classes that were broken down to smaller than necessary elements. IDs/classes that could be better grouped were combined, and repeated stylings were combined where it made since. Overall, the CSS file was reduced from 200 lines to 139!

[task list](#required-tasks)
<hr>