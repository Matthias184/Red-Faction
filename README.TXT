            ==========================
               Red Faction - v 1.20
                    Readme File
            ==========================

For more information on Red Faction, please visit
  www.volition-inc.com  or  www.redfaction.com


Version History:

1.20
 - Fixed hole in VPP loading that allowed cheaters to run mod-like
   changes without actually running a mod.

1.10
 - Made changes to require fewer hard drive accesses during gameplay.
 - Fixed data-mismatch problem when joining a multiplayer server that
   gave the "Data does not match" error message. 
 - Fixed instances where a multiplayer server would crash when kicking
   a player.
 - Fixed railgun trajectory visual to no longer deflect off some walls.
 - Fixed crash from clicking on scroll bar in multiplayer map list.
 - Fixed misplaced dedicated server/password icons on Servers screen
   when using 1280 resolution.
 - Fixed selection problem when changing Filter on Servers screen.
 - Fixed server list to properly identify servers running mods
 - Fixed console closing problem.  Only need to hit "~" once now.
 - Fixed crash instances caused by hitting both "Shift" keys simultaneously.
 - L14S3 endgame screen text now displays properly in 800x600.
 - Railgun will properly fire through multiple targets.
 - Removed delay in picking up dropped weapons in multiplayer.
 - First-person arms on "Scientist Parker" and "Ultor Scientist" now 
   match models in multiplayer.
 - Zooming in with scoped weapons now displays scope if first person
   weapons are turned off.
 - Disabled "Shift-Esc" to quit out of game.
 - Dedicated server now skips over any missing maps found in map lists.
 - Disabled save games during the bomb defuse screen.
 - RED levels now work when you install the game to a directory
   path with spaces in it.
 - Fixed crash with the RED running out of VRAM when desktop is at
   very high resolutions.
 - Changed RED to favor the updated CHM help file, if it exists.
 - Removed unused flags from RED's Light Properties dialog.
 - RED can now import V3D files as mesh brushes.  Requires V3D exporter
   for 3ds Max found in the RFToolkit.

1.00
 - Initial Release


-----------------
Table of Contents
-----------------

1. Manual Addenda
     1a. Join Game/Servers screen
     1b. Create Game/Options screen

2. The Red Faction Launcher
     2a. Play
     2b. Setup
     2c. Readme
     2d. Update
     2e. Uninstall
     2f. Exit
     2g. Volition Logo
     2h. THQ Logo

3. Console Commands

4. Dedicated Server Operation

5. Capture the Flag Rules

6. Recommended Multiplayer Level Loads

7. RED - The Red Faction Editor

8. Mod Support

9. Troubleshooting

10. Technical Support Information

11. Red Faction Web Links

12. Legal Stuff


-----------------
1. Manual Addenda
-----------------
A few changes to the game were made after the game manual went to print.
This section documents where the game functionality differs from what's
described in the manual.

1a.  Join Game/Servers Screen (page 7)
  The "Connect" option was replaced with a "LAN-only" checkbox.  By default,
this option is off, showing you all tracked Internet game servers.  Turning
this option on will show you only those games running on your local area
network.

The "Mod" filter option described in the manual was removed.  Instead,
servers running mod games are shown in a different color in the server
list.

Two optional icons may appear in the Game Type column.  One is a "computer"
icon indicating the server is in dedicated mode (see Section 4).  The
other is a padlock-type icon, indicating the server is password protected.


1b.  Create Game/Options screen (page 8)
  A new option called "LAN-only Game" was added to this screen.  By turning
this on, your game will be running >only< over your local area network,
and not over the Internet via the THQMultiplay Game Tracker.  Players
wishing to join your LAN-only game will need to also enable this option
on their Join/Servers screen.

The "Dedicated" button described on page 9 of the manual was removed.
You must use the "-dedicated" command-line option in order to run a
dedicated multiplayer server.  Please see section 4 of this README
for details.



---------------------------
2. The Red Faction Launcher
---------------------------

The Launcher's buttons enable you to set up and play Red Faction, customize 
your hardware settings, get updated versions of Red Faction, and access the
Red Faction web pages at Volition, Inc. Here's what each button does:

2a. Play
  Click this to launch Red Faction.

2b. Setup
  Under Setup, you'll see tabs for Video, Audio, Speed, Network, DirectX, 
and Misc.

  * Video - You must have a 3D Accelerator card to play Red Faction. You can 
have Red Faction detect your video card by clicking on the "Detect Available 
Cards" button while choosing from one of four resolutions and either a 16-bit
or 32-bit framebuffer.

NOTE to 3dfx Voodoo card owners:
Red Faction should automatically detect if you are trying to run the game
on a Voodoo card.  If you encounter difficulty getting the game to run,
Red Faction will allow you to use command-line parameters to allow you to
play.  Use the command-line parameters "-voodoo" for any Voodoo cards
except the Voodoo3, and "-voodoo3" for the Voodoo3 if you have difficulty.

  * Audio - Red Faction supports DirectSound, and EAX. You can choose one of
