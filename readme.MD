# Timeline

## Project Overview

About
TimelineTS is a TypeScript library designed to simplify the creation and management of interactive timelines in web applications. It provides a flexible and customizable timeline component, allowing developers to seamlessly integrate timelines into their projects.

## Table of Contents
- [Usage](#usage)
- [Styles of Timelines](#styles-of-timelines)
  - [Timeline - classic](#timeline-classic) 
  - [Timeline - inline](#timeline-inline)
  - [Timeline - inline_circle](#timeline-inline-circle)
  - [Timeline - inline_classic](#timeline-inline-classic)
  - [Timeline - arrow](#timeline-arrow)
  - [Timeline - arrow_reverse](#timeline-arrow-reverse)
  - [Timeline - line_arc](#timeline-line-arc)
  - [Timeline - arc](#timeline-arc)
  - [Timeline - arc_dot](#timeline-arc-dot)

## Usage

To integrate this timeline library into your project, follow these simple steps:

1. **Include the Library Files:**

   Add the library's JavaScript and CSS files to your project. 

   ```html
   <!-- Add this to the <head> of your HTML file -->
   <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/shoaibn98/Timeline/Timeline.min.css">
   <script src="https://cdn.jsdelivr.net/gh/shoaibn98/Timeline/Timeline.min.js"></script>
   ```
2. **Initialize the Timeline:** 
    make an empty `div` tag with `Timeline_Timeline` class name and define some `id` for this Elements. 
    You have to give this `id` as `targetId` to your data Option.
    In your JavaScript file, create an instance of the timeline and customize it according to your needs.
    ```html
        <div class="Timeline_Timeline" id="myTimeline" >
        </div>
    ```
    ```JavaScript
     
    const option={
            targetId: "myTimeline", // *required : ID of target div elements
            width: 400, // *required : to set Total width of timeline
            offset: 150, // *required : to set distance between each Event 
            timeline: "arrow_reverse", // *required : style of Timeline
            data: [  //*required : data to show on timeline
                ["2021", "Old Event", "Description"],
                ["2024", "current Event", "Description"],
                ["2026", "Future Event", "Description"], 

            ],
            background: "#fff" // optional : to set background color
    }
    const myTimeline = new Timeline(option);
    ```

## Styles of Timelines



### timeline classic
```JavaScript
const option={
    //...
    timeline="classic";
    //...
}
```
![](/img/classic.png)

### timeline inline
```JavaScript
const option={
    //...
    timeline="inline";
    //...
}
```
![](/img/inline.png)

### timeline inline circle
```JavaScript
const option={
    //...
    timeline="inline_circle";
    //...
}
```
![](/img/inline_circle.png)

### timeline inline classic
```JavaScript
const option={
    //...
    timeline="inline_classic";
    //...
}
```
![](/img/inline_classic.png)

### timeline arrow
```JavaScript
const option={
    //...
    timeline="arrow";
    //...
}
```
![](/img/arrow.png)

### timeline arrow reverse
```JavaScript
const option={
    //...
    timeline="arrow_reverse";
    //...
}
```
![](/img/arrow_reverse.png)

### timeline line arc
```JavaScript
const option={
    //...
    timeline="line_arc";
    //...
}
```
![](/img/line_arc.png)

### timeline arc
```JavaScript
const option={
    //...
    timeline="arc";
    // OR
    timeline="arc_dot";
    //...
}
```
![](/img/arc.png)


- ## New Style coming soon

made with ♥  by  [Shoaib Norouzi](https://shoaibnorouzi.alwaysdata.net)
