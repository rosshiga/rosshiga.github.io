---
layout: project
type: project
image: images/w3card.png
title: w3card-blog
permalink: projects/w3card
# All dates must be YYYY-MM-DD format!
date: 2017-01-06
labels:
  - W3.CSS
  - Responsive Design
  - Blog Template
summary: A free open source blog template I developed using W3.CSS.
---
[GitHub: w3card-blog](https://github.com/rosshiga/w3card-blog)

[Demo project: EE491 (Cards may be hidden) ](https://demo.rosshiga.com)

<div class="ui small rounded images">
  <img class="ui image" src="../images/micromouse-robot.png">
  <img class="ui image" src="../images/micromouse-robot-2.jpg">
  <img class="ui image" src="../images/micromouse.jpg">
  <img class="ui image" src="../images/micromouse-circuit.png">
</div>

[W3Schools](https://www.w3schools.com) is a great resource for learning modern web design.
They release an open CSS framework called [W3.CSS](https://www.w3schools.com/w3css/default.asp).
I used this framework to create a Material Design card-like interface for blog posting.

Color scheming and themes are easily swappable by changing the referenced [W3.CSS pallet](https://www.w3schools.com/w3css/w3css_color_themes.asp). 
```html
<head>
...
    <!-- W3.CSS is an open source modern CSS framework http://www.w3schools.com/w3css/-->
    <link rel="stylesheet" href="http://www.w3schools.com/lib/w3.css">
    <!-- Change theme here ---> 
    <link rel="stylesheet" href="http://www.w3schools.com/lib/w3-theme-green.css">

    <title>w3card-blog</title>
    <link rel="stylesheet" href="assets/blog.css">
    <script src="assets/blog.js"></script>
</head>
```

I used this template as a simple form input for my [EE491 IoT Bike Lock](https://github.com/rosshiga/EE491_IoT) project.

I also started to explore Hexo static site generation using this template. If you know Hexo and would like to help me out please fork my [w3card-hexo repo](https://github.com/rosshiga/w3card-hexo).