these by clicking on "Detect Available Sound Cards" and then selecting from 
the dropdown box and checking the appropriate checkbox. You can enable Launcher 
sounds from here as well.

  * Speed - This setting determines the default Detail Level used in 
Red Faction. You may manually change this default if you wish, but it may 
adversely affect your gameplay speed.

  * DirectX - On this tab you can check your DirectX version and choose to 
install or update DirectX on your machine.

  * Misc. - This tab allows you to enter optional command-line switches.
Valid switches include:

   -dedicated <game config name>
   -lanonly
      See the section on Dedicated Server Operation for details on these.

   -voodoo
      Forces RF to use your any Voodoo compatible cards instead of the one
   specified in the RF Launcher.  Note, Voodoo3 owners need to use the
   card-specific "-voodoo3" option instead.

   -voodoo3
      Same as "-voodoo", but for Voodoo3 cards only.

   -timedemo <levelname>
      Player is created at start of level and spins around once. stats on
      framerate are recorded and displayed in the console and in a text file.

   -frameratetest <levelname>
      Same thing as timedemo, but does the spin/sample at each node in the
      level, giving stats for each node and the level as a whole.

   -level <levelname>
      This tells Red Faction to load the level file specified.  The RFL
      level file needs to be inside a VPP file, created either by RED using
      the File/Create Level Packfile command, or a third-party VPP editing
      tool.  This VPP file may be in either the \user_maps\single or \multi
      directories.

   -mod <modname>
      This tells RF to use the specified "mod" files in place of any
      standard files.  Please see Section 7 of this readme for more
      information on data-based mods.


2c. View Readme
  View this file.


2d. Update
  This button enables you to see if a new version of Red Faction is
available for downloading. If one is available, you can choose to
update by clicking on OK. The process is automated.


2e. Uninstall
  Uninstalls Red Faction from your computer.


2f. Quit
  Closes the Launcher without running Red Faction.


2g. Volition Logo
  This takes you to Volition's Internet home page.


2h. THQ Logo
  This takes you to the Internet home page for THQ.


-------------------
3. Console Commands
-------------------
     The RF game console can be toggled on/off using the tilde "~" key.  This
gives you access to a few special commands and shortcuts.  Most of these are
only used in multiplayer games.

name <player name>
   Changes your Multi/Player playername to the name specified.

rate <connection type | value>
   Sets the rate at which game servers are allowed to send you update
   packets in multiplayer games.  This is equivalent to the "Connection
   Speed" setting on the Network tab in the RF Launcher.  Valid connection
   types, and their pre-defined rates (in bytes-per-second) are:
      modem    2600
      isdn     5000
      cable   15000
      t1      30000
      lan     30000
   You can also specify an exact numerical rate instead of a connection
   type.

simultaneous_ping <value>
   Determines how many servers can be pinged/queried at the same time in
   the Servers screen.  Default is 16.  Players with high-bandwidth
   connections may be able to increase this without problems.

team <red | blue>
   Switch yourself to the specified team in Team multiplayer modes.  Valid
   choices are "red" and "blue".

rcon_request <rcon password>
   Request rcon command access on a dedicated server.  See the readme section
   on dedicated server operation for details.

rcon <console command>
   Issues an rcon command.  See readme section on dedicated server operation
   for details.

info
   Displays a list of connected players

level <level filename>
(server command)
   Server command to change to specified level.  Example: "level ctf08".
   Leave off the .RFL extension.  If running a dedicated server, the rcon
   prefix is necessary.  See the readme section on dedicated server
   operation for details.

kick <playername>
(server command)
   Boots the specified player off your server.  Rcon access is needed
   if attempting this on a dedicated server.  Quotes around the playername
   may be required if the name contains special characters or spaces.

ban <playername>
(server command)
   Bans the named player by adding his/her IP address to "banlist.txt".
   The "banlist.txt" file is preserved between server sessions.
   Wildcards are also supported to ban multiple IP's on the same subnet.
   Examples:
      63.123.86.41
      65.123.86.*
      65.*
   Wildcards in the middle of the address are not valid.

ban_ip <IP address>
(server command)
   Same as "ban", but allows use of player's IP address instead of his/her
   playername.  Note, both ban commands add IP addresses to the
   "banlist.txt" file, the difference is only in how the server initially
   specifies the player.


-----------------------------
4. Dedicated Server Operation
-----------------------------

Server Options ---
All dedicated server options are stored in the "dedicated_server.txt" file, found
in your Red Faction install directory.  This is a simple text file with a list of
supported options, and their parameters.  Full instructions on each option can
be found at the top of that file.

Starting a Server ---
First, make sure you have correctly set your network connection type in the RF
Launcher.  This is found under Setup, under the Network tab.  It's CRUCIAL that
you set this correctly for proper server operation.  The same is true for
non-dedicated servers.

