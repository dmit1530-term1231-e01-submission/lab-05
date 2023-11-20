# DMIT1530: Lab 05

This lab is an individual activity, to be completed on your own. It is worth 5% of your overall grade.

For the due date and time, please refer to Moodle.


## Introduction

The website you will be building for this lab is a fictitious lifestyle blog that focuses on winter activities and décor. 

This website has three main areas, each of which covers a web component that we have learned in Module 3. In order, they are:

1. A hero banner with a pure CSS parallax scroll effect.

2. A one- or two-column flex layout that makes use of the `<picture>` element.

3. A horizontal scroll widget with multiple cards.

You will be given all the written content, the typographic styles, and CSS variables for colours and various repeating motifs. However, you will need to complete the markup and write the remainder of the CSS based upon your in-class demonstrations and the provided screenshots. 

Because the focus of this lab is on the web components you have learned in Module 3, there is no top-level navigation or footer. 


## Methodology

1. You will begin with the HTML. Although the written content has been provided to you, you will need to create the form and structure of the document. 

**Note**: Make sure that you complete all of the information in the `<head>` of the document and that your HTML passes validation. Any lab that does not pass validation will receive a mark of 0%.

2. Begin writing your CSS. At the top of the stylesheet, you have been given a list of variables and some utility classes. Your reset code also sets a typographic scale. Your task is to focus on the components and their intended functionality. 


## Hints

The hero banner uses the following declarations to create the frosted background for the text:

```CSS
 .some-element {
    backdrop-filter: blur(5px);
    background-color: #ffffff4a;
 }
```

The images in each card in the horizontal scrolling component have the following `border-radius`:

```CSS
 .some-element {
    border-radius: var(--border-radius) var(--border-radius) 0 0;
 }
```

This layout has only one media query. If you are unsure what the breakpoint should be, take the widths of the images in the `<picture>` element area into consideration. 

The cards in the horizontal scrolling widget are 21 rem wide.

---

## Rubric

This lab will be out of five (5) marks. You will be graded on the following criteria:

1. The hero banner uses a pure CSS parallax scroll effect. When the user scrolls through this area of the website, the background should remain fixed (i.e. not move) while the rest of the content scrolls (i.e. does move). (+1)

2. The second area is a simple flex layout that uses `<picture>` elements. The `<source>` or `<img>` inside of the `<picture>` change when the viewport reaches a specific width. This width should work in conjunction with the website's media query. (+1)

3. The third area is a horizontal scroll widget with eight cards. This area overflows only the container, not the viewport. There is a scrollbar that can be used to see the cards that do not fit within the viewport. (+2)

4. The styles and overall layout is as close to the screenshots as possible. (+1)
