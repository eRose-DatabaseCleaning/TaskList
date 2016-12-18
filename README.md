<!---
Here is a link to know how to make this file nice and clean:
https://guides.github.com/features/mastering-markdown/

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

Some inspiration can also be found here: https://raw.githubusercontent.com/dev-osrose/osIROSE-new/master/README.md
-->

## Urgent task list
|   Category   |   Description  |  Assigned to  |
|     :---:    |     :---:      |     :---:     |
| Sources - Client & Server       | MaxHP and MaxMP should be a variable sent in the packet from and to the server     | Numenor    |
| Sources - Client     | HP fix - Computation is done from the Server side but also from Client side. We should make it match and make the server computation the priority      | Numenor      |
| Sources - Client     | Add better option to tp with the GM       | Laurenzzo & Hugo      |
| STB     | Bonefire (and summons in general) don't die when summoner is far away -->this has to be fixed in the AIP files. For example it works well with the Ruff AIP files. Should we put all AIP files from Ruff there then?       | Laurenzzo      |




##Complete list of tasks
### Sources (newest to oldest)
- [ ] Add more slots in inventory
- [ ] Change max number of party member (temporary fix and then clan fix?)
- [ ] Add GM command to change party level
- [ ] Reduce zone where to click to enable the chat
- [ ] Name change if a jewel is equipped? + bug "runit_in < num_runits" [zz_visible.cpp#1877]
- [x] Get more time to drop (multiplied by 5)
- [ ] Enable moving a char with keyboard (but only the active window and while not in the chat)
- [ ] Change drop formula to be more intuitive (see work of Laurenzzo)
- [ ] Add more info and option when you Ctrl+RClick on a ally char.
- [ ] Change the right-click on ally to a Ctrl+right click to see some info.
- [ ] Make the blue items just a stat like the refine stat. For the drops, add a new column inside the STB to say if this monster can drop blue items or not. ---> Next step is the craft of such item (new skill like refine)
- [ ] Add an option to choose for constant or not rendering
- [ ] Atfer implementation of auto-login add automatic option to launch several game with password and automatically open the windows with the right size to be splitted on the screen
- [ ] Implement auto-login
- [ ] Prevent windows to be opened out of the screen when resolution changes
- [ ] Fix the 2nd skill bar (numbers for bar one, and F keys for 2nd bar)
- [x] Make the limitation on the FPS working! (but a bit dirty, have to find where the value of 1000 for get_rs()->min_framerate is coming...)
- [ ] If right-click in the skill bar, open more details about the skill
- [ ] Add the possibility to navigate inside menus with number (1 = option 1 etc)
- [ ] Add better option to tp with the GM
- [x] Add new GM commandes for apparaisal items
- [x] Improve debug rendering (Alt+d in GM mode)
- [x] Change shortcut to switch 'visible name of drops' with only Atl+Gr (switch on AND off) + enable this option by default
- [ ] When crafting, the overview of the item should show basic stats
- [x] When using apparaisal, it should continue until we right-click to cancel it
- [x] Right-click unselect target, even if hold: this has to be fixed
- [ ] HP fix
- [ ] MaxHP and MaxMP in packets
- [x] Always drop no matter the level difference with the monster
- [x] Drops should NOT always drop socket items
- [x] Party buff also focus summons
- [ ] The game is sometimes super slow (semi-fixed with the FPS fix. Have to continue to investigate)

### STB (newest to oldest)
- [x] Add more sexy HP gauge bar
- [x] Fix quest with engagement ring that you cannot complete after lvl 22
- [x] Add spero's wooden chest and associated quest (we decided not to add it :-) )
- [ ] Remove unwanted messages (like the "promotion sale for the warehouse" or the messahe after the tutorial saying you just learned two skills... that you already have)
- [ ] Bonefire (and summons in general) don't die when summoner is far away -->this has to be fixed in the AIP files
- [ ] When a npc speaks in the chat, the name is wrong (it takes the second column of the STB files)
