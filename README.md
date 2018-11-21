# DeepGTAV

This folder contains a number of files used to compile a plugin that enables the control/messaging from the game.  Copy the files from the /bin to the game directory.  If you need to edit the files, use Visual Studio to open DeepGTAV.vcxproj which will load the project.  You can then make changes and build.  The project is configured to automatically place the new files in the game directory.  

Note that these files have been edited to work for our self-driving purposes and is not just a clone of DeepGTA.  Specifically, I changed the time parameter to return the current system time in ms instead of the time in the game.  The system time is used in the RTT calculations.  Also, there are a number of changes to the FOV and spawning code to work better for our purposes.

Once the game starts DeepGTAV will wait for TCP clients to connect on port 8000.

Copy the contents of bin/mods to the GTAV directory
Copy the contents of bin/release to the GTAV directory (overwriting existing files)
