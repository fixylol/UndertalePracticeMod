# UNDERTALE Practice Mod
UNDERTALE mod intended for speedrun practice.

## How to install
Download the BPS patch and use the ROM patcher of your choice ([Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/) is recommended) to apply it. Apply it to a vanilla copy of UNDERTALE v1.001 Linux, or a copy of v1.001 that has been already patched to Linux using the official speedrun.com patch file.
*It will likely complain about the ROM file being too big. Click "Force calculate checksum", and proceed as normal.*
![image](https://github.com/fixylol/UndertalePracticeMod/assets/22797315/aa563c2c-561e-4157-8cad-1f02cf4c30bf)

## How to use
When in the overworld, press M to open the practice menu.
![image](https://github.com/fixylol/UndertalePracticeMod/assets/22797315/f1686c9b-f206-435c-889a-fbe855d8e61d)

The Main page contains options to enable/disable debug, savestate functionality, and (most) in-game music. The Stat page contains options to change your stats, such as LV, HP, EXP, Gold, or Name. The Item page lets you select from a list of every item in the game (excluding duplicates) to place into your inventory. The Misc page contains options to change file0 and undertale.ini flags, plot and fun values, and other miscellaneous features.

In the overworld or battles, use Q and E to save and load savestates. To change the savestate slot, hold down P and press a number on the number row.

Most vanilla debug behavior is preserved. I won't put every debug key here, but if you don't know how to use normal debug or need a refresher there is a helpful (and interesting) guide on [the Cutting Room Floor Wiki](https://tcrf.net/Undertale/Debug_Mode). I haven't touched most of the fights, but a lot of the weird/annoying overworld functions have been removed.

MDS practice will warp you to the Mad Dummy room, with all the proper flags set and a punch card in your inventory. When you perform MDS, a display in the top-left corner of the screen will show whether you were early, late or on-time.

This mod will automatically check this repo for updates by default. If you wish to turn this off, go to Misc > "Menu options..." > "Automatically check for updates".

If you wish to give feedback, report bugs, or just want to be notified for new updates, feel free to [join my discord!](https://discord.gg/4d82wPGHau)

## Weapon Practice
"Practice Weapons" will open a menu for the multi-hit weapon practice mode. You can choose which boss to fight, which weapon to use, and--if applicable--your LV, whether the boss uses attacks on you, whether the boss or yourself are invincible, and your turn goal for statistics purposes.

When in the weapon practice mode, press TAB to enable or disable the statistics display in the top left corner. "Score" refers to how accurate you were with each hit, comparing your average score for the session against the maximum score of the weapon you are using. "Crits"/"Quads" will compare the amount of crits (with 2-3 hit weapons) or quads (with 4 hit weapons) you've hit against the total amount of attacks in that session. Crit/Quad streak will show your current streak, as well as the maximum streak in that session. "Last pattern" shows the last pattern you've hit.

If you have boss invincibility enabled, displayed below all this will be a simulation of the boss you're fighting. Current turn shows the turn you're currently on in the simulation, against the best possible turn count in the simulation. Previous will show the turn count of the previous simulation, as well as the average turn count (based on your average crit/quad rate in that session). Below that is a total amount of simulation bosses you've heartlessly slaughtered.

Press Q or E to change the pages. Don't worry, savestates are disabled here. On the next page there are more detailed stats of your crit/quad rate with each attack pattern of the weapon you're using.

## Timer

By default, the timer can be started/ended with the Space key and reset with the G key. To change the keys used for the timer, go to "Edit hotkeys" and select each option you wish to change.

If you wish to change the look of the timer, go to "Edit style". You can change the size of both timers and the splits, the font of the timers and splits, the opacity of the background, and the format the splits are displayed in.

To change what the 2 timers display, look below to where it says "Timing" and "Update". "Timing" refers to what the timer reads ("Run" time, which is overall, or "Segment" time which is the specific segment if you're using splits). "Update" refers to when this timer updates, either constantly (every frame) or upon entering a room.

### Defining splits

This mod comes with several split presets, available in the "Presets" menu. "Midgame RTA" is Waterfall, Hotland and New Home. The rest are self-explanitory. These splits use common split times, used by runners like mrlink2k, Winter Storm (that's me!) and Shayy.

If you wish to customize these splits, or make your own entirely, go to the "Edit splits" menu.

To add a split, first select "Add split". A text box will appear. You can type in a room name or ID to have the timer split (or begin if it's the first split, or end if it's the last split) upon entering that room. If you wish to have it split upon entering through a specific door in that room, and you know what the global.entrance value for this room is, then you can specify that as a decimal to the room ID. Note that this decimal must have a leading 0 if it's below 10. For example, if you wish to split upon entering room 139 through entrance 2, input 139.02.

You can also split upon cutscenes. This requires knowing what the ID of the cutscene object is, as well as the con value. This information can be gathered through UNDERTALE Mod Tool (or just ask around in the UNDERTALE server, I'm sure someone will be happy to help). When you have the ID and con value, input the ID as a negative number and then the con value as a decimal (and, similar to entrance values, the con value must have a leading 0 if it's below 10). The 2 examples in the presets are -1039.16 (object 1039 being the object for the Undyne Spears 2 cutscene) and -1566.04 (object 1566 being the elevator at the end of True Lab). If you wish to have Spears 2 split upon the bridge being cut, rather than the fadeout, set your Spears 2 split as -1039.10.

## Credits

This project was started by Winter Storm. This README was also written by Winter Storm. This also her repo. She will stop talking about herself in the third person now this is weird.

A fair amount of the menu code was written by Indyindeed. This includes the functions for the input prompts, as well as drawing menu options.

This mod wouldn't exist without the original weapon practice, savestate and in-game timer mods by willyjwillyj and OceanBagel. The practice mode and in-game timer in this mod aren't their code, but it is heavily based off their designs.

This mod is built off of UNDERTALE, which was developed by Toby Fox. Thank you for accidentally creating one of the most difficult and engaging speedgames out there.