Dedicated servers must be run from the command-line, using the game
executable "RF.exe".  Example:

  rf -dedicated dm

This will start Red Faction in dedicated server mode, using the "dm"
game configuration found in the "dedicated_server.txt" file.  With the default
settings, this starts a Deathmatch game for up to 16 players.  Another default
configuration is included, named "ctf", using Capture the Flag mode.

Another way to start RF in dedicated mode, is by entering "-dedicated <configname>"
in the command-line field on the Launcher's Setup/Misc tab, then hitting Play.
This is the equivalent of running "rf -dedicated <configname>" from a command
prompt.


Additional Command-Line Options ---

-lanonly
   This optional command-line parameter tells the server to /not/ notify
the THQMultiplay Game Tracker about its location.  This switch ONLY affects 
dedicated servers. When using this option, your server will not appear on the 
THQMultiplay server lists.  It will only be visible to players on your LAN, or 
to those that use the "Add Server" button to contact it by IP address. In-game
(non-dedicated) server type is completely controlled by the "Lan Only" checkbox
on the server create options screen.


Special Server Commands ---
You will only see a console display while your dedicated server is running.
You are able to enter server commands simply by typing them into the console.
Most of the commands described below are also available for non-dedicated
servers, through the regular in-game console.

level <level filename>
   Changes to the named level.  Example: "level ctf05".  Leave off the .RFL
   extension.  You can only change to levels appropriate for the current
   game mode.  Meaning, you can't load a "ctf*" level while running Deathmatch.

info
   Displays a list of players currently connected to the server, current ping
   times, and IP addresses.

kick <playername>
   Boots the named player off your server.

ban <playername>
   Bans the named player by adding his/her IP address to "banlist.txt".
   The "banlist.txt" file is preserved between server sessions.
   Wildcards are also supported to ban multiple IP's on the same subnet.
   Examples:
      63.123.86.41
      65.123.86.*
      65.*
   Wildcards in the middle of the address are not valid.

ban_ip <IP address>
   Same as "ban", but allows use of player's IP address instead of his/her
   playername.  Note, both ban commands add IP addresses to the
   "banlist.txt" file, the difference is only in how the server initially
   specifies the player.

say <message text>
   Sends a server chat message to all players.

quit
   Unloads the data and shuts down the dedicated server.

Remote Console Commands ---
You can use a few dedicated server commands while playing on your server.
To enable remote console operation (rcon), hit the tilde "~" key while
playing to bring down the game console, and type:

  rcon_request <rcon password>

You can set your server's rcon password in the "dedicated_server.txt" file.
If you correctly enter it using the "rcon_request" command, everyone will
receive a chat message indicating you were granted rcon access.

At this point you can issue selected server commands such as "level", "kick",
and "ban".  While using rcon access, they must be prefixed by "rcon".
Example:

  rcon level dm13

Assuming you have rcon access, this console command switches to dm13.rfl.


-------------------------
5. Capture the Flag Rules
-------------------------
   Red Faction offers Multiplayer Capture the Flag for two opposing teams of
players. The object of the game is to score points for your team by collecting
your opponents' flag and returning it to your base while protecting your own
flag.
   Teams are awarded one point per capture. To capture, you have to touch your
opponents' flag to automatically steal it. While carrying the flag, you will
see a flashing flag icon in the lower left of the screen besides the team score.
You must return the enemy flag to your own flag stand while your flag is there
in order to score a point.
   If your own flag is stolen, to return it to the flag stand you must kill the
opponent carrying the flag, which will be visible on his back and will emanate a
glow that matches your team color. When killed, the opponent will drop the flag
in the field -- you must touch the flag to return it to your base before another
opponent comes and touches the flag to pick it back up.
   Games can be set to terminate after a certain number of captures by a team or
can end after a set time. In addition to team score, players are awarded individual
points for kills as well as capturing or defending flags. Individual scores do not
affect team score.


--------------------------------------
6. Recommended Multiplayer Level Loads
--------------------------------------

CTF01: "Blasted Canyon"        8-12
CTF02: "Warlords"              6-10
CTF03: "Score"                12-16
CTF04: "Nemesis"               8-12
CTF05: "Checkmate"             6-8
CTF06: "The Art of War"       24-32
CTF07: "En Masse"             24-32

DM01:  "The Lobby"             4-6
DM02:  "Installation XJ15"     4-6
DM03:  "Waste Treatment Plant" 4-6
DM04:  "Badlands"              8-16
DM05:  "Hangar18"              6-10
DM06:  "High and Dry"          8-12
DM07:  "Mine Warfare"          8-12
DM08:  "Relentless"            4-6
DM09:  "Office Space"          8-12
DM10:  "Any Way"               4-8
DM11:  "Watch Your Step"       4-6  (EXCLUSIVE!)
DM12:  "Killbox"               4-6
DM13:  "Mazeway"               4-6
DM14:  "Coffee Break"          4-6
DM15:  "One to the Dome"       8-12
DM16:  "S.R.O."                4-8
DM17:  "Grey Matter"          12-16
DM18:  "Zig"                   4-6  (EXCLUSIVE!)      
DM19:  "High Rise"             8-12            
DM20:  "Hermis"                2-6


