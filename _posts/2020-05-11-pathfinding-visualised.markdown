---
layout: post
title:  "Visualising Dijkstra's algorithm with P5.js"
date:   2020-05-11 13:48:14 +0100
---

<img src="/assets/images/dijkstra.png" loading="lazy">

Ever since I first learned about graph-traversal and pathfinding algorithms, they've interested me. It might be because of the real-world applications, or it could be because of my years playing _Age of Empires_ on Windows XP, watching miniscule Hoplites scurry about on their deathly mission. 

In learning about graphs and graph traversal, one method came up more than others – Dijkstra's algorithm. At the same time, I was focusing a lot of my energy on learning P5.js, a brilliant library for creating art with JavaScript. I decided to create a small visualisation of Dijkstra's algorithm, something that would allows users to play around with graphs – adding nodes, edges, and changing their position. 

## The tool

[P5.js](https://p5js.org/) is one of my favourite things, ever. As a person who thrives on _making stuff_, I'm surprised it took me so long to find P5, and to really get to grips with it. At its core, P5.js is a library for creative expression, turning statements, loops and logic into art. Real, actual art. I'm no great artist myself, but the P5 community contains many - and you can see their work on the [P5.js website](https://p5js.org/showcase/), on [Reddit](https://www.reddit.com/r/processing/top/?t=all), and on [Twitter](https://twitter.com/p5xjs/media). 

P5.js itself is a project of the [Processing Foundation](https://processingfoundation.org/) - an organisation helping people learn to code through the visual arts.


## Dijkstra's algorithm

Rather than attempt to explain what has already been explained so well across the internet, I'll instead link to the resources that helped me grasp Dijkstra's, and graphs as a whole. They are, in no particular order: 

* The brilliant Base CS podcast, which first stoked my interest in Computer Science: 
* * https://www.codenewbie.org/basecs/106
* * https://www.codenewbie.org/basecs/107
* [Computerphile](https://www.youtube.com/watch?v=GazC3A4OQTE)
* Clément Mihailescu's own Pathfinding Visualizer (a great inspiration and starting point): https://www.youtube.com/watch?v=msttfIHHkak&t=1072s


## The visualiser

The visualiserallows you to: 
* Place nodes
* Add edges between nodes
* Drag nodes
* Double-click to set start/end node
* Reset start and end
* Reset graph

Barring some iffy CSS, and some key missing features, I'm proud of this litte thing. I encourage you to go and have a play with it – it still amuses me, and I built it more than three months ago. 

Currently, you're not able to: 
* Delete individual nodes 
* Remove edges
* Select multiple nodes/edges for dragging/deletion
* Add other weighting (not jsut distance)
* Add directions to edges (represented as infinite distance)