This guide explains how to run a custom Doom .WAD map using GZDoom.

Prerequisites

Before starting, make sure you have:

GZDoom
A Doom IWAD, such as DOOM.WAD or DOOM2.WAD
Your custom .WAD file

Note: A custom map is usually a PWAD and requires the original game's IWAD to run.

1. Install GZDoom

Download GZDoom and extract the contents of the archive to a directory of your choice.

For example:

C:\Games\GZDoom\

The directory should contain:

C:\Games\GZDoom\
├── gzdoom.exe
└── ...
2. Obtain the Required IWAD

Your custom map may require an original Doom IWAD.

Common examples include:

DOOM.WAD
DOOM2.WAD

If you own Doom or Doom II, you can obtain the appropriate IWAD from your game installation.

Place the required IWAD in the GZDoom directory, or configure GZDoom to locate it.

3. Add Your Custom WAD

Place your custom WAD in the same directory.

For example:

C:\Games\GZDoom\
├── gzdoom.exe
├── DOOM2.WAD
└── mymap.wad
4. Launch the WAD

The simplest method is to drag the custom WAD file onto gzdoom.exe.

Alternatively, you can launch it from the command line.

Open Command Prompt in the GZDoom directory and run:

gzdoom.exe -iwad DOOM2.WAD -file mymap.wad

Replace mymap.wad with the name of your WAD file.

5. Using Multiple Files

GZDoom can load multiple WADs and other supported resource files simultaneously.

For example:

gzdoom.exe -iwad DOOM2.WAD -file map.wad texturepack.wad mod.pk3

The order in which files are loaded can affect how resources are overridden.

Troubleshooting

If the WAD does not launch:

Verify that you have the correct IWAD.
Check whether the WAD was designed for Doom, Doom II, or another compatible game.
Make sure you are using a compatible source port such as GZDoom.
Verify the WAD filename in the command.
Check the WAD's documentation for any required additional files or launch parameters.

Once everything is configured correctly, GZDoom should launch the custom map using the specified IWAD.