-------------------------------
7. RED - The Red Faction Editor
-------------------------------
Red Faction includes RED, the full-featured level editor used by Volition to
create the RF levels.  A shortcut to RED can be found in your Red Faction
folder under the Start Menu.

Online documentation for RED is available under the Help/Help Topics menu.
All RED functions are documented in more detail in the Help file.  Here
are a few of the basics:

Any levels you create need to be saved in one of these directories:
  \RedFaction\user_maps\single
  \RedFaction\user_maps\multi

THE GAME WILL NOT LOAD RFL FILES DIRECTLY.  You need to export your level into
a VPP "packfile" with the "Create Level Packfile" under the File menu.
You will need to do this before using the "Play Level" command, or
before attempting to find the level in the Multiplayer map list screen.
Please see the Tutorials section of the RED online Help file for details.

Custom Textures:
You can add new level textures to RED by saving them to this folder:
  \RedFaction\user_maps\textures

All textures must be 24- or 32-bit TGA (Targa) files.  They must be
a power of 2 in each dimension (32x32, 64x32, 256x256, etc.)

If you use the "Create Level Packfile" command on any level that uses
custom maps, they will automatically be included in the new VPP file.
Please see the Tutorials section of the RED online Help file for details.


--------------
8. Mod Support
--------------
Red Faction contains support for data-based "mods".  A basic tutorial on
how to create a mod can be found in this file:
  \Red Faction\mods\MOD Tutorial.txt

Also see the Tutorials section of the RED online Help file for details
on RED editor usage with mods.


------------------
9. Troubleshooting
------------------

SUPPORTED CARDS
---------------

Red Faction has been tested with the following video cards:

NVidia Geforce, Geforce 2, and Geforce 3.
NVidia TNT and TNT2.
3dfx Voodoo2 through Voodoo5 (D3D only).
Matrox G400.
Radeon.
ATI Rage 128.
PowerVR Kyro II.

If your card is not on the list, you can still run Red Faction but may 
experience technical problems.


===================================================
Installation notes for Microsoft ADPCM installation
===================================================

Note: you only need to do this if you did not hear the test sound
in the launcher.

Red Faction requires that Microsoft's ADPCM audio commpression codec be 
installed.  If your system does not currently have it, you can install 
the codec by following these instructions:

1) Open the 'Control Panel' - in Start->Settings->Control Panel
2) Open 'Add/Remove Programs'
3) Click on the 'Windows Setup' tab
4) Highlight multimedia
5) Click details
6) Make sure that the 'audio compression' checkbox is fully checked.  
   If you cannot hear sounds, then chances are that this box is in the 
   half-greyed out.
7) hit ok
8) hit ok again


===================================================
EAX
===================================================

Users running Win2k need to get updated drivers from Creative's site for 
EAX to work in Win2k.


===================================================
Video Cards
===================================================

Please ensure you are using the latest drivers available for your video card
if you experience random crashes, exits, or graphical glitches while playing 
Red Faction.  You should check your card manufacturer's site for drivers first, 
and use generic chipset drivers if your manufacturer's drivers do not 
resolve the problem.  A list of web sites for generic drivers is listed 
below.

If problems persist, make sure that your computer and video card's BIOS are
both updated to the latest version (particularly for AGP cards) and that 
your video card is on the supported list of hardware for your motherboard.

All Nvidia cards:

Red Faction has been tested using version 6.50 of Nvidia's Detonator 3 drivers.  You should 
try using the latest drivers for your Nvidia card before running Red Faction, though some
users have reported problems running games with the 21.81 drivers.  If you do encounter
problems with the 21.81 drivers, you can try earlier ones to rectify the problem.


Nvidia drivers are available at:

http://www.nvidia.com/Products.nsf/htmlmedia/detonator3.html

Matrox cards:

Red Faction has been tested using version 6.04 of Matrox's drivers.  You 
may experience random crashes or texture corruption if you are using an 
earlier version of these drivers.

Matrox drivers are available at:

http://www.matrox.com/mga/support/drivers/home.cfm

ATI Rage 128:

Drivers are available at:

http://support.ati.com/products/pc/rage128pro/rage128pro_drivers.html

3dfx Voodoo cards:

Red Faction should automatically detect if you are trying to run the game on a Voodoo 
card.  If you encounter difficulty getting the game to run, Red Faction will allow 
you to use command-line parameters to allow you to play.  Use the command-line parameters
" -voodoo " for any Voodoo cards except the Voodoo3, and " -voodoo3 " for the Voodoo3 if 
you have difficulty.

