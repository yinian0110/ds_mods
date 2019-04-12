This MOD is modified by the DST version of Too Many Items (author: Skull) and is open source following the original MOD using the [GPL3 protocol](<https://www.gnu.org/licenses/gpl-3.0.html>).

Too Many Items series MOD is a great MOD series, which provides great convenience for players who need to test and demonstrate. But [Too Many Items for DS](<https://steamcommunity.com/sharedfiles/filedetails/?Id=579513934>) have much fewer useful functions than [Too Many Items for DST](<https://steamcommunity.com/sharedfiles/filedetails/?Id=551338671>). To this end, I transplanted the DST version of Too Many Items to the DS version, re-implemented some of its functions and added some new features that might be useful in DS.



My main changes:

- Porting UI interface to DS (actually, this is a little change, mainly the compatibility between DST and DS)
- Removed the inapplicable functions of DS, re-implemented some functions, and added some new features for DS.
- Re-establish the complete list of items and map target list for DS
- It supplements the way to spawn items  that can not be spawned directly by commands such as SpawnPrefab. Several examples:

  - poison birchnut tree: share the same code with birchnut tree (deciduoustree).

  - buzzard:  can be spawned directly, but without special treatment, the game crashes when it flies away

  - Chester (Shadow Chester, Ice Chester), Packim (Fat Packim, Fire Packim), ROBIN
- Adding icons to the list of living and building items. The game provides only the icon for inventory items and some special items. That is, it doesn't provide icon for most living and building items, only provide their animation. To get a icon, one need to extract it from the animation file. Some of the images I added were downloaded from [Don't Starve Wiki](<https://dontstarve.fandom.com/wiki/Don%27t_Starve_Wiki>), others were extracted by myself. This is also the reason why the MOD file is so much larger than the original MOD.



ATTENTION:

- Some items on the list of livings and buildings will cause crash when they are created in a world that does not belong to them, such as antqueen in a world other than Hamlet. I've removed some of the items that could cause crash in different worlds, but there may be omissions, and more importantly, I tested them under the [latest Hamlet beta](<https://steamcommunity.com/games/219740/announcements/detail/1727601346322579127>), which allowing hamlet's pighouse be built outside hamlet. Considering these characteristics will be add to the official version in the future, I do no special adjustments for the official edition..

- The current state of the MOD is testing. Some things have not been tested rigorously (I can't do a lot of tests by myself, I need to consider whether the DLCs are enabled and which world you are current in). They may cause crash and lead to some magical mistakes. Feedback is welcome if something goes wrong, and please don't use it in your own official archives.

- Even if all kinds of BUGs have been removed, it is strongly not recommended to use them in official games, which will greatly reduce the fun of the game.

- In the list of items,  there is the code of the item under the name of the item. If there is a plus sign ("+") in the code, it means that this MOD has a special treatment for it.




Future plans:

- Solve all kinds of crash problems

- Allow players to move items from the "other" category into the official category

- Provide interfaces for other MODs to adjust the categories and functions of items in this MOD









# Main panel

In terms of the function of generating items, there are many categories of items:

- Special: Collections

- All: Includes foods, resources, weapons, tools, clothing, gifts

- Food, Resources, Weapons, Tools, Clothing, Gifts: item would enter your inventory when generated

- Livings, Building: item would be generated near player.

- Others: Items that do not appear in the above categories (such as new ones in later versions) and MOD items will appear here, but contain a lot of items that may cause crash.



The way in which items are generated:

- Click to generate an item. (You can change it in the options)

- Right-click to generate 10 items. (You can change it in the options)

- SHIFT + click or right-click to get and produce quantities of material.

- CTRL + Click to add or remove custom items list (collection).



Search:

- Enter key or click anywhere: search for input.
- UP key: Last input.
- DOWN key: Next input or empty input.
- ESC key: exit input.



In addition, there are also some small functions, such as(the effect of holding down CTRL and clicking for the same button are in parentheses) setting health to full (to 10%), setting sanity to  full (to 0), setting hunger to full (to 0), setting temperature to 25 degrees (to environmental temperature), setting moisture to 0 (to 100), setting log value to full (to 0), emptying backpack (emptying backpack and inventory), Detoxification (Poisoning), Game pause/Continuation, God Mode, Creation Mode, One-Hit Kill Mode



# Debugging panel

- Season:

  - Vanilla: Summer and Winter

  - ROG: Spring, Summer, Autumn, Winter

  - shipwrecked: Mild, Wet, Green, Dry

  - Hamlet: Temperate, Humid, Lush, Aporkalypse

- Time: Next stage, 1 day later, 5 days later, 10 days later, 20 days later

- Speed: 0.6 times speed, normal speed, 2 times speed, 3 times speed

- Weather: Lightning, starting/stopping rain and snow, starting/stopping volcanic eruptions (shipwreck), starting/stopping hurricanes (shipwreck), starting/stopping fog (Hamlet, humid season)

- Players: unlock all technology (not creation mode), unlock all characters, change character and continue playing, empty morgue

- Entities: Delete, fertilize, ripen, harvest, pick, freeze

- Beefalo: fight, ride, pet, normal

- Followers: add, expel, health, hunger, loyal

- Game: rollback, save, entering the next world, resetting the world ID to 1 (normally the ID will add 1 after entering the next world), going to the world of survival, shipwreck, Hamlet

- Teleport: Record the current location, transfer to the recorded location

- Map: Full map (temporary, lost after reloading the game), Full map (permanent), empty map, display all the rooms in the current ruins (HAMLET) on the map, teleport to certain designated locations (different lists in different worlds). Teleport to locations has been optimized specifically:
  - If the player is on land but the target is on water, a lograft will be built and aboard before teleport (or you'll drown right away.).

  - If the player is on water but the target is on land, the ship will be parked in place before teleport (otherwise the ship will be destroyed directly).

  - In Hamlet, the problem of geting stuck when teleport directly across rooms is avoided.


