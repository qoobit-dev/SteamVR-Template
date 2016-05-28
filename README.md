Steam VR Template

.pdf version on the onedrive
Hi everybody
I propose here a Steam VR Template. It's a work in progress and I would like very much that we all contribute to.

I've included the final Vive controllers, with the animated triggers. Just drag and drop the Vive_Pawn in your game and voilà!

Files can be found at https://onedrive.live.com/redir?resi...t=folder%2czip

From version 1.5, files can also be found on github at https://github.com/ProteusVR/SteamVR-Template (you need to be logged to Github to open the link) 

To install, just unzip into the appropriate Templates directory like C:\Program Files\Unreal Engine[Version]\Templates for launcher version or [ForkLocation]\UE4\Templates for source version. Launch a new project, and you'll find it in the blueprint section.

Templates are always tested on 2 different systems before uploading. It works.

Eternal thanks: The goal of this template is to put together a noob-proof SteamVR pawn to drop in your scene. However, one size for all solutions will not answer to all specific implementations, but it can gives you a head start. The template will be updated regularly with Unreal forum contributors suggestions. My eternal thanks to (but not only) mitchemmc for input maps and controllers mapping and PenguinTD for amongst many functions , teleportation method #2 and Ultraman.

All assets are whether homemade, from the public domain or from Epic demos (you can use them freely in UE4 projects).

Features of 1.7 – UE4.11.2: April 28, 2016
-Animated triggers in both controllers
-Map of all buttons/trackpad on controllers
-Toggle on/off debugging squares of controllers and/or base stations
-Toggle on/off debugging meshes of base stations
- 2 different ways to teleport
- Ghost move
- Basic vehicle (early version)
-Scalability settings for Vive
-Finger tracking on trackpad
-Trace line with trigger
-Force feedback
-3 adorable dogs on cubes to test scalability settings
-Conductor’s baton to test grabbing
-Added animated "grabbing" mesh right hand (will be refined) -- can be used instead of right controller mesh
-Teleportation with trackpad à la The Lab with cylinder & particles validation
-Go/No go teleportation zones with camera fade out
-Addition of 2 moving platforms for testing purpose: 
one by simple actor move (embark/disembark by triggering overlap volume)
one by matinee (press left menu button to embark & move and to stop platform)
-Toggable particles system at the 4 chaperone corners and at the center
-Addition of a cone at the tip of the right trigger -- can be rotated
-“UltraMan” mode
Standing/seated experience switch

General settings (found in Vive folder)
Transportation Method: 0=Room-scale only; 1=Teleport with trackpad; 2=Teleport with trigger & Trackpad; 3= Ghost move
Standing or Seated Experience: 0=Standing; 1=Seated
Blink Time: Blink Time (in seconds) during teleportation (0=none)
Right Hand Visibility: Toggle Right Controller / Right Hand
Spawn Particles at Chaperon Corners: Yes/No

Scalability settings (found in level blueprint)
The sg ones is in fact a group of r settings. For a thorough explanation see https://docs.unrealengine.com/latest...nce/index.html
Specifically for VR, visit also http://www.tomlooman.com/getting-started-with-vr/

FXAA is less ressource hungry, provides crisper images but there still some aliasing
TempAA is ressource-intensive, provides images that are bit blurrier but removes all aliasing
Personnaly, I prefer the look of tempAA, even if farther textures are a bit blurry. I found the sweet spot between ressource/usage and image quality is a screen percentage of 150. I can crack it up a bit but over 175 a begin to have serious drops in FPS (in tempAA). Note that the sweet spot can vary between rigs. Note that for textures within let's say 2-3 m I don't see any differences between settings, they are all super crisp.
Other settings like adjusting streaming poolsize and setres should be tailored accordingly to your GPU VRAM and main monitor res

Default inputs
Teleport with up trackpad (method #1)
Teleport with trigger and up trackpad (method #2)
Move with trackpad (Ghost mode)
Left menu button for Matinee platform embark/disembark
Right Menu button for UltraMan mode on/off
Step near the vehicle to take possession / control with left trackpad/disembark with right menu button

Inactivated features at start (need input mapping):
Toggle Base Stations Debug Boxes
Toggle Base Stations Meshes
Cone Rotation at tip of controller
Force feedback

On the groceries list
-Reliable grab function + objects/tools/weapons to test
-Initial spawn on playerstart
-Customizable avatar
-Interactive menus
-Camera passthrough / Tron mode
-Leap motion integration
-Adapt chaperone size to scene / scene to chaperone size (not sure if feasible/pertinent)
-Animated hands meshes (more)
-Teleportation particles system
-Multiplayer

Changelog
Version 1.1 - UE4.11.0: April 6, 2016 (project files)
-Animated triggers in both controllers
-Map of all buttons/trackpad on controllers
-Toggle on/off debugging squares of controllers and/or base stations
-Scalability settings

Version 1.2 - UE4.11.1: April 7, 2016 (project files)
-More precise animated triggers in both controllers

Version 1.3 - UE4.11.1: April 10, 2016 -- now as a template!
-Finger tracking on trackpad
-Trace line with trigger
-Teleportation with cone validation
-Toggle on/off debugging meshes of base stations
-Force feedback

Version 1.4 - UE4.11.1: April 13, 2016
-Added animated "grabbing" mesh right hand (will be refined) -- can be used instead of right controller mesh
-Teleportation with trackpad à la The Lab with cylinder validation
-Go/No go teleportation zones
-Force feedback following teleportation (different for each controller)

Version 1.5 - UE4.11.1: April 14, 2016
-Reduced recourse to event tick
-Event tick on/off (by default event tick is off -- press upper menu button to enable it)
-Addition of 2 moving platforms for testing purpose: one by simple actor move and another moved by matinee
-Toggable particles system at the 4 chaperone corners and at the center
-Teleportation on platforms is now possible -- without being moved (see bugs)
-Addition of a cone at the tip of the right trigger -- can be rotated
-Added the right hand grip fbx on the onedrive -- will be refined
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

Version 1.7 – UE4.11.2: April 28, 2016
- Added Settings Menu
- Added Ghost move
- Added particles system with teleportation method 1
- No go teleportation zones with camera fade out
- Basic vehicle (early version): Step near the vehicle to take possession / control with left trackpad/disembark with menu buttons
- Fixed the 2 moving platforms for testing purpose: 
one by simple actor move (embark/disembark by triggering overlap volume)
one by matinee (press left menu button to embark & move and to stop platform)

Next iteration v1.8:
- I’m amazed by mordentral plugin, and if he doesn’t mind I’ll put it along the template when he’ll release it. I’ll put also objects/tools/weapons along to try picking up things. The reason why I will not use environments like the stylized low poly one on the marketplace is this template is open-source and doesn’t include any copyrighted assets. 
- Fixed vehicle
- Inclusion of Vive_Character
- Vive_pawn and Vive_Character spawn on PlayerStart
