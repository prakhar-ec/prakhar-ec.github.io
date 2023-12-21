---
layout: page
title: December Week 3
---

Dec 19 - Dec 23<br>
Week#: 51/52<br>


## Monday

- Did basic Work Log setup and other system settings.

- Got the Github SSH Keys added for authentication.

<br />


## Tuesday

- Started off with a short call with Ab to setup the docs and run basic configurations.
- Got a note of what would be the major task and how I might go around doing it.
- Tried setting up the dev environment on my own while following the docs.
- Ran into some permission issues in docker and had to use `chown`.
- The day passed by trying to get the containers work which kept failing.

<br />

## Wednesday

- Picked up where I left yesterday. Had to make the containers work somehow.
- Was consulting Ab parallely while working trying to get things done.
- Did a deep dive into Volumes and Mounts and how they work, difference between volume and binds what to use when.
- Finally made the containers work.
- Turns out I had to grant folder permission from docker desktop too.
- Used SQL commands to create the tables and fill them up provided by Ab.
- The website lets me create a new project but having error while adding components. Will start debugging now.
- Parallely added a Getting-Started.md page to setup the containers and get them working. 

<br />

## Thursday

- Started debugging why I can't see anything in the grid.
- Adding a component might now show in 2D but is visible when viewing in 3D.
- Some components are obviously missing hence few of the console errors.
- Can use arrow keys to move components but still haven't figured out a way to zoom-in/out.
- Switching from 3D to 2D shows the components for a brief moment.
- The element becomes null and thus it doesn't get filled.
- The issue was the url being passed to fabric. It got converted to `http` thus throwing the error.
- Went through all the files to try and trace back the issue. Turns out fabric was setting in the `http` on it's own. 
- I could either append `https` at the start of relative urls or hardcode the initial url. 
- Choosing the later was a better option and went for it(Ab adviced).
------


