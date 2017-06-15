---
layout: post
title: "The Course Map"
date: 2017-06-14
excerpt: "My undergraduate thesis"
tags: [project, R, Python, thesis]
feature: 
comments: true
project: true
---

## The Premise

Like the description suggests this is/was my undergraduate thesis. Anyone that has gone to college and not known exactly what they want to do understands the struggle of attempting to figure it out.
The most important thing is information. What courses can I take? What general classes (Gen Eds) do I need to take regardless of what I choose? What departments are there? Is there a special track I'm interested in? What's the most efficient path through all the courses and prerequisites? These questions and many others must be answered before one can even begin earning their degree. Unfortunately, many schools (mine included) only have their course catalog to offer students as a means of gaining information. So what you've got to work with is a textbook hundreds of pages big. I think there's a better way. 

## My Work

This is where my system comes in. The Course Map as I have dubbed it is my attempt to sketch out a system that can more effectively give students information on courses, departments, and the flow of prerequisites and corequisites. As in how can a student get from point A to point B. I do this through mapping out the courses in relation to one another. Instead of reading all the information you can look at a graph comprised of nodes. Each node is a class and prerequisite relationships are arrows in between nodes. This creates a network of sorts. 
<figure>
<img src= "/assets/img/courseMapExample1.png" style="width=150px;height=150px" target="_blank">
<figcaption>Example of a Map</figcaption>
</figure>
The overall function of the program goes like so. 

1. Course Catalog -> Python Text Miner
2. Python -> Condensed Info (TSVs & a SQLite Database)
3. Info -> R
4. R -> Web Application

Unfortunately this is not a smooth or automated pipeline for a number of reasons. One has to run the python text miner which outputs all the files and then you have to upload the files you're trying to visualize to the web application. Making the application more reactive is the main focus of future works. If you want to avoid the nitty gritties of the implementation you can simply explore the web app [here](https://shmog.shinyapps.io/coursemap). 

### To Be Continued . . . 
