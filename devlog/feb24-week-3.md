---
layout: page
title: February Week 3
---

Feb 12 - Feb 16<br>
Week#: 07/52<br>

## Monday

Starting at 08:15AM

- 08:15AM - I wanted to get more of the work done regarding last weeks issue #72. Posted the goal for the day to Ab and started working on them.
- 10:00AM - Faced an issue with Overlapping dimension parameters. Should divide by section or partitions.
- 10:30AM - Added the Interal section of woodworks with labels for each section.
- 12:30PM - Blocker relating to weather to add woodwork using LayoutPlanner lib functions or not.
- 02:00PM - I added dimensions for partitions (discussion pending)
- 04:00PM - Worked and added exports column in the Projects table.
- 06:00PM - Had a short review and further discussion with Ab about the Feature. Got some changes to make the PR and define another function to work.
- 07:00PM - Made some changes in the backend. Currently refactoring getFigures -> getElements


## Tuesday

Starting Work at 08:00AM

- 08:00AM - Started working at refactoring the files and breaking down the functions into different functions.
- 10:00AM - Refactored file completely.
- 12:00PM - Wrote the functions for generating woodworkmap, I'll try generating some woodworks.
- 02:00PM - Had to attend college meet to present to the supervisor.
- 04:00PM - Problem while generating woodworkmap is they don't have rooms.
- 07:00PM - I'm having trouble adding rooms in the background. I'll try one more time then post it to Ab. I think i'm missing something minor right now.


## Wednesday

Starting work at 08:00AM

- 08:00AM - I'll aim at the issue with no floor plan when generating Woodwork Map.
- 09:30AM - Got on call with Ab to discuss the issue and get some clarity on how to proceed with the snapshots and pdf.
- 10:30AM - Got off call and started working on fixing the woodworks map issue to show floorplans too.
- 12:00PM - The issue itself is fixed and the images are being generated. Now I'll work on displaying the whole page as a static containing the faces of the various woodworks.
- 02:00PM - Woodworks are being generated in a PDF format, I'll try to make it look visually appealing as well as start storing the figures in the backend.
- 04:00PM - I have to store the woodworks map in the backend. Gave some thought and also struggling with the database.
- 04:30PM - Solved the db problem. Working on displaying the woodworks along with labels.
- 06:00PM - Now sending the woodwork snapshots to the backend and creating the drawing with woodworkmap too.
- 07:00PM - I'll try to wrap and push code.

## Thursday

Starting work at 08:00AM

- 08:00AM - I'll complete off the route and upload to blob storage of the woodwork map as well as the drawing.json file.
- 10:00AM - Got container details and started adding JSON and images to it.
- 12:00PM - JSON uploading is working itself, as well as image upload. Facing some issue while drying to JSONIFY the result from the blob URL.
- 12:40PM - Got on call with Ab to sort out the issue as well as make some suggested changes.
- 06:00PM - Didn't face any blockers. Coded out the Drawings.svelte, used it as a component. Shifted from POST + PUT request to POST only. And the blob storage connections are working.


## Friday

Starting work at 08:00AM

- 08:00AM - I'll try wrap the PR completely, and look at changes if any.
- 08:45AM - Faced an issue while trying to get Labels for each component on the Map. Discussed with Ab to rewrite the function or just modify it.
- 12:00PM - Fixed the label issues, and now both sides and Names are visible on the drawings page.
- 12:00PM - Got some PR changes by Ab, so I went and tried coding them. Spent some time tryingn to create an order when drawings are requested.
- 02:00PM - Added the code for creating the orders, was confused on retrieving the order-id.
- 04:00PM - Ab told that we don't get orderId :-> he asked to modify the table to remove order_id itself.
- 06:00PM - Pusehd the code by removing the unnecessary columns.