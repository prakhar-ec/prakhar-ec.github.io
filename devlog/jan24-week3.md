---
layout: page
title: January Week 3
---

Jan 15 - Jan 22<br>
Week#: 03/52<br>


## Monday
- Joined in at 9:00 and saww a new issue had been assigned to me. I went through some details of the issue to get an idea of it, then wanted to hold a meet with Ab to discuss it.
- I came up with an exhaustive list of possible combinations for shortcuts that were either mentioned or visible in the UI.
- The meet started at 10:20 AM, we discussed the combinations and discussed a bit about which library to use for this task.
- I started documenting the shortcuts we already had and the shortcuts that were still meant to be implemented.
- Now, I saw one issue that Shortcuts will have to be enabled selectively, that is, incase of search bar focus we want to disable the shortcuts that were running.
- My v1 of the shortcuts was creating a manager and then enabling or disabling them whenever neeced.
- We wanted to bind the shortcuts to certain elements but that was of no consequence since we can't do that. I spent some time actually studying about the even trigger and how they are propagated in the dom tree and how we can limit the shortcuts for a focus.
- I worked and tried binding the elements with Keyboardjs - a dead end. Then we got on a call at 6:26PM and discussed out the issue and a possible path.
- We had a discussion about merging shortcut manager into shortcuts and try working with that. keyboardjs also had a context option which we could explore.
- The review meet was postponed.


## Tuesday
- Already had the task in mind: shortcuts using contexts.
- Started at 9:00 AM  and coded everything we had planned and got on meet at 10:40AM, there we discussed the implementation I had and if it is feasible or not.
- I added all the shortcut features we initially came up with, focus on Searchbar, go through the Seach and choose one of them, gallery closes on escape etc.
- I was done adding these shortcuts at 3:30 PM itself, then we were discussing the possibility of moving the code to svelte components itself, this might be cleaner but shortcuts are required everywhere.
- Got on call at 6:44 PM to have a short code review and decide on what to do, I showcased the features added too. Got some little pointers to fix and that should wind up the v1 of the shortcuts.
- Still thinking if it's a good idea to use shortcuts groups or something else.
- Have the weekly review at 9:30 PM, let's see.


## Wednesday

- Clocked in at 9:00AM. I'm reviewing yesterdays work and then syncing up with Ab to get tasks for the day.
- Added the Reset text and changed the naming of Keyboard context according to the component names.
- We got on call at around 10:58 AM and started discussing the Agenda. WE also came up with a discrepancy with the commit history and resolved that.
- The call ended at 1:00 PM. There were a few code issues that are to be resolved(I'll mention them while solving), and maintain shortcuts for Woodworks panel.
- The target is to get done with this today itself.
- I changed the variable name to something better.
- First task was to remove Shortcut.js and just use keyboardjs directly. So that we don't have to consider managing etc.
- Then move all the code to functions and call them in App.js init func.
- I made all the changes except refactoring the suggestions class ( not a priority right now) Done till 2:30 PM.
- Now I'll focus on the woodworks modal and how to work with it.
- So I need to make a Shortcuts.js to initialise as well create the full mapping of the shortcuts.
- This should also map the bindings to functions( on select)
- The OnSelect is a dynamic function and has to be passed while initializing. This would make sure the onSelect is made when Modular init is called.
- We can get the canvas information using canvas maybe,
<!-- Modular js line 27  -->
- I've sat and written the classes for Shortcuts too. I wound up with the basic
- Have been going through the code a lot and Ab recognized the problem that I was speaking about, the shortcuts don't have to be dynamic but to trigger them we need some handler fuunction which are initiated later on in the program.
- Planning to maybe extend the functionality of the adapter class to support this operation or make a separate function.(7:30 PM)
- I went through the code again as Ab said to get the mouse offset and try and get the section.(10:00 PM), I'll try adding it and discuss tomorrow.


## Thursday

- Started off at 8:30 AM, I want to wind up the work as much as I can before the first call of the day.
- The idea is to get the box from canvas and work with that.