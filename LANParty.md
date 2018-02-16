# LAN Party Documentation

I've put this document together to help get you started running a LAN party in either the UNIX or Systems Lab (a.k.a. Syslab).
This covers some general things, as well as the setup for a few spesific games. If you have any questions, please contact qrb2.

## General Setup
If you're hosting a LAN party, I'd reccomend showing up at least 30 minutes beforehand. An hour is even better. In the UNIX lab, use the Teacher's station (Stallman) at the front of the room. In the Syslab, use station 24. Note that in the Syslab you will need to plug in the thick VGA cable dropping from the ceiling by the projector screen if you want to use the projector (Station 24 should have an adapter plugged in for VGA at the get-go).

Log in to the Windows image; unless you are feeling adventurous and want to try running PC games in Linux...

I store games in my home (S:) drive. Unfortunately, to share them, you will need to copy the files/folder to the local machines "Thawspace0" (W:) drive, then enable sharing. To do this, right-click on the folder or file (I usually put all the games under one 'games' folder) and click properties. In the dialogue box that opens, select the Sharing tab, then click on the "Share..." button. In the box that opens, type "everyone" into the search prompt, and click "Share". The window should then show a confirmation, with the file and the path to access it from other machines in the room (it will look something like \\\\MACHINE_NAME\\FOLDER) .

As of Feb 2018, I have most games shared in the UNIX lab at \\\\STALLMAN\\games, and in the Syslab at \\\\SYSLAB24\\games.

## Artemis Setup
In the games folder, there is a folder called "Artemis". Have LAN party participants copy the Artemis folder to their local desktop, then use the Artemis.exe file inside it to launch the game.

DO NOT RUN THE SHARED COPY DIRECTLY. This will cause crashes/instability with the game if everyone tries this.

When you are ready, click "start server" on your station. NOTE THAT THE IP SHOWN WILL *PROBABLY* BE INCORRECT. To find the *correct* port, you will need to use the "ipconfig" command in cmd. (In the Syslab, you will want to use the IP address listed for Ethernet Adapter Ethernet 2, which will be something like 153.106.116.x).

Write the IP on the board or share it with people however works best. From here on out, you should be able to play the game without any additional tweaks.

## KTANE Setup

This is pretty straightforward. Just run the KTANE executable stored in the games folder on your machine, and communicate verbally with your teammates. You can print out or get copies of the "bomb defusal manual" from qrb2 beforehand.

## League Setup

I have downloaded and installed a full copy of LoL directly to the (W:) drive on SYSLAB24. Instruct users to copy the "Riot Games" folder directly to the top level of their (C:) drives, then run the game by using the LeagueClient.exe application in the folder.

Note that many people copying this at the same time will SEVERELY congest the network, as it is over 8.0GB of files. I'd reccomend having two or three people copy, then another 2 or 3, and so on. You could also just invite people to download a copy from the LoL site or use their own laptops.


