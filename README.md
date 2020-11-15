 # Horiseon Social Solution Services - Code Refactor
In this project, I refactored the exisiting code for *Horiseon's* homepage to improve its compliance with accesibility standards. I also made changes to the HTML file to include semantic tags in the site structure, and consolidated and reordered the CSS styles in order to make it easier to modify and read if future changes are required.

## Table of contents
  - [Why Accessibility?](#why-accessibility)
    - [Images and alt text](#images-and-alt-text)
    - [Semantic HTML](#semantic-html)
  - [Changes to HTML and CSS](#changes-to-html-and-css)
    - [Example of consolidated classes](#example-of-consolidated-classes)
  - [Credits](#credits)

## Why Accessibility?
Making the web more accessible helps users with disabilities use and understand website or other tools in the way that they are designed to be used, making for a more inclusive experience.

There has recently been a big push for accesibility, and it has also become important for websites' SEO rankings. Although this gives businesses an extra reason to take accesibility into account, it has also opened important conversations around how people with disabilities use the web.

### Images and alt text
The most obvious aspect to take into account when checking code for accesibility is making sure that all images have alt text added. It is important to note that this does not mean every single image on the page needs to have a description. Images that do not add any value or information, such as icons with descriptive text next to them, have a null alt text to avoid redundancy, such as in the example below.

![Icon example](/README-assets/icon-example.png)

### Semantic HTML
Using semantic tags in HTML whenever possible instead of generic tags such as `<div>` elements helps give creen readers context of the page structure, improving accesibility. It also makes it easier for developers to read and modify the code in the future.

## Changes to HTML and CSS
In addition to accesibility focused changes, I made changes to the HTML and CSS files to make is easier to read, with comments and indentation, and consolidated several CSS classes that were redundant to make it easier to make changes to all elements that use the same style. Order was reorganised to match HTML order, unnecessarily specific selectors were modified. Other changes were necessary due to the addition of semantic tags to the HTML.

### Example of consolidated classes

**Before -**
*Several identical classes*

    .search-engine-optimization {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
    }

    .online-reputation-management {
        margin-bottom: 20px;
        padding: 50px;
        height: 300px;
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        background-color: #0072bb;
        color: #ffffff;
    }

    .social-media-marketing {
        margin-bottom: 20px;
        padding: 50px;
        height: 300px;
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        background-color: #0072bb;
        color: #ffffff;
    }

**After -**
*Consolidated class*

    .services {
            margin-bottom: 20px;
            padding: 50px;
            height: 300px;
            background-color: #0072bb;
            color: #ffffff;
    }

The final result is visually identical to the original site, but with better accessibility, code readability and structure. [View refactored site here.](https://ferwicker.github.io/homework-1-code-refactor/)

![Site screenshot](/README-assets/01-html-css-git-homework-demo.png)

## Credits
For information on making emojis accesible to screen readers with alt text, this article and example from Adrian Roselli was useful: https://adrianroselli.com/2016/12/accessible-emoji-tweaked.html 