Red Faction has been tested with the following driver versions for Voodoo cards. We
recommend using these drivers if at all possible, since older drivers may not be tested
with or support DirectX 8.0 which is necessary to run Red Faction:

Voodoo 4/5: Version 1.04.00 (WHQL Certified)
Voodoo   3: Version 1.07.00 (WHQL Certified)
Voodoo   2: Version 3.02.02 (Reference Drivers)

In addition, there are 3rd party drivers for Voodoo cards available on voodoofiles.com
that are newer than the drivers listed here. While they have not been tested, some users
have reported success using them and you may wish to try them.

When using the Red Faction editor RED, Voodoo card users should set their desktop color 
depth to 16-bit in Windows. 

Voodoo2 cards:

If you have a Voodoo2, the RF Launcher will still list 1024x768 and 1280x1024 as
valid resolutions.  No Voodoo2 cards can support 1280x1024, and unless you're running
in SLI, you cannot use 1024x768, either.  The max resolution for non-SLI Voodoo2 cards
is 800x600.  Choosing a resolution higher than this may cause the game to crash.

The latest Voodoo drivers can be downloaded from http://www.voodoofiles.com if the 
3dfx.com website is not available.

Radeon:

If problems are encountered using Radeon cards with the latest release drivers, you
may get better results using the 4.13.7115 beta drivers instead.

==================================================
Hardware Acceleration
==================================================

You may encounter problems running Red Faction if your hardware acceleration settings
are not set properly. Make sure your hardware acceleration is set to either
"Most Functions" or "Full."

==================================================
Accessibility Options
==================================================

There are a number of accessibility shortcuts that are enabled by default in some
Windows operating systems, such as XP. When activated, these features may bring up
pop-up windows which can cause Red Faction to crash. If you experience these problems,
you may disable the shortcuts by going to the Control Panel and looking under 
"Accessibility Options." In general, you should disable programs that use pop-ups while
playing Red Faction.

==================================================
Memory Management
==================================================

If you run out of memory while playing Red Faction, you can take steps to help
alleviate this problem in Windows. Make sure you allow Windows to manage your virtual
memory and shut down other programs that are not needed during the game, including those
in the taskbar. In addition to this, you should make sure you have an adequate amount of
free hard drive space available for swapping by all your programs.

==================================================
ALT-Tab Issues
==================================================
You may experience problems if you use Alt-Tab to exit Red Faction. For immediate
program exit, press Shift-Esc.

==================================================
Modem Dial-out Problems
==================================================
If you are connecting to the Internet via modem and using ICQ, you may experience
an undesired dial-out. The installer/uninstaller may dial-out when ICQ has been
running previously but is NOT running at install/uninstall time. If the modem is
already connected, or if ICQ is running (or was never running to begin with), you
will not encounter this problem.


==================================================
AGP Aperture Size
==================================================

If the game crashes on startup or periodically while playing, you can try lowering 
the AGP aperture size in your system's BIOS setup utility to 64 megabytes. This option is
typically found under the "Chipset Features Setup." You may also wish to ensure that
your system's AGP drivers and BIOS are up to date by downloading the latest updates 
from your motherboard's manufacturer's web site (particularly if you have an ASUS
motherboard). These problems have ocurred under Windows 2000 while using GeForce cards,
though other configurations might be subject to similar problems.


==================================================
VIA Chipsets and SoundBlaster Live
==================================================

A number of users have reported problems when running motherboards with the VIA 686B
chipset in combination with a SoundBlaster Live. This problem is not specific to Red
Faction, and you can read more about the issue at the following urls:

http://www.realworldtech.com/page.cfm?ArticleID=RWt042201222938

http://www.ipkonfig.com/Articles/Via-SBL/index.shtml


==================================================
Joystick Users
==================================================

Joystick control is not officially supported by Red Faction. For those players who 
are more comfortable using a joystick for games, we recommend using the "JoyToKey"
program which supports mouse emulation (including wheel support). It is available for
download at the following URL:

http://hp.vector.co.jp/authors/VA016823/joytokey/english.html


==================================================
DirectX Initialization Errors
==================================================

In some instances users may get an error when trying to run Red Faction concerning
the initialization of DirectX 8.0. An example of this error is listed below:

Error: Unable tto initialize DirectX 8.0 - Device creation failed!
File: C:\projects\RF_PC\vsdk\gr\directx\gr_direct3d.cpp - Line 1872

A player can often get around this error simply by rebooting their system and then
running Red Faction again.

---------------------------------
10. Technical Support Information
---------------------------------
If you're unable to resolve your problem with the above information,
please contact THQ for assistance.

   THQ Customer Service Department
   818-880-0456
   http://www.thq.com/support/

Live Customer Service Representatives are available to help you
Monday through Friday, 9am to 5pm PST, or you can use our automated
systems by phone or on the web 24 hours a day, 7 days a week.

