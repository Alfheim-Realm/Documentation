# Alfheim Realm

## Description:
* 

## Main Features:
* [Server Rates](#server-rates)
* [Server Limits](#server-limits)
* [Server Maps](#server-maps)
## Changed Features:
* [Fairy System](#fairy-system)
* [Experience System](#experience-system)
* [Damage Handler](#damage-handler)
* [Amplifier System](#amplifier-system)
* [Forging System](#forging-system)
### Server Rates:
* Solo EXP: 
* Party EXP: 
* Fairy EXP: 
* Ship EXP: 
* Drop Rate: 
### Server Limits:
* Player Level: 65
* Fairy Level: 41
* Equipment Socket: 2
### Server Maps:
* Ascaron (+ Region)
* Magic Sea (+ Region)
* Deep Blue (+ Region)
* Forsaken City (1, 2 & 3)
* Dark Swamp (1, 2 & 3)
* Demonic World (1 & 2)
* [Chaos Argent](#chaos-argent)

#### Fairy System:
* Everything is customizable via variables.
* Rations considered "auto" do not need to be in third slot, system will auto detect that fairy is not full and will check if player has an auto ration and will consume it. If it needs more than one ration, it will consume till full.
* Players will need to put skills in order from novice to standard, cannot place standard directly.
* All related texts are now tied to variable for easy modification.
* Configurable maximum level for each kind of fruit (normal and great) with an overall maximum level that cannot be surpassed.
* Fairies do not need to be "married" in order to be considered second generation, automatically all fairies that could be obtained from marriage can use possession skill.
* New fairies (Angela and Angela Jr) are usable, along with new improved fruits and rations.
#### Experience System
* Able to customize all rates from just variables: solo, party and boat experience.
* Removed experience from maps without needing items within inventory.
* Increase rates on a per day basis.
* Able to adjust rates on a per level basis to decrease experience obtained the closer the player is to the level limit. Adjusts automatically when increasing level limit.
#### Amplifier System:
* Everything is customizable via variables.
* Can add new amplifiers with a single variable and ItemInfo line.
* Won't allow players to use an amplifier if they already have used one with the same or better bonus.
* Able to adjust each percentage of super and lucky strike for each level bonus.
#### Damage Handler
* Function "after_player_kill_player" has been updated to be customizable.
  * Able to customizable kill feed texts.
  * Able to make kill feed text local or global notices on a per-map basis.
#### Forging System:
* Allow to put level limits on a general level, type (unique, dragon, basic) and individual gems.
* Allow to set the specific success rate percentage for each level on each type: forging gems, combining gems and combining refining gems.
* Allow to modify the success rate for each socket percentage.
* Allow to move gems from one slot to another when empty.
  * If a socket goes emtpy upon gem extraction, the gem in the next socket can be moved down. Example: if socket 1 goes empty upon last gem extraction, gems from socket 2 can be moved to 1 and gems from socket 3 moved to 2.
* Prohibit forging same attribute type gem in a single equipment.
  * Example: cannot forge "Chipped Gem of Rage" if equipment already has "Gem of Rage".
* Set a maximum forge level on equipment.
* Blacksmith's plier are customizable.
  * Can obtain "Refining Gem" upon extraction of gem.
  * Can empty the equipment socket and get all gems in it.
  * Combination of the 2 above.
* All of the above can be customized via variables.
* Several gems are available for usage within the files: normal, unique, dragon, advance, hat, broken, cracked, chipped, great and azrael gems.
#### Chaos Argent:
* The whole map script was cleaned, modified and improved to easier usage and modification with only variables.
* The essence of the map stayed the same, but a lot of improvements were made on the map to increase player engagement.
* New functions were added to handle cheaters like players forming party inside, anti-relog penalties, multi-account prevention and so on.
* Added new ways to obtain honor/chaos points upon getting kill-streaks, revenge and internal ranking kills.
#### Extra Stuff:
* Fixed backend stuff.
  * Easier ways to manage "Medal of Honor".
  * Grouped all healing items into a single function with customizable variables.
  * Cleaned and fixed all manufacturing items.
  * Cleaned all character and monster skills.
* Added effect/state handler to allow easier modification of glows or state bonuses.
* Quest System:
  * Added functions to easier create daily and weekly quests by just adding 2 extra variables to the desired quest.
  * Modified some core functions to allow for quests to be timed just by adding the desired time in seconds to the quest.