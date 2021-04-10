# p5.anywhere Project Description

## Overview

I would like to create p5.anywhere, a client library with a matching server backend that will make it easy to create connected experiences between p5 sketches (and more) on any device.

The initial goal will be to create a portable server deployable with a single click, but a further goal would be a Processing-hosted community server, allowing for an even lower barrier to entry.

Example use cases include one-to-many scenarios (e.g. a performer sending data to audience devices), many-to-one scenarios, (e.g. an audience using phones to draw on a shared canvas) and many-to-many scenarios (e.g. a multi-user collaborative workspace for local and remote users).

## Qualifications

I have experience building tools for realtime connected systems in both academic and commercial contexts.

During a residency at NYU's [Future Reality Lab](https://frl.nyu.edu/), I created a javascript-based client and server for their multi-user VR project, HoloJam. During this time, I also built a generic system for connected experiences called [Khoros](https://scottmadethis.net/interactive/khoros/), which would partially serve as the foundation of p5.anywhere.

More recently, I created [Heat](https://scottmadethis.net/interactive/heat/), an extension for Twitch that allows audience members to directly interact with live video by clicking on the screen.

I also have experience working directly on Processing-related projects, including Hello Processing and Hello p5.js.

## Priority Area

The priority area I'm choosing to address is "Accessiblity". In teaching various workshops over the years on creating connected experiences with tools like p5, the server/networking component has consistently been a major sticking point.

I believe this is partially because it requires a new domain of networking knowledge that can be a bit overwhelming for beginners. It also opens up otherwise simple projects to all of the difficulties and concerns associated with creating and hosting custom server software.

I now make it a habit to develop a simple server setup for students to use before these sessions, but I've done this enough times that I believe I can create a more generic approach that will make it easy for anyone to prototype these kinds of connected setups with very little effort.

## Expected Results

At a minimum, this project will result in the creation of a p5.anywhere client library with an accompanying portable server.

Additionally, I plan to livestream all work sessions and post the resulting videos to YouTube. These sessions will both serve as documentation of the development process as well as provide a live multi-user testbed for the tools as I work on them. 

## Expanding Possibilities

As described above, my hope is that p5.anywhere will lower the barrier to entry for creating connected experiences of many kinds. I feel this is especially important now given the major online shift for work and learning during the last year. 

Further, these tools can also serve as a backend for other Processing Foundation projects. Imagine, for example, live-streamed teaching sessions in which the instructor can instantly push demo code to all of the student editors.

## Addressing Needs

This project is aimed primarily at an audience brand new to creative technology who are using p5 to take their first steps in that realm.

While there are now a huge range of tools and platforms to create and host a server backend with relative ease, none of them quite offer the intuitive simplicity provided by Processing and p5. My fundamental aim here would be to simplify basic network communication to the level of calling ellipse().
