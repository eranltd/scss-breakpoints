# scss-breakpoints
Best Practice, Surgery level responsive design breakpoints system both width and height media queries

---
layout: docs
title: Breakpoints
description: Breakpoints are customizable widths that determine how your responsive layout behaves across device or viewport sizes
group: layout
toc: true
---

## Core concepts

- **Breakpoints are the building blocks of responsive design.** Use them to control when your layout can be adapted at a particular viewport or device size.

- **Use media queries to architect your CSS by breakpoint.** Media queries are a feature of CSS that allow you to conditionally apply styles based on a set of browser and operating system parameters. We most commonly use `min-width` in our media queries.

- **Mobile first, responsive design is the goal.** Bootstrap's CSS aims to apply the bare minimum of styles to make a layout work at the smallest breakpoint, and then layers on styles to adjust that design for larger devices. This optimizes your CSS, improves rendering time, and provides a great experience for your visitors.

## Available breakpoints

 includes five default breakpoints, sometimes referred to as _grid tiers_, for building responsively. These breakpoints can be customized.

<table class="table">
  <thead>
    <tr>
      <th>Breakpoint</th>
      <th>Dimension - Width</th>
      <th>Dimension - Height</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Small</td>
      <td>&lt;(0em, 40em); /* 0, 640px */</td>
      <td>&lt;(0em, 22.5em); /* 0, 360px */</td>
    </tr>
    <tr>
      <td>Medium</td>
      <td>&ge;(40.063em, 64em); /* 641px, 1024px */</td>
      <td>&ge;(22.5625em, 36em); /* 361px, 576px */</td>
    </tr>
     <tr>
      <td>Large</td>
      <td>&ge;(64.063em, 90em); /* 1025px, 1440px */</td>
      <td>&ge;(36.0625em, 50.625em); /* 577px, 810px */</td>
    </tr>
    <tr>
      <td>Extra Large</td>
      <td>&ge;(90.063em, 120em); /* 1441px, 1920px */</td>
      <td>&ge;(50.6875em, 67.5em); /* 811px, 1080px */</td>
    </tr>
    <tr>
      <td>Extra Extra large</td>
      <td>&ge;(120.063em); /* 1921px */</td>
      <td>&ge;(67.5625em); /* 1081px */</td>
    </tr>
  </tbody>
</table>

```scss

 @import 'src/assets/breakpoints.scss';
  //by width
  @media #{$xlarge-height}  { 
        display: block;
       }
    }
 
 //by height
 @media #{$xlarge-height-up}  { 
        display: block;
       }
    }
```
