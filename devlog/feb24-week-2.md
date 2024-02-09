---
layout: page
title: February Week 2
---

Feb 05 - Feb 09<br>
Week#: 06/52<br>

## Monday

Started work at 09:00 AM.

- 09:00AM - Working on issue #98. Will add moving feature - the main shortcut
- 09:43AM - Got on call with Ab to resolve a small code blocker.
- 12:00AM - The Split toggle is working but seems buggy. Investigating it. I also fixed Modular page.
- 02:00AM - issue #98 - Adding moving controls to the box.
- 04:00AM - Move Controls are working, the code isn't working as expected right now.
- 04:00AM - Joined college presentation meet
- 06:00AM - issue #98 - Found why Split toggle was buggy. Fixed, also move using m is almost working.
- 07:00AM - Stuck at rendering the component after moving it using the mouse.

## Tuesday

Started work at 08:30AM
- 08:30AM - I made the PR #195  with all the bugs.
- 11:00AM - Got on call with Ab, he was upset from my code. Will improve.
- 11:40AM - Switching from issue #98 to issue #72 because it took too much time.
- 01:30PM - Made the basic Modal Outline
- 03:30PM - The UI for the modal is done, I am confused about the Drawing page.
- 04:30PM - Got on meet with Ab to discuss further of issue #72 - adding the Drawing Page. I have a path now.
- 05:40PM - Meet eneded, got some light as to what I have to do.
- 07:00PM - I've fetched the prices for the woodworks, I'll start creating the table and the backend routes now.
- 10:30PM - 12:00AM - Tried making changes to the database.

## Wednesday

Starting work at 08:30AM

- 08:30AM - Ab commented some more context on the PR. We have a flow in mind, Goal is to get as much done today as possible.
- 09:15AM - Made the DB migration aka Table ( issue #72)
- 12:00AM - Made the basic Model, and functions to manage the table. Got on call with Ab to discuss further flow.
- 01:00AM - Started working on the flow.
- 03:00AM - Storing Ids from the modal in the database
- 05:00AM - The definitions are being stored in db, for the woodworks.
- 06:00AM - Prepared a layout of the `js/Drawings.js` to manage the state.
- 07:00AM - Pages are fetching the Drawings. Adding `getFigures` for each state of the woodworks module.


## Thursday

Started work at 8:45AM.

- 08:45AM - I was not able to understand the flow for getFigures. So starting with that.
- 11:00AM - Made some more changes to the DB, modified the table.
- 12:30PM - Added the getFigures() in the heirarchy tree.
- 02:00PM - Ab suggested a change in flow. I'm having trouble trying to wrap my mind on how to make the 2D renders. I am trying to mimic the render process but that isn't the right way.
- 05:30PM - I've extracted out the information from 'js/woodworks.js'.
- 06:30PM - Tried drawing on the canvas but faced an error.

Still working on issue #72

## Friday

Started work at 09:00AM

- 09:00AM - Got on call with Ab to get a basic rectangle on the screen.
- 12:00PM - I was able to generate a basic Figure from the data given.
- 01:30PM - Each woodwork was working, just the partititons were double lined.
- 03:30PM - Tried tweaking the partititons but no use.
- 04:30PM - The Figures show  up with labels and dimension lines.
- 05:00PM - I'll try to clean up some of the code.
- 06:30PM - Logging off. I tried some code cleanup as well as realised a bug in the dimensions. had to debug a lot but I think it works now.