Your 5-digit Product Code is 49026.  Please have this number ready
when you contact Customer Service.


-------------------------
11. Red Faction Web Links
-------------------------

If you're interested in Red Faction-related web sites and information, here 
are some great places to start.

Volition, Inc. homepage - The official homepage of Volition, Inc.
  http://www.volition-inc.com

THQ, Inc. homepage - The official homepage of THQ, Inc.
  http://www.thq.com

Red Faction homepage - The official Red Faction homepage
  http://www.redfaction.com

Red Faction Watch - An excellent fan run website which not only features 
comprehensive Red Faction coverage but for all of Volition's games.
  http://redfaction.volitionwatch.com/
  http://www.volitionwatch.com/

Descent Network's Red Faction - A fan run website offering many
downloads as well as tools for user-made mods.  They're also home to the
Red Faction Webring.
  http://www.red-faction.com/
  http://www.red-faction.com/webring/


---------------
12. Legal Stuff
---------------

THQ Inc. Software License Agreement

1.	READ THE FOLLOWING TERMS AND CONDITIONS CAREFULLY BEFORE INSTALLING THE 
PROGRAM. THIS SOFTWARE LICENSE AGREEMENT IS A LEGAL AGREEMENT BETWEEN YOU 
(AN INDIVIDUAL OR A SINGLE ENTITY "YOU") ON ONE HAND, AND THQ INC. AND ITS 
SUBSIDIARIES AND AFFILIATES (COLLECTIVELY REFERRED TO AS "COMPANY") ON THE 
OTHER HAND, FOR THE SOFTWARE PRODUCT ENTITLED "RED FACTION," WHICH 
INCLUDES COMPUTER SOFTWARE AND ANY ASSOCIATED MEDIA, PRINTED MATERIALS, 
AND/OR "ONLINE" OR ELECTRONIC DOCUMENTATION (TOGETHER CALLED THE 
"PROGRAM"). BY INSTALLING, COPYING, OR OTHERWISE USING THE PROGRAM (OR, IN 
THE EVENT YOU HAVE PURCHASED THE PROGRAM AS CONTAINED ON A CD-ROM, BY 
OPENING THE PACKAGING MATERIALS THEREOF), YOU ACKNOWLEDGE THAT YOU HAVE 
READ THIS SOFTWARE LICENSE AGREEMENT AND AGREE TO BE BOUND BY ITS TERMS.  
IF YOU DO NOT AGREE TO THE TERMS OF THIS SOFTWARE LICENSE AGREEMENT, DO 
NOT INSTALL OR USE THE PROGRAM AND DELETE ALL COPIES IN YOUR POSSESSION. 

2.	Company grants you a non-exclusive, non-transferable license to use the 
Program, but retains all property rights in the Program and all copies 
thereof.  You may:  (i) use the Program on any supported computer 
configuration, provided the Program is used on only one (1) such 
computer; and (ii) permanently transfer the Program and its documentation 
to another user provided you retain no copies and the recipient 
agrees to the terms of this Agreement.  You may not transfer, 
distribute, rent, sub-license, or lease the Program or documentation, 
except as provided herein; or alter, modify, or adapt the Product or 
documentation, or portions thereof.

3.	You acknowledge that the Program in source code form remains a 
confidential trade secret of Company.  You agree not to modify or 
attempt to reverse engineer, decompile, or disassemble the Program, 
except and only to the extent that such activity is expressly permitted 
by applicable law notwithstanding this limitation.

4.	OWNERSHIP: All right, title and interest and intellectual property 
rights in and to the Program (including but not limited to any titles, 
computer code, themes, objects, characters, character names, stories, 
dialog, catch phrases, locations, concepts, artwork, images, 
photographs, animations, video, sounds, audio-visual effects, music, 
musical compositions, text and "applets," incorporated into the 
Program), the accompanying printed materials, and any copies of the 
Program, are owned by Company or its licensors. This Agreement grants 
you no rights to use such content other than as part of the Program. 
All rights not expressly granted under this Agreement are reserved by 
Company.

5.	This Agreement is effective upon your installation of the Program 
and shall continue until revoked by Company or until you breach any 
term hereof; upon termination you agree to destroy or delete all 
copies of the Program in your possession. 

6.	You shall not modify the Program or merge the Program into 
another computer program (except to the extent the Program is made 
to operate within a computer operating system and in connection with 
other computer programs) or create derivative works based upon the 
Program. 

7.	The Program may not be downloaded or otherwise exported or 
re-exported into (or to a national or resident of) any country to 
which the U.S. has embargoed goods or to anyone on the U.S. Treasury 
Department list of Specially Designated Nationals or the U.S. Commerce 
Department's Table of Deny Orders. If you do not meet these criteria 
or are not sure, do not install the software and destroy any copies 
in your possession. If you live in such a country, no license is 
granted hereunder.

