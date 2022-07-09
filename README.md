# Unreleased-level-Shambala-Waterworks

A level existed between Shambala Santuary and Palawan Lagoon: Shambala Waterworks. It was never included in the final game due to lack of time and technical problems. No one has seen this level since 1999 but many files have been forgotten in the game. (I'm sure it would be possible to make it work again if we had it, or recreate it if not ...)

-In this level the main goal was to open 4 portcullis doors using a system consisting of 4 channels and a water wheel. These doors led to the Ice Boss. But problem the water is frozen.

-The first step was to to melt an ice dam in the DivRoom 1 in order to supply water to the whole station. For that you had to find an Oil jar, break it on the ice dam and fire the oil with the Zippo.

-The water now flows through channels and can now be diverted to DivRooms 2 and 3 using the sluice in the DivRoom 1.

The next step was to complete 3 "Diversion rooms" also called "Div rooms" in any order you want, which must be opened with "Silver key", "Gold key" and "Garnet key". You had to divert the waterflow in any diversion rooms to start the associated mechanisms using some sluices gates. The level was filled with mills, sluices and various mechanisms. The goal of this whole operation was to open 4 gates leading to the Ice Boss.

Two areas of this level have been cut and integrated in other levels:
<pre>
- The Diversion room 2 (The flour mill): Now in Tian Shan River. (The river was smaller and you can see a walled-up entrance that is no longer used)
- The Ice boss arena: Now in Shambala Santuary. (Originally, the Shambala Santuary level ended after giving the flower to the old lady).
</pre>
![alt text](https://raw.githubusercontent.com/Jones3D-The-Infernal-Engine/Unreleased-level-Shambala-Waterworks/a0f42e3c93322f6730956c780250681ad63ffc3c/04_shw.jpg?raw=true)
<pre>
- Loading screen                - Still in game folder.
- Ice boss arena                - Dev SHW era <1999.
- Diversion room 2              - Dev SHW era <1999.
- Diversion room 1              - Dev SHW era <1999.
</pre>

# Third theoretical version of the layout

![alt text](https://raw.githubusercontent.com/Jones3D-The-Infernal-Engine/Unreleased-level-Shambala-Waterworks/main/shw_map_v3.jpg?raw=true)

# Level voices lines (not included in the released game)

In intro cutscene. (shw_opening.cog - var indyline)<br/>
"```SW01J01.WAV```"	"Brr.  Cold in here."

Voice line when action on a door in the "River area". (shw_rivervoice.cog - var inrivspot)<br/>
"```SW01J02.WAV```" "The stream is frozen solid. Ice won't spin too many waterwheels..."

Voice line when action on a door in the "River area". (shw_rivervoice.cog - var inrivhint)<br/>
"```SW01J02A.WAV```" "If I could melt the ice here, the river would flow again, I'll bet."

Not present in the official SHW COGS files. (Maybe in general voice cog or just never included???)<br/>
"```SW01J02B.WAV```" "I need something to heat this ice up and melt it."

Voice line when crossing a surface in "First area". (shw_powervoice.cog - var inwheelspot)<br/>
"```SW01J03.WAV```" "A waterwheel and four different sluiceways.  Why so many...?"

Voice line when crossing a surface in "Wheel cave" (shw_portroomvoice.cog - var intheyknew)<br/>
"```SW01J04.WAV```" "They certainly knew how to use water power here..."

Voice line when Indy have contact with a gate (var gatedev), probably a sluice. (shw_sluicevoice.cog - var inhmm)<br/>
"```SW01J05.WAV```" "It's a sluice-gate.  The monks must have used it to direct the water flow..."

Not present in the official SHW COGS files. (Maybe in general voice cog or just never included???)<br/>
"```SW01J06.WAV```" "Here's where the monks made flour for their daily bread..."

Voice line when crossing a surface in "Diversion room 2". (shw_div2voice.cog - var intheyknew)<br/>
"```SW01J06A.WAV```" "Quite a milling machine.  The first step in pounding out the monks' daily bread, no doubt."

Voice line when Indy take a "flask" but no inventory object index (bin) is defined. (shw_rivervoice.cog - var inflaskspot)<br/>
"```SW01J07.WAV```" "Some lamp oil...I might be able to warm things up with this."

# Specific items of the level
![alt text](https://raw.githubusercontent.com/Jones3D-The-Infernal-Engine/Unreleased-level-Shambala-Waterworks/740511db93f360b053127e7d61f7d92da7569be8/04_shw_items.jpg?raw=true)
<pre>
- shw_jar_oil.3do               - Oil jar : Melt the ice dam.
- shw_divkeyblue.3do            - Sapphire key : Open diversion room 1.
- shw_divkeygold.3do            - Gold key : Open diversion room 2.
- shw_divkeyred.3do             - Garnet key : Open diversion room 3.
</pre>

# Level scripts infos

***** NOW USED IN TIAN SHAN RIVER (02_riv) (Integrated Diversion room 2) *****
<pre>
- shw_hammer.cog                - Simple script used by each of the three hammers to control Indy's crush death.
- shw_Hammer_cam.cog            - Controls the hammer mill status in the diversion room 2, once used by monks to produce their flour. In the original level, the machine only worked if Indy directed the flow of water in that room. (Using a sluice system located in a room that no longer exists, probably "the main cave"). If the water is diverted away from the diversion room 2, the machine is stopped and reset to a standard position which prevents Indy from climbing to the upper floors.
</pre>
***** NOW USED IN SHAMBALA SANCTUARY (03_shs) (Integrated Ice boss arena) *****
<pre>
- shw_noledge.cog               - Prevents Indy from hanging onto the ledge before the ground (thing) collapses below him (And then, not to pass his hands through the ground). By default the surface is not "hangable", it becomes "hangable" 1 second after the fall of the ground (Thing).
- 04_shw_cinematic_3.cog        - Cutscene triggered when Indy open the door at the end of the level, the holy woman sends him to Palawan.
- shw_bosscinematic.cog         - Cutscenes triggered when Indy entered in the arena showing the ice boss and when killing him.
- shw_fogswitch.cog             - Change the fog when Indy crosses surfaces (4 for artivate and 4 for desactivate).
- shw_iceboss.cog               - Ai, movements and general actions of the ice boss.
- shw_imp1control.cog           - Small cutscene triggered when Indy pick up the Urgon part.
</pre>
***** NO LONGER USED IN THE RELEASED GAME *****

IN PROGRESS
<pre>
- shw_fallfx.cog                - Defines a still existing water sound (riv_h20_rapid_a.wav) for "ghost objects" and also defines a downward sector thrust. Probably a waterfall that is part of the "waterslide park" usable by Indy and mentioned by the level designer. The script receive orders (user0:) from variable "icedamcog", which was probably "shw_newriver_thaw.cog". The water flowing after the dam melts would therefore supply one or more waterfalls that can be used by Indy. (And then, maybe visitable early in the level without water, sound an thrust?)
</pre>
# End
