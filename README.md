# UNDERTALE Practice Mod
UNDERTALE mod intended for speedrun practice.

## How to install
Download the BPS patch and use the ROM patcher of your choice to apply it. Apply it to a vanilla copy of UNDERTALE v1.001 Linux, or a copy of v1.001 that has been already patched to Linux using the official speedrun.com patch file.
![image](https://github.com/fixylol/UndertalePracticeMod/assets/22797315/aa563c2c-561e-4157-8cad-1f02cf4c30bf)

## How to use
When in the overworld, press M to open the practice menu.
![image](https://github.com/fixylol/UndertalePracticeMod/assets/22797315/f1686c9b-f206-435c-889a-fbe855d8e61d)
The Main page contains options to enable/disable debug, savestate functionality, and (most) in-game music.

In the overworld or battles, use Q and E to save and load savestates. To change the savestate slot, hold down P and press a number on the number row.

Most vanilla debug behavior is preserved. I won't put every debug key here, but if you don't know how to use normal debug or need a refresher there is a helpful (and interesting) guide on [the Cutting Room Floor Wiki](https://tcrf.net/Undertale/Debug_Mode). I haven't touched most of the fights, but a lot of the weird/annoying overworld functions have been removed.

### Weapon Practice
"Practice Weapons" will open a menu for the multi-hit weapon practice mode. You can choose which boss to fight, which weapon to use, and--if applicable--your LV, whether the boss uses attacks on you, whether the boss or yourself are invincible, and your turn goal for statistics purposes.

When in the weapon practice mode, press TAB to enable or disable the statistics display in the top left corner. "Score" refers to how accurate you were with each hit, comparing your average score for the session against the maximum score of the weapon you are using. "Crits"/"Quads" will compare the amount of crits (with 2-3 hit weapons) or quads (with 4 hit weapons) you've hit against the total amount of attacks in that session. Crit/Quad streak will show your current streak, as well as the maximum streak in that session. "Last pattern" shows the last pattern you've hit.

If you have boss invincibility enabled, displayed below all this will be a simulation of the boss you're fighting. Current turn shows the turn you're currently on in the simulation, against the best possible turn count in the simulation. Previous will show the turn count of the previous simulation, as well as the average turn count (based on your average crit/quad rate in that session). Below that is a total amount of simulation bosses you've heartlessly slaughtered.

Press Q or E to change the pages. Don't worry, savestates are disabled here. On the next page there are more detailed stats of your crit/quad rate with each attack pattern of the weapon you're using.

### Timer

To enable the timer, go to "Timer Options" > "Enable timer". The timer will appear in the top left corner of the screen. To change the timer size, go down to "Timer scale" and press Z. This will increment it by 0.25, to a maximum of 2, where it will then loop back to a minimum of 0.5.

To set the rooms in which the timer will start (and optionally, end), go to "Set timer start/end rooms". There are numerous presets for IL and segment practicing. If none of these apply to you, select "Custom start/end" and input the room name or ID of the rooms you want to start and end in. If you wish to never end the timer, simply put 0 or a room that you don't intend to visit during the run time. The timer will automatically reset upon setting rooms.

## Credits

This project was started by Winter Storm. This README was also written by Winter Storm. This also her repo. She will stop talking about herself in the third person now this is weird.

A fair amount of the menu code was written by Indyindeed. This includes the functions for the input prompts, as well as drawing menu options.

This mod wouldn't exist without the original weapon practice, savestate and in-game timer mods by willyjwillyj and OceanBagel. The practice mode and in-game timer in this mod aren't their code, but it is heavily based off their designs.

This mod is built off of UNDERTALE, which was developed by Toby Fox. Thank you for accidentally creating one of the most difficult and engaging speedgames out there.