8.	You are responsible for assessing your own computer and the 
results to be obtained therefrom. YOU EXPRESSLY AGREE THAT USE OF THE 
PROGRAM IS AT YOUR SOLE RISK. THE PROGRAM IS PROVIDED ON AN "AS IS," 
"AS AVAILABLE" BASIS, UNLESS SUCH WARRANTIES ARE LEGALLY INCAPABLE OF 
EXCLUSION. EXCEPT WITH RESPECT TO THE LIMITED CD-ROM WARRANTY AS SET 
FORTH IN SECTION 9 BELOW, COMPANY AND ITS LICENSORS DISCLAIM ALL 
WARRANTIES AND CONDITIONS, WHETHER ORAL OR WRITTEN, EXPRESS OR 
IMPLIED, INCLUDING WITHOUT LIMITATION ANY IMPLIED WARRANTIES OR 
CONDITIONS OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, 
NON-INFRINGEMENT OF THIRD PARTY RIGHTS, AND THOSE ARISING FROM A 
COURSE OF DEALING OR USAGE OF TRADE, REGARDING THE PROGRAM. COMPANY 
AND ITS LICENSORS ASSUME NO RESPONSIBILITY FOR ANY DAMAGES SUFFERED 
BY YOU, INCLUDING, BUT NOT LIMITED TO, LOSS OF DATA, ITEMS OR OTHER 
MATERIALS FROM ERRORS OR OTHER MALFUNCTIONS CAUSED BY COMPANY, ITS 
LICENSORS, LICENSEE AND/OR SUBCONTRACTORS, OR BY YOUR OR ANY OTHER 
PARTICIPANT'S OWN ERRORS AND/OR OMISSIONS. Company and its licensors 
make no warranty with respect to any related software or hardware 
used or provided by Company in connection with the Program except 
as expressly set forth above.

9.	LIMITED CD-ROM WARRANTY: Notwithstanding anything to the contrary 
contained herein, and solely with respect to Programs distributed on 
CD-ROM, Company warrants to the original consumer purchaser of this 
Program on CD-ROM that the recording medium on which the Program is 
recorded will be free from defects in material and workmanship for 
90 days from the date of purchase. If the recording medium is found 
defective within 90 days of original purchase, Company agrees to 
replace, free of charge, any product discovered to be defective 
within such period upon its receipt of the product, postage paid, 
with proof of the date of purchase, as long as the Program is still 
being manufactured by Company. In the event that the Program is no 
longer available, Company retains the right to substitute a similar 
program of equal or greater value. This warranty is limited to the 
recording medium containing the Program as originally provided by 
Company and is not applicable to normal wear and tear. This warranty 
shall not be applicable and shall be void if the defect has arisen 
through abuse, mistreatment, or neglect. Any implied warranties 
prescribed by statute are expressly limited to the 90-day period 
described above. To receive warranty service:  Notify the THQ 
Customer Service Department of the problem requiring warranty service 
by calling (818) 871-880-0456 or on the web at http://www.thq.com.  
If the THQ service technician is unable to solve the problem by phone 
or on the web via e-mail, he will authorize you to return the Product, 
at your risk of damage, freight and insurance prepaid by you, together 
with your dated sales slip or similar proof-of-purchase within the 
ninety (90) day warranty period to:  THQ Inc., Customer Service 
Department, 27001 Agoura Road, Suite 325, Calabasas Hills, CA 91301.  
Company is not responsible for unauthorized returns of the Program 
and reserves the right to send such unauthorized returns back to 
customers.  This warranty shall not be applicable and shall be void 
if:  (a) the defect in the Program has arisen through abuse, 
unreasonable use, mistreatment or neglect; (b) the Program is used 
with computer software and hardware not meeting the minimum systems 
requirements for the Program; (c) the Program is used for commercial 
purposes (including rental); (d) the Program is modified or tampered 
with; or (e) the Program's serial number has been altered, defaced 
or removed.  Licensor will replace defective media at no charge as 
set forth above.  This is your sole and exclusive remedy for any 
breach of warranty. 

10.	LIMITATION OF LIABILITY.  YOU ACKNOWLEDGE AND AGREE THAT COMPANY 
AND ITS LICENSORS SHALL NOT ASSUME OR HAVE ANY LIABILITY FOR ANY 
ACTION BY COMPANY OR ITS CONTENT PROVIDERS, OTHER PARTICIPANTS OR 
OTHER LICENSORS WITH RESPECT TO CONDUCT, COMMUNICATION OR CONTENT OF 
THE PROGRAM. COMPANY AND ITS LICENSORS SHALL NOT BE LIABLE FOR ANY 
INDIRECT, INCIDENTAL, SPECIAL, PUNITIVE, EXEMPLARY, OR CONSEQUENTIAL 
DAMAGES RESULTING FROM POSSESSION, USE, OR MALFUNCTION OF THE 
PROGRAM, INCLUDING DAMAGES TO PROPERTY, LOSS OF GOODWILL, COMPUTER 
FAILURE OR MALFUNCTION AND, TO THE EXTENT PERMITTED BY LAW, DAMAGES 
FOR PERSONAL INJURIES, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH 
DAMAGES. EXCEPT AS EXPRESSLY PROVIDED HEREIN, COMPANY'S AND ITS 
LICENSORS' ENTIRE LIABILITY TO YOU AND YOUR EXCLUSIVE REMEDY FOR ANY 
BREACH OF THIS AGREEMENT IS LIMITED SOLELY TO THE TOTAL AMOUNT PAID 
BY YOU FOR THE PROGRAM, IF ANY. BECAUSE SOME STATES DO NOT ALLOW 
THE EXCLUSION OR LIMITATION OF LIABILITY FOR CERTAIN DAMAGES, IN 
SUCH STATES COMPANY'S AND ITS LICENSORS' LIABILITY IS LIMITED TO 
THE EXTENT PERMITTED BY LAW. 

