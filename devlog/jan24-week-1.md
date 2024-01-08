---
layout: page
title: January Week 1
---

Dec 01 - Jan 07<br>
Week#: 01/52<br>

## Monday

- Had the Orientation meet at 12 PM and that's it for todays day, office begins tomorrow.
- Read a book to get myself to increase my attention span. 

## Tuesday


### What have I done since the last log?
- Started off at 9:00 AM sharp. Began with importing the SQL dumb.
- Ab had Sent the 3rd SQL dumb for materials. Loading the tables worked, the items are now available in 3D.
- Trying to evaluate the cause of the `TypeError: can't convert undefined to object` when trying to use the TV Set for 3D rendering.
- I tried tracing back the issue from the back the error actually arrives from TV set being returned as undefined.
- Ab asked to create a flowchart for the working of Furniture loading - added as much info as I could in it.
- Made some corrections as suggested and improved readability. 
- Sat on a meet with Ab to find the issue. I need to bring in more efficiency. Was relying on console.logs more than browser debugging. Was able to trace back the issue to the json file itself.
- Fixed the issue and the rendering works. For now the console is free from errors.
- Started working on documentation to prepare a documentation of the tables of the database that are being used.


### Any problems or Blockers?
- Trying to understand the tables as a whole and prepare relationship between each other.

### What's next for tomorrow?
- Will try and complete the mapping of atleast one table today and get approved. Then move on to prepare the rest of them.
- Complete a full testing of the frontend in another thread to make sure there aren't any other render issues.


## Wednesday


### What have I done since the last log?
- Started off at 9:00AM and had already finished the iteration 1 of direct mapping of tables.
- Shared with Ab and got some reviews.
- I had a issue assigned to me, took a good look at it and tried to understand the main goals.
- Broke off the issue into several parts and was in constant to and fro with Ab to keep the communication channel clear.
- I added the Search bar first using sveltestrap but the autofocus kept on going berserk. Was about to shift to normal <input> but then used vanilla javascript with a little delay to autofocus on tab change.
- Experimented with `Fuse.js` and went through the documentation to understand it's working and what is required to get the basic feature up and running.
- Started looking into the `Materials.js` trying to find the complete array of objects to use in Fuse.js.
- The aim was to complete the task EOD but wanted to include the code in a more optimal way. Decided to add to the Repo class itself.



### Any problems or Blockers?
- Deciding to add to Repo class or include in the component itself. 

### What's next for tomorrow?
- Will complete the current issue as fast as I can and create the PR.
- Add notes for optimization if I can think of any.


## Thursday


### What have I done since the last log?
- Started of at 9:00AM and started working on yesterday's issue.
- Included the Search in the Repo class itself and hooked it up with the search bar.
- The search bar wasn't exactly smooth, since it was searching for every character change.
- I looked for a way to throttle the input so that the search trigger would wait for a second before actually searching for the key.
- The working did get smoother with the trigger.
- Made the PR along with few comments here and there.
- Got assigned another issue today.
- Similar to the last one, this time the search bar has to be implemented with the 2D layout.
- Started off by adding the Search bar.
- Few complications arised, what should trigger what. How does the sub-category function. Should I open the gallery for all?
- Talked to Ab about it trying to decide what to do. Had to postpone the issue for the next day.


### Any problems or Blockers?
- Deciding when the Gallery should open, accordtion or menu should open.

### What's next for tomorrow?
- Decide on the action according to what is typed in the Search bar itself.
- Make the PR for the issue. 


## Friday


### What have I done since the last log?
- So we went a little back and forth. One problem is we want the ID to match exactly and the type and category to be implemented a little fuzzy.
- Trying to decide weather we should use three indexes or two indexes.
- Ab came up with the plan to separate id search and type/category search - so two indexes.
- Implemented the indexes and it seems to work for now.
- Trying to add the preview for a direct Id match so that the user can add it directly.
- Communicating with Ab trying to decide on the final working.


### Any problems or Blockers?
- Couldn't open the PR, added a delay because gallery and direct match are confusing.

### What's next for tomorrow?
- Weekend. Will try to complete the issue and make a PR on Monday itself.


## Week Retrospective


### How did the Week Go?
- The Week went good, the work load was balanced for now. I took some time trying to understand the bigger picture of the code repository.
- Slowly understanding the working of the files with each other and how they are connected. Worked on two issues and gaining some idea on Svelte itself.
- I went slow on the communication channel initially, to keep the work going I need to communicate more and be clear about what I am doing. Even slight doubts or misconceptions can cause large delays.


### What could've been better?
- I think the pace for the first week was good. 

### What's in for the next week?
- Increase the Pace of work I do.
- Communicate better with more efficiency.
- Close off the last weeks issues.
