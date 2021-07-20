# Unreleased-level-Shambala-Waterworks

A level was planned between Shambala Santuary and Palawan Lagoon: Shambala Waterworks. It was never included in the final game due to lack of time and technical problems. No one has seen this level since 1999 but many files have been forgotten in the game. (I'm sure it would be possible to make it work again if we had it, or recreate it if not ...)

In this level, the first step was to find to melt an ice dam in order to supply water to the whole station. For that you had to find an Oil jar, break it on the ice dam and fire the lacquer with the Zippo.
So you knew how to access the main cave. The next step was to complete three "Div rooms" in any order you want, which must be opened with "Silver key", "Gold key" and "Garnet key". The level was filled with mills, sluices and various mechanisms. The goal of this whole operation was to free four gates leading to the Ice Boss.

Two areas of this level have been cut and kept in other levels:

- The Div Room 2 (The flour mill): now in Tian Shan River. (You can see a walled-up entrance that is no longer useful)
- The Ice Boss Arena: now in Shambala Santuary. (Originally, the Shambala Santuary level ended after giving the flower to the old lady).

![alt text](https://raw.githubusercontent.com/Jones3D-The-Infernal-Engine/Unreleased-level-Shambala-Waterworks/main/04_shw.jpg?raw=true)

# Level scripts infos

***** DEPORTED AND NOW USED IN TIAN SHAN RIVER (02_riv) (Diversion room 2) *****

- shw_hammer.cog                - 
- shw_Hammer_cam.cog            - 

***** DEPORTED AND NOW USED IN SHAMBALA SANCTUARY (03_shs) (Ice boss arena) *****

- shw_noledge.cog               - Prevents Indy from hanging onto the ledge bafore the ground (thing) collapses below him (And then, not to pass his hands through the ground). By default the surface is not "hangable", it becomes "hangable" 1 second after the fall of the ground (Thing).
- 04_SHW_Cinematic_3.cog        - Cutscene triggered when Indy open the door at the end of the level, the holy woman sends him to Palawan.
- SHW_BossCinematic.cog         - Cutscenes triggeredw when Indy entered in the arena showing the ice boss and when killing him.
- shw_fogswitch.cog             - Change the fog when Indy crosses surfaces (4 for artivate and 4 for desactivate).
- SHW_IceBoss.cog               - Ai, movements and general actions of the ice boss.
- shw_IMP1control.cog           - Small cutscene triggered when Indy pick up the Urgon part.

***** NO LONGER USED IN THE RELEASED GAME *****

IN PROGRESS

- shw_fallfx.cog                - Defines a still existing water sound (riv_h20_rapid_a.wav) for some "ghost objects" and also defines a downward thrust. Probably a waterfall that is part of the "waterslide park" usable by Indy and mentioned by Chris Mc Gee. The script receive orders (user0:) by a cog variable: "icedamcog", probably "shw_newriver_thaw.cog". The water flowing after the dam melts would therefore supply one or more waterfalls that can be used by Indy. (And then, maybe visitable early in the level without water, sound an thrust?)

# End
