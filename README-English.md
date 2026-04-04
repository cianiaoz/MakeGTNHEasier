Make GTNH Easier

### How to Start?

By default, press V to open the configuration GUI.

You can change this keybind in Controls.

![modifyDefaultKey](ReadmeResource/modifyDefaultKey.png)

🧮Control Panel

![ControlPanel](ReadmeResource/ControlPanel.png)

The function name is displayed on the left, and the control buttons are on the right.

The red OFF button on the left is used to toggle the function on or off.

The None option in the middle allows you to bind a hotkey.(ESC is bound to None)

The Set button on the right is for configuring select functions.

🛠️ Features

1. Auto Switch Tool

Auto Switch Tool features three buttons: the left button toggles the function on and off, the middle one can be bound to a hotkey for quick enabling or disabling, and the Set button switches the working modes.

There are two working modes:

Continuous(Default): When you mine a block, the mod automatically checks your hotbar, calculates the fastest tool every tick, and switches to it.

Click: The tool switching logic is only executed once when you press the left mouse button to mine.

Additional Features

1.Tinkers' Construct axes lose durability and give no XP when cutting grass. This mod features a built-in blacklist to prevent automatic axe switching while harvesting grass
2.If the mod detects you attacking a entity, it will turn off tool switching and play a sound. This stops your tools from changing unexpectedly during fights.(Falling gravel is an entity too)

2. LootGame Gol Helper

You must enable this feature before playing Game of Light.This function can read the sequence and light up the targets accordingly. You only need to click them in order as prompted.

![GOL](ReadmeResource/GOL.png)

3. LootGame MS Helper

You can turn on this feature while playing.
It will find mines and safe tiles every few seconds.
Red tiles are mines, green tiles are safe.
When there are many possible answers,
it will show you the safest tile in yellow.
The result is obtained by calculation, the feature does not know the real answer.

![MS](ReadmeResource/MS.png)

4. Slime Island Locator / Galactic Dungeon Predictor / Roguelike Dungeon predictor

After enabling these features, you will enter a subpage.
These features work similarly: you enter a seed manually, and the structure coordinates will be shown to you.
Sometimes the structure entrance is not at the calculated point, but it is nearby. Keep looking for it.
Besides, the structure may be incompletely generated or uninhabitable due to terrain issues. This feature cannot predict these situations.

5. Thaumic Ingot Predictor

Enter the in-game day shown in the top-left corner,and it will tell you when to use Research Notes to get the research note for Thaumium Ingot.
Sometimes I use certain methods to skip the Bricked Blast Furnace :),This feature is made for that purpose.
Do not use commands like /time set day, as this will reset the day counter shown in the top-left corner, leading you to enter the wrong day.

6. GT Ore Predictor

Enter a seed (this function caches your seed input. The cache will be cleared when you exit the world to reduce repeated input).
Set the radius, select the ore vein you want to find, and this function will show you its location.
The third column is a search bar, not a selection bar.
Selected ore veins will be highlighted in yellow. You can also choose ---scan all veins--- to display all vein types within the range.

Notes:
1.Only supports the Overworld and the Nether.
2.GT ore veins attempt to generate multiple times due to terrain. This function only simulates the first generation result, so it is not 100% accurate. Use this only if you cannot find the veins after trying hard
3.Use the Prospector's Scanner later. This feature will not be useful for long

