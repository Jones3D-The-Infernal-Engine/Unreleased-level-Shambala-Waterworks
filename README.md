# Unreleased-level-Shambala-Waterworks

A level was planned between Shambala Santuary and Palawan Lagoon: Shambala Waterworks. It was never included in the final game due to lack of time and technical problems. No one has seen this level since 1999 but many files have been forgotten in the game. (I'm sure it would be possible to make it work again if we had it, or recreate it if not ...)

In this level, the first step was to find to melt an ice dam in order to supply water to the whole station. For that you had to find an Oil jar, break it on the ice dam and fire the lacquer with the Zippo.
So you knew how to access the main cave. The next step was to complete three "Div rooms" in any order you want, which must be opened with "Silver key", "Gold key" and "Garnet key". You had to divert the waterflow in any diversion rooms to start the associated mechanisms. The level was filled with mills, sluices and various mechanisms. The goal of this whole operation was to free four gates leading to the Ice Boss.

Two areas of this level have been cut and deported in other levels:

- The Div Room 2 (The flour mill): now in Tian Shan River. (You can see a walled-up entrance that is no longer useful)
- The Ice Boss Arena: now in Shambala Santuary. (Originally, the Shambala Santuary level ended after giving the flower to the old lady).

![alt text](https://raw.githubusercontent.com/Jones3D-The-Infernal-Engine/Unreleased-level-Shambala-Waterworks/main/04_shw.jpg?raw=true)

# Level voices lines (not included in the released game)

```diff

```

In intro cutscene. (shw_opening.cog - var indyline)
```diff-"SW01J01.WAV"```	0	"Brr.  Cold in here."

Voice line when action on a door in the "First area". (shw_rivervoice.cog - var inrivspot)
"SW01J02.WAV"	0	"The stream is frozen solid. Ice won't spin too many waterwheels..."

Voice line when action on a door. (shw_rivervoice.cog - var inrivhint)
"SW01J02A.WAV"	0	"If I could melt the ice here, the river would flow again, I'll bet."

Not present in the official SHW COGS files. (Maybe in general voice cog or just never inclued???)
"SW01J02B.WAV"	0	"I need something to heat this ice up and melt it."

Voice line when crossing a surface in "First area". (shw_powervoice.cog - var inwheelspot)
"SW01J03.WAV"	0	"A waterwheel and four different sluiceways.  Why so many...?"

Voice line when crossing a surface in "Wheel cave" (shw_portroomvoice.cog - var intheyknew)
"SW01J04.WAV"	0	"They certainly knew how to use water power here..."

Voice line when Indy have contact with a gate (var gatedev), probably a sluice. (shw_sluicevoice.cog - var inhmm)
"SW01J05.WAV"	0	"It's a sluice-gate.  The monks must have used it to direct the water flow..."

Not present in the official SHW COGS files. (Maybe in general voice cog or just never inclued???)
"SW01J06.WAV"	0	"Here's where the monks made flour for their daily bread..."

Voice line when crossing a surface in "DivRoom 2". (shw_div2voice.cog - var intheyknew)
"SW01J06A.WAV"	0	"Quite a milling machine.  The first step in pounding out the monks' daily bread, no doubt."

Voice line when Indy take a "flask" but there isn't but there is no inventory object index. (shw_rivervoice.cog - var inflaskspot)
"SW01J07.WAV"	0	"Some lamp oil...I might be able to warm things up with this."

# Level scripts infos

***** DEPORTED AND NOW USED IN TIAN SHAN RIVER (02_riv) (Diversion room 2) *****

- shw_hammer.cog                - Simple script used by each of the three hammers to control Indy's crush death.
- shw_Hammer_cam.cog            - Controls the hammer mill status in the diversion room 2, once used by monks to produce their flour. In the original level, the machine only worked if Indy directed the flow of water in that room. (Using a sluice system located in a room that no longer exists, probably "the main cave"). If the water is diverted away from the diversion room 2, the machine is stopped and reset to a standard position which prevents Indy from climbing to the upper floors.

***** DEPORTED AND NOW USED IN SHAMBALA SANCTUARY (03_shs) (Ice boss arena) *****

- shw_noledge.cog               - Prevents Indy from hanging onto the ledge before the ground (thing) collapses below him (And then, not to pass his hands through the ground). By default the surface is not "hangable", it becomes "hangable" 1 second after the fall of the ground (Thing).
- 04_shw_cinematic_3.cog        - Cutscene triggered when Indy open the door at the end of the level, the holy woman sends him to Palawan.
- shw_bosscinematic.cog         - Cutscenes triggered when Indy entered in the arena showing the ice boss and when killing him.
- shw_fogswitch.cog             - Change the fog when Indy crosses surfaces (4 for artivate and 4 for desactivate).
- shw_iceboss.cog               - Ai, movements and general actions of the ice boss.
- shw_imp1control.cog           - Small cutscene triggered when Indy pick up the Urgon part.

***** NO LONGER USED IN THE RELEASED GAME *****

IN PROGRESS

- shw_fallfx.cog                - Defines a still existing water sound (riv_h20_rapid_a.wav) for "ghost objects" and also defines a downward sector thrust. Probably a waterfall that is part of the "waterslide park" usable by Indy and mentioned by the level designer. The script receive orders (user0:) from variable "icedamcog", which was probably "shw_newriver_thaw.cog". The water flowing after the dam melts would therefore supply one or more waterfalls that can be used by Indy. (And then, maybe visitable early in the level without water, sound an thrust?)

# End