11.	INJUNCTION. Because Company would be irreparably damaged if 
the terms of this License Agreement were not specifically enforced, 
you agree that Company shall be entitled, without bond, other 
security or proof of damages, to appropriate equitable remedies with 
respect to breaches of this Agreement, in addition to such other 
remedies as Company may otherwise have under applicable laws.

12.	INDEMNITY. At Company's request, you agree to defend, indemnify 
and hold harmless Company, its affiliates, contractors, officers, 
directors, employees, agents, licensors, licensees, distributors, 
content providers, and other users of the Program, from all damages, 
losses, liabilities, claims and expenses, including attorneys' fees, 
arising directly or indirectly from your acts and omissions to act 
in using the Program pursuant to the terms of this License Agreement 
or any breach of this License Agreement by you. Company reserves the 
right, at its own expense, to assume the exclusive defense and 
control of any matter otherwise subject to indemnification by you 
hereunder, and in such event, you shall have no further obligation 
to provide indemnification for such matter. 

13.	U.S. GOVERNMENT RESTRICTED RIGHTS. The Program and 
documentation have been developed entirely at private expense and are 
provided as "Commercial Computer Software" or "restricted computer 
software." Use, duplication or disclosure by the U.S. Government or 
a U.S. Government subcontractor is subject to the restrictions set 
forth in subparagraph (c)(1)(ii) of the Rights in Technical Data and 
Computer Software clauses in DFARS 252.227-7013 or as set forth in 
subparagraph (c)(1) and (2) of the Commercial Computer Software 
Restricted Rights clauses at FAR 52.227-19, as applicable. The 
Contractor / Manufacturer is THQ Inc., 27001 Agoura Road, Suite 325, 
Calabasas Hills, CA 91301.

14.	TERMINATION. Without prejudice to any other rights of Company, 
this License Agreement and your right to use the Program may 
automatically terminate without notice from Company if you fail to 
comply with any provision of this Agreement or any terms and 
conditions associated with the Program. In such event, you must 
destroy all copies of this Program and all of its component parts.

15.	GENERAL PROVISIONS. You may not use, copy, modify, sublicense, 
rent, sell, assign or transfer the rights or obligations granted to 
you in this Agreement, except as expressly provided in this 
Agreement. Any assignment in violation of this Agreement is void, 
except that you may transfer your Program to another person provided 
that person accepts the terms of this License Agreement. If any 
provision of this Agreement is held to be unenforceable for any reason, 
such provision shall be reformed only to the extent necessary to 
make it enforceable, and such decision shall not affect the 
enforceability of: (i) such provision under other circumstances, 
or (ii) the remaining provisions hereof under all circumstances. 
Company's failure to enforce at any time any of the provisions of 
this Agreement shall in no way be construed to be a present or future 
waiver of such provisions, nor in any way affect the right of any 
party to enforce each and every such provision thereafter. The express 
waiver by Company of any provision, condition or requirement of this 
Agreement shall not constitute a waiver of any future obligation to 
comply with such provision, condition or requirement. Notwithstanding 
anything else in this Agreement, no default, delay or failure to 
perform on the part of Company shall be considered a breach of this 
Agreement if such default, delay or failure to perform is shown to 
be due to causes beyond the reasonable control of Company. This 
Agreement shall be governed by the laws of the State of California 
and the United States without regard to its conflicts of laws rules 
and you consent to the exclusive jurisdiction of the state and 
federal courts in Los Angeles County, California. The United Nations 
Convention on Contracts for the International Sale of Goods shall 
not apply to this Agreement. This Agreement represents the complete 
agreement concerning this License Agreement between you and Company. 

Red Faction(TM) - © 2001 THQ Inc.  Developed by Volition, Inc.
Uses Bink Video. Copyright (C) 1997-2001 by RAD Game Tools, Inc. 
Red Faction, Geo-Mod(TM) Technology, Volition, THQ and their respective 
logos are trademarks and/or registered trademarks of THQ Inc.
