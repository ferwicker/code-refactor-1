 # Horiseon Social Solution Services - Code Refactor
In this project, I refactored the exisiting code for Horiseon's homepage to make it compliant with accesibility standards. I also made changes to the HTML file to include semantic tags in the site structure, and consolidated and reordered the CSS styles in order to make it easier to modify and read if future changes are required.

## Why Accessibility?
Making the web more accessible helps users with disabilities, like visual impairments, use and understand website or other tools in the way that they are designed to be used, making for a more inclusive experience.

There has recently been a big push for accesibility, it has also become important for websites' SEO rankings. Although this gives businesses an extra reason to take accesibility into account, it has also opened important conversations around how people with disabilities use the web.

### Images
The most obvious aspect to take into account when checking code for accesibility is making sure that all images have alt text added. It is important to note that this does not mean every single image on the page needs to have a description. Images that do not add any value or information, such as icons with descriptive text next to them, have a null alt text to avoid redundancy, such as in the example below.

![Icon example](/README-assets/icon-example.png)

### Semantic HTML
Using semantic tags in HTML whenever possible instead of generic tags such as `<div>` elements helps give creen readers context of the page structure, improving accesibility. It also makes it easier for developers to read and modify the code in the future.

## Changes to HTML and CSS
In addition to accesibility focused changes, I made changes to the HTML and CSS files to make is easier to read, with comments and indentation, and consolidated several CSS classes that were redundant to make it easier to make changes to all elements that use the same style. Other changes were necessary due to the addition of semantic tags to the HTML.

*Example of consolidated classes:*

**Before** | **After**
------------ | -------------
Several identical classes | Consolidated class
Content in the first column | `.services {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    background-color: #0072bb;
    color: #ffffff;
}`


## Credits
For information on making emojis accesible to screen readers with alt text, this article and example from Adrian Roselli was useful: https://adrianroselli.com/2016/12/accessible-emoji-tweaked.html 