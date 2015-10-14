------------------------

Amibiance-BLUISH_CUSTOM2

It's an Ubuntu 14.04 Ambiance theme, but tweaked for transparency and color.

Changes to the original theme:
1. Added transparency to active and inactive windows 
2. Changed windows borders to 5 px -It was hard to change window size with the 1 pixel border so ...
3. Changed the selection color in the OS to be more bluish (#8ea3bd).
4. Changed the color of theme to green (#55759e)
5. Windows borders and titlebars are now colored with mix from themes @dark_bg_color and @fg_color. 
6. Added semitransparent png images for aditional effect of windows titlebars and borders.
7. Added dark panel with the theme color in Nautilus.
8. Changed close, minimize maximize buttons in dropdown mode - used image files from the Ambiance graphite theme by ravefinity-project.
9. Moved the title of the windows to te right. 
 - If you want to change that behaviour modify "-UnityDecoration-title-alignment" parameter in "unity.css" (file is located in "/gtk-3.0" theme folder) from 1.0 to 0.0 (if you want the dafault behaviour) or to 0.50 to center the title.
10. Added theme color to the LibreOffice toolbar. Now it should respect the color changes of the theme.
 - If you want to disable this feature delete "libreoffice.rc" from "/gtk-2.0/apps" theme folder, and delete the last line "include "apps/libreoffice.rc" in "gtkrc" (file is located in "/gtk-2.0" theme folder).

---------------------
Installing the theme:
---------------------

1. Download and unpack the downloaded "tar.gz" archive to your "~home/YourUserName/.themes" folder (if there aint one just create it).
2. Use Unity Tweak Tool or whatever app suits you to load the theme. To install Unity tweak tool open terminal window and type in: "sudo apt-get install unity-tweak-tool", type your password, hit enter and follow instructions :)
3. Enjoy & comment please ;)

---------------------
Theme tweaks:
---------------------
1. To make menus and top panel transparent use Compiz config manager (CCSM). You can install it via Software center. 
 - Transparency of menus: Activate the "Opacity, Brightnes and Saturation" plugin in CCSM. Go to "WindowSpecificSettings" section in "Opacity" tab and click "New". In the openened dialog in "Windows" field paste this(without the quotes): "Tooltip | Menu | PopupMenu | DropdownMenu". In "Window values" are the the transparency settings (higher value=less transparency).
 - To make the top bar transparent go to "Ubuntu Unity Plugin" in CCSM. In "General" tab change the "Panel opacity" value to les than zero (mine is 0,300). The same goes to launcher in "Launcher" tab there is option "Launcher opacity" change it to your preferenced value.

2. The theme color can be modified to your own preference. To do it just change the values of the "@dark_bg_color" in "gtk-main.css"  file in "/gtk-3.0" theme folder from the default setting to whatever you like. For applications not using GTK3 like LibreOffice, Audacity, Google Chrome and etc change the value of the color in line: "color["bg_color_dark"] = "#your-color-here"" under the "style "dark"" in gtkrc (file is located in "/gtk-2.0" theme folder) to be the same as the one in "@dark_bg_color" in "gtk-main.css". Thats all.

3. The size of the window borders can be changed in /gtk-3.0/apps/unity.css file. Open the file in gedit or some other app and change the values in line "-UnityDecoration-extents: 28px 5 5 5" where "28px" is the height of the top and the others are the values of the left, right and bottom borders. 
--------------------
License:
--------------------
GPL2

--------------------
That's all. Enjoy!
Ilian Dimitrov - AlKaTRaZ
