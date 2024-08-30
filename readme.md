
# Scaleform HUD for CS:GO demos

This is an addon that replicates CS:GO's old Scaleform HUD. **It only works for watching/recording demos or playing offline with -insecure.**

To use this you will need to install [HLAE](https://www.advancedfx.org/) and [MIGI](https://zoolsmith.github.io/MIGI3/). If you are not familiar with these programs, they have guides available on their website.

## Usage

1. Place **panorama.my.zip** in **C:/Users/yourname/AppData/roaming/HLAE**. Do not extract the file.

2. Place the **p_scaleform** folder in your MIGI addons folder and click the "UPDATE BUILD" button in MIGI.

3. Open the HLAE Custom Loader and launch CSGO with the commands `-game migi/csgo -afxdetourpanorama`, like this:
![custom launcher](https://github.com/user-attachments/assets/153ffc65-1315-4f40-b239-0cf1eea70019 "custom launcher settings")

If you get an error when launching, make sure MIGI and HLAE are updated to the latest version.

## Changeable settings

- Parts of the HUD (such as the opacity of the backgrounds for health, ammo, money, and location) can be changed in **p_scaleform\panorama\styles\csgostyles.css**. You can also change the speed of the animations for certain HUD elements, hide panels, and other small things. Make sure to rebuild MIGI after making any changes.

- There is also an option to use the 2013 MVP panel. To do this, go into **p_scaleform\panorama\layout\hud\hudwinpanel.xml** and in line 4 change "hudwinpanel.css" to "hudwinpanel**old**.css", then rebuild MIGI.

- By default, weapon names in the bottom right corner are colored based on their rarity (similar to using cl_loadout_colorweaponnames 1 back when it worked). To disable this, open **panorama/styles/hud/hudweaponselection.css** and comment out everything from line 847 to 878 (it's at the very bottom) and rebuild MIGI.

## Screenshots

![POV demo, default settings](https://github.com/user-attachments/assets/1c52795c-d5c2-4224-bad5-c7c56e552e5a "POV demo, default settings")

![GOTV demo, default settings](https://github.com/user-attachments/assets/2cc08d60-9cf1-4b96-887b-59bcf7bd12bd "GOTV demo, default settings")

![defuse panel](https://github.com/user-attachments/assets/878f273d-c007-4be0-a53b-16d4cbdde46e "defuse panel")

![2013 MVP panel](https://github.com/user-attachments/assets/17c8d063-9cca-4520-a437-2d242560047b "2013 MVP panel")

## Credits

- [offline](https://www.youtube.com/offlined)
- [skam](https://www.youtube.com/@skam)
- [jo (me)](https://www.youtube.com/shittyboyz)

And thanks to ccqts and sloxy for also helping me with CSS/XML when I first started working on this project.