Mica, Manganese, and Quartz can be really hard to find :(
The prediction accuracy for the End is far too low, possibly due to terrain. I have disabled this feature in the End to avoid misleading you. Perhaps the End uses a different ore generation logic?

![GTOrePredictor](ReadmeResource/GTOrePredictor.png)

7. Freecam

Fairly straightforward; no further explanation needed.
You can bind a key to use this function.

Notes:
1.This only ignore your mouse and movement inputs. It does not block other inputs, such as camera rotation or interactions with other mods—for example, pressing V to attach items to blocks.
2.There are no restrictions in single-player, but this function is limited in multiplayer. Read 'Commands & Server Rules'

8. TargetScanner

It uses an independent thread for scanning and draws 3D highlighted borders around target blocks in the world.

GT Ore Compatibility:
This feature supports GT ore(it cannot find GT ores that are completely covered on all six sides by other blocks).I know why this happens. It is a special rule in GT. I think the mod author did this on purpose to stop certain things. So I will not fix this in future updates. I just wanted to help you find rare ore veins easily. That’s why I made the "GT Ore Predictor" too
With this tool, "GT Ore Predictor", and the game's Prospector's Scanner,finding rare ores is much easier

Whitelist Management:
There is a built-in list of blocks this tool can scan. You cannot change this list.
Its language depends on your game's language before you open the game.If you uses Chinese at first, the list stays Chinese even if you change the game to English later.
To make the list English, set your language to English, close the game completely, then open it again.The same goes for changing back to Chinese.
This rule only affects the list, because the list initializes only once when the game starts.
Other mod text in the game will update when you change the language in-game.
Whitelist Details:
1.Single Block Group
Gypsum->OW
Coal->OW
Diamond->OW
Lapis->OW
Gold->OW
Redstone->OW
Mica->OW
RubberTreeLeaves(IC2 rubber leaves)
WispyCotton(Witchery)
2.Multiple Block Group 
Manganese->OW,Nether(MnO2 ore,not Mn ore, don't worry)
Quartz->Nether (All ores contained in the Nether Quartz Vein)
Calcite->OW,ET Future
Iron->OW (Common Ore Types, not including Tantalite)
Copper->OW (Common Ore Types)
Tin->OW (Common Ore Types)
Healing Axe Tasks->(All items needed for the Hunger No More quest)
Shimmering Mushroom->(all color)
Dungeon->(loot game and galacticraft)
Beehives->(Forestry/ExtraBees /MagicBees)

Notes
1.You must wait 1 second after turning the tool on or off.
2.This tool works freely in single-player, but has limits in multiplayer. Read 'Commands & Server Rules'

9. JourneyMap Teleport
First, open the config menu to bind a key.Then manually enable the function.Next, open the journey map and press the bound key.You will be teleported to the location your mouse is pointing to.
Note: The bound key is only used to trigger teleportation, not to turn the function on or off.
To toggle this function, you must click the button in the config menu manually.

⌨️ Commands & Server Rules

To ensure fairness for multiplayer servers

Single-player: All features are unlocked by default with no restrictions.

Multiplayer: Freecam and Target Scanner are locked by default.(The Target Scanner can use non-sensitive groups.)

To unlock them, this mod must also be installed on the server, and an admin (permission level 2) can run these commands:

/makegtnheasier list
View the authorization status of all features.

/makegtnheasier unlock <feature>
Unlock sensitive features (supports: freecam, target_scanner).

/makegtnheasier lock <feature>
Re-lock a feature.

Tip: For non-sensitive features only (such as auto tool switch, LootGame helpers), installing the mod only on the client is enough.

⚠️ Important Notes
This mod does not modify vanilla game logic, nor add new items/blocks.If you encounter any bugs, simply remove the mod to restore normal gameplay — your world will not be corrupted.

Copyright & Distribution:

Free sharing: You can share this mod freely without crediting the author.

No commercial use: Selling this mod in any form is strictly forbidden.

Open-source: This project is closed-source for now, to prevent tampering with security logic. Source code may be provided for legitimate requests.

This mod is for learning and entertainment purposes only.The author takes no responsibility for bans or penalties resulting from using this mod on servers.Please use it only in compliance with server rules.


💖 Acknowledgements
English: Special thanks to the GTNH team for their incredible dedication. More importantly, we appreciate the immense effort put into maintaining the 1.7.10 development environment, keeping this classic version of Minecraft alive and thriving.

Changelog
1.0.1
- Added support for Roguelike Dungeons to the structure location feature. You can now use this tool to predict where they will generate.
- Added quick teleport functionality for Journey Map. See the Bilibili video for details.
- Added language files. The mod now supports English.
- Fixed minor bugs from version 1.0.0.