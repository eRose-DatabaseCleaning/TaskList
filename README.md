<!---
Here is a link to know how to make this file nice and clean:
https://guides.github.com/features/mastering-markdown/

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

Some inspiration can also be found here: https://raw.githubusercontent.com/dev-osrose/osIROSE-new/master/README.md
-->

<!---
## Urgent task list
|   Category   |   Description  |  Assigned to  |
|     :---:    |     :---:      |     :---:     |
| Sources - Client & Server       | MaxHP and MaxMP should be a variable sent in the packet from and to the server     | Numenor    |
| Sources - Client     | HP fix - Computation is done from the Server side but also from Client side. We should make it match and make the server computation the priority      | Numenor      |
| STB     | Bonefire (and summons in general) don't die when summoner is far away ->this has to be fixed in the AIP files. For example it works well with the Ruff AIP files. Should we put all AIP files from Ruff there then?       | Laurenzzo      |
-->




##Complete list of tasks
### Sources (newest to oldest)
- [x] Windows are not resizable anymore by dragging the mouse at the edge of the window
- [x] Add a launcher option with width and height; automatically put the windows in the right position if one change the resolution from the launcher and not from the options menu; if change resolution from launcher, update the option dialog accordingly (and so come back to this after full screen); if same res than in the .ini file, don't change position of windows. If different, please reset the position of the windows. Correct default position of 2nd skill bar.
- [ ] Add options to: constantly render or not the screen; change between 30 and 60FPS
- [x] Give same cosmetic for basic skill and normal skill
- [x] Add correct condition to basic skill + add new case in the "check skill conditation": if we have a bagpack or wings
- [x] Lvl 35 cleric passive skill implemented: double skill duration
- [x] New skill to drop at distance for 1000 stamina
- [ ] One should also recover MP (like it is done for HP) all the time, not only when using "sit"
- [x] Add success rate when crafting (with update to show 100% if we have a success rate >=100%)
- [ ] Add clan skill for: party level (bonus part) +6 production part + clan house
- [ ] Add special lvl 35 skill: Arti==blue craft; Bourg==Party stockpiling ; Cleric==buff duration; Mage==summons don't loose health; Raider==Recover HP/MP when dodge (skill active only each XX seconds); Scout==bonus zuly (also for party); Knight==more focus by agro (especially when fighting someone). For example a auto-taunt every 10s you fight; Champ==if you don't have one piece of equipment it gives you a bonus/malus in def/atk (more atk, less def ^^)
- [x] Add option to the launcher to set the initial position of the window
- [x] Remove the camera that starts turning when mouse reaches the edge
- [ ] Add a skill to tp to the clan house and a warp in the clan house to any zone (but have to unlock it first with specific quest for each zone (hard to get: money plus lot of power!)
- [ ] continue action after some skills (ex: healing) -- search for keyword "CMD_STOP" in visual studio
- [ ] Make two chats: one big, one small that separates log and talks... This is maybe what is doing frarose (https://github.com/eRose-DatabaseCleaning/Sources-non-evo/blob/be45f82f8ef288602db7cb09e532170b7b2b504c/Client/Interface/it_mgr.cpp#L1186). You can find the chatbox here: https://github.com/eRose-DatabaseCleaning/Sources-non-evo/blob/be45f82f8ef288602db7cb09e532170b7b2b504c/Client/Interface/CChatBox.cpp
- [x] Add a new shortcut to sit (Alt+Z)
- [ ] When you look at a new equipment it shows what you have equiped at the moment to compare
- [x] Add the last step to autologin: the char selection (then next step is the multiple launch, ask Laurenzzo :-) )~~
- [ ] ~~To complicated for nothing, project aborded for the moment. Exit button on the char select view should send you to the account login page~~
- [ ] When you click on a summon, don't run towards it (have to add a category to: OBJ_MOB, OBJ_NPC etc for summon. Then have to change the cursor (to be the same than when you select an avatar (search for CURSOR, here: https://github.com/eRose-DatabaseCleaning/Sources-non-evo/blob/e56f146001a86aeaa2b1d20158b45da2b55eefc6/Client/System/CGameStateMain.cpp#L1212) and then change it here : SetTargetObject_Normal in JCommandState.cpp: https://github.com/eRose-DatabaseCleaning/Sources-non-evo/blob/master/Client/JCommandState.cpp#L956). An interesting function to be able to see hp of all char and to get inspiration: https://github.com/eRose-DatabaseCleaning/Sources-non-evo/blob/master/Client/JCommandState.cpp#L1049 
- [ ] Add more slots in inventory
- [ ] Change max number of party member (a clan skill?): see here: https://github.com/eRose-DatabaseCleaning/Sources-non-evo/search?utf8=%E2%9C%93&q=MAX_PARTY_MEMBERS with the line we want here: https://github.com/eRose-DatabaseCleaning/Sources-non-evo/blob/be45f82f8ef288602db7cb09e532170b7b2b504c/Server/SHO_GS/SHO_GS_LIB/GS_PARTY.CPP#L609 
- [x] Temporary fix to update party level by 2 (6 player at lvl 1, 7 at lvl >=5)... This needs to be improved, see point above!
- [x] Add GM command to change party level
- [ ] Reduce zone where to click to enable the chat
- [ ] Name change if a jewel is equipped? + bug "runit_in < num_runits" [zz_visible.cpp#1877]
- [x] Get more time to drop (multiplied by 5)
- [ ] Enable moving a char with keyboard (but only the active window and while not in the chat)
- [ ] Change drop formula to be more intuitive (see work of Laurenzzo)
- [ ] Add more info and option when you Ctrl+RClick on a ally char.
- [x] Change the right-click on ally to a Ctrl+right click to see some info.
- [ ] Make the blue items just a stat like the refine stat. For the drops, add a new column inside the STB to say if this monster can drop blue items or not. ---> Next step is the craft of such item (new skill like refine)
- [ ] Add an option to choose for constant or not rendering
- [ ] Atfer implementation of auto-login add automatic option to launch several game with password and automatically open the windows with the right size to be splitted on the screen
- [x] Implement auto-login (Login step:OK; Server step:OK; Char step: new task above)
- [x] Prevent windows to be opened out of the screen when resolution changes
- [x] New shortcut for skill bars "1 2 3..." for normal bar and F1 F2 etc for second bar. If in a dialog, then use Alt+1 2 3 instead (F1 F2 etc will always work). To switch bar: Ctrl+1 2 3 4 for the normal bar, and F9 F10 F11 F12 for the other one.
- [x] Fix the memory for skill bars. For the moment, only page 1 of bar 1 is saved ! The rest is not and you have to put your skill by hand all the time...
- [x] Not correct skins for skill bar (number doesn't show current page of the bar, shortcut are not correctly pictured) (see xml files and create and setID !)
- [x] Make the limitation on the FPS working! (but a bit dirty, have to find where the value of 1000 for get_rs()->min_framerate is coming...)
- [x] If right-click in the skill bar, open more details about the skill
- [x] Add the possibility to navigate inside menus with number (1 = option 1 etc) and therefore remove skill action when in dialog
- [x] Add better option to tp with the GM
- [x] Add new GM commandes for apparaisal items
- [x] Improve debug rendering (Alt+d in GM mode)
- [x] Change shortcut to switch 'visible name of drops' with only Atl+Gr (switch on AND off) + enable this option by default
- [x] When crafting, the overview of the item should show basic stats
- [x] When using apparaisal, it should continue until we right-click to cancel it
- [x] Right-click unselect target, even if hold: this has to be fixed
- [ ] HP fix
- [ ] MaxHP and MaxMP in packets
- [x] Always drop no matter the level difference with the monster
- [x] Drops should NOT always drop socket items
- [x] Party buff also focus summons
- [ ] The game is sometimes super slow (semi-fixed with the FPS fix. Have to continue to investigate)
- [x] Force constant rendering + various shortcut bug fixes
- [x] Remove isTaiwan and fix calculation to be a iRose like server

### STB (newest to oldest)
- [ ] Implement new quests for special skill at lvl 40
- [ ] About the level 30 job quest: Soldier==very long (have to kill aquas for hours with first hit). It's nice won't change it;Muse==easy and super nice reward!; Dealer==have to be smart but easy, let it that way; Hawker==impossible for the 2 first level. Need help for the last one. Have to change it, like 2 captains in 10 minutes. Or better-->do a speed challenge NOT depending on the spawn rate. --->So for this part, redo the quest for hawker.
- [x] Fix 5-color-scales (you need 10, not 5!) in episode quest
- [ ] Fix zombie quest (episode quest)
- [ ] Fix the bridge in El Verloon above the turtles so we don't get stuck on it.
- [ ] Description of "gathering (stock piling?) in dealer skills is wrong-->to check and fix!
- [x] Add more sexy HP gauge bar
- [x] Fix quest with engagement ring that you cannot complete after lvl 22
- [x] Add spero's wooden chest and associated quest (we decided not to add it :-) )
- [ ] Remove unwanted messages (like the "promotion sale for the warehouse" or the messahe after the tutorial saying you just learned two skills... that you already have)
- [ ] Bonefire (and summons in general) don't die when summoner is far away -->this has to be fixed in the AIP files
- [ ] When a npc speaks in the chat, the name is wrong (it takes the second column of the STB files)
