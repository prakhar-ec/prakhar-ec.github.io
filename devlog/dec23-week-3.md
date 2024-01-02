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


## Friday

- Started the day with the aim to figure out the reason behind the mysql container data not being persistent.
- Tried to narrow down where the issue was starting exactly.
- I thought because I didn't use the `ecstop` command this was happening, this wasn't the case.
- Then I tried multiple combinations of stopping, starting, restarting the containers and restarting the docker daemon. 
- Figured out the docker daemon restart was causing the issue.
- Now, I was using a pre-installed ubuntu i.e I've been using it for 2 years so naturally it had some extra services running. Decided do perform a fresh installation.
- Did a fresh installation of Ubuntu and created two user - this took 3 hours which included downloading, backing up the data and preparing the laptop as well as the installation.
- Went up with the full setup and the issue was still there.
- Then went to proper googling and stack overflow. Found some questions and answer that had the same case but their solutions didn't work for my system. I thought this was system specific. 
- Tried using an external storage i.e using something in my home directory. It worked. The data was persistant meaning there was something with the directory itself.
- Went through inspection of containers and found the volumes were being mounted no problem there.
- Tried to navigate to the path specified in the mounts. Path not found error.
- I think maybe docker was trying to find that folder in the host machine to store the sql data, and the folder not being there was causing the issue. Created folder `data/myql` and Voila! it worked.
- Will need to commit the `data/mysql` folder as empty. It is needed for every new repo pull.
- Tried changing the .gitignore for this, tried various combinations of `data/*` and `!data/mysql/`.
- None seemed to work. The problem is git doesn't recognise a empty folder as modification as such. Tried a workaround. Added an emtpy `data/empty` folder with .gitkeep as the sole file. Then pushed and added `data` to .gitignore. Worked!
- Now anyone who clones the repo will have a empty `data/mysql` folder with just one .gitkeep file.
- Added comments in the file to make sure the purpose is clear and isn't modified.


