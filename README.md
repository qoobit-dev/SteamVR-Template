# SteamVR-Template
I propose here a Steam VR Template. It's a work in progress and I would like very much that we all contribute to.

I've included the final Vive controllers, with the animated triggers. Just drag and drop the Vive_Pawn in your game and voilà!

Files can be found at https://onedrive.live.com/redir?resi...t=folder%2czip

To install, just unzip into the appropriate Templates directory like C:\Program Files\Unreal Engine[Version]\Templates for launcher version or [ForkLocation]\UE4\Templates for source version. Launch a new project, and you'll find it in the blueprint section.

Templates are always tested on 2 different systems before uploading. It works.

As seen in other threads, there is currently a bug in multiplayer (local) mode. We have 2 Vive there but we'll wait until the ticket is resolved before working on multiplayer mode.

Features v1.5
-Animated triggers in both controllers
-Map of all buttons/trackpad on controllers
-Toggle on/off debugging squares of controllers and/or base stations
-Scalability settings
-Finger tracking on trackpad
-Toggle on/off debugging meshes of base stations
-Added animated "grabbing" mesh right hand (will be refined) -- can be used instead of right controller mesh
-Teleportation with trackpad à la The Lab with cylinder validation
-Go/No go teleportation zones
-Force feedback following teleportation (different for each controller)
-Event tick on/off (by default event tick is off -- press upper menu button to enable it)
-Addition of 2 moving platforms for testing purpose: one by simple actor move and another moved by matinee
-Toggable particles system at the 4 chaperone corners and at the center
-Teleportation on platforms is now possible -- without being moved (see bugs)
-Addition of a cone at the tip of the right trigger -- can be rotated
-Desktop resize

Version 1.6 - UE4.11.2: April 20, 2016
New features:
Pickup/release/throw any object on the scene with the controllers
Platforms (simple move & matinee) teleport
“UltraMan” mode
Standing/seated experience switch
2 different ways to teleport
Custom scalability settings for the Vive
3 adorable dogs on cubes to test scalability settings
Lot of cleanup

Default commands:
Teleport with up trackpad (method #1)
Grab/Release objects with trigger
Menu buttons for UltraMan mode on/off
Teleport with trigger (method #2) – it’s better to disable Grab before

General options
Toggle Camera Fade In/Out when teleport
If Fade On, adjust blink time
Standing/seated position
Teleport distance
Toggle right hand visibility

Demo v1.1 at https://youtu.be/BYzwl1n-7gE 
Demo v1.6 at https://youtu.be/GPfywx2ZeN0 

On the groceries list:
-Fade out camera when entering no teleport zone
-Camera passthrough / Tron mode
-Leap motion integration
-Adapt chaperone size to scene / scene to chaperone size (not sure if feasible/pertinent)
-Animated hands meshes (more)
-Teleportation particles system
