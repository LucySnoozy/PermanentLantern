# PermanentLantern
Permanent Lantern SpEffect - Mirror for Nexus

Installation:

- Download ModEngine2﻿ and extract the .zip file to anywhere you like (preferably not in the Desktop/Download folder. On another driver or inside the game folder works just fine)

- Download this mod, open the .zip file and drag out the event folder into your ModEngine2's mod folder.

- Start the game with launchmod_eldenring.bat and enjoy a permanent lantern.



Installation with Seamless Coop:

Please refer to this guide to use this with Seamless Coop:

https://docs.google.com/document/d/1c0BqWI5WjRx-XkqmJubY9U7cfXfKHwc-uiJDxV3tKOg/edit?usp=sharing



Compatibility:

If the mod you are playing with doesn't come with an event folder, you can just use this with it.

- Otherwise download Dark Script 3 and open the common.emevd.dcx of the mod you are using and add the following:

- Under $Event(0, Default, function() { there is gonna be a bunch of InitializeEvent lines, go to the last one, add a new line and enter this:

﻿﻿//Lantern Event
  InitializeEvent(0, 3665345, 0);

After that scroll all the way to the bottom, add 2 new lines and add this:

//Lantern Event
$Event(3665345, Restart, function() {
SetSpEffect(10000, 3245);
});

Save the file and it should work now with the mod you used.
