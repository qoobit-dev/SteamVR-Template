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

Demo v1.1 at https://youtu.be/BYzwl1n-7gE 

Bugs
Debugging squares of controllers and base stations do not follow after teleportation
Cannot be moved while on moving platforms
While teleportation and interaction with meshes works, it seems that the SceneRoot (initially at 0,0,0) doesn't move with the pawn. The previous 2 bugs probably are the result of this discrepancy.
Fading camera when clipping through no go zones (i.e. walls) will result in system crash -- whether UE4 or entire system (reboot) -- beware!
Pickup doesn't work yet

Also on the groceries list:
-Camera passthrough / Tron mode
-Leap motion integration
-Adapt chaperone size to scene / scene to chaperone size (not sure if feasible/pertinent)
-Animated hands meshes (more)
-Teleportation particles system
