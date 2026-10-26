# Recomp Splatterhouse 2010 (Xbox360 ver.)

На завершающей стадии тестов, сейчас делаются улучшения и добавляются в ЛАУНЧЕР.

Currently in the final stage of testing; improvements are being made and added to the LAUNCHER.

TEST - Recomp Splatterhouse 2010 (Xbox 360 ver.)
https://www.youtube.com/watch?v=U16HddhCwrY

Launcher TEST - Recomp Splatterhouse 2010 (Xbox 360 ver.)
https://www.youtube.com/watch?v=_E1lbWy0F1I


Quick start (what you need to do)

Steps
1)Download the release and extract it anywhere. 
You get splatterhouse.exe + Launcher.exe, amd_fidelityfx_dx12.dll + rexgpu-xenos.dll + rexruntime.dll
(optional) splatterhouserecomp.toml my config.
The launcher will generate its own TOML file each time; this is simply a pre-configured, ready-to-use file (it won’t cause any conflicts and can be deleted at any time). It already contains settings for button controls, the texture pool, resolution, FSR, and more. You can adjust all of these settings within the launcher itself.
Cache, logs, and Profile are created automatically within the game folder.
<img width="712" height="358" alt="image" src="https://github.com/user-attachments/assets/976deeea-717d-4804-ab2d-be888fdcfe79" />

2)
Next, you need to unpack the game files to obtain the asset files containing the game content:
$SystemUpdate
data
AvatarAssetPack
default.xex
nxeart
DLC

<img width="698" height="254" alt="image" src="https://github.com/user-attachments/assets/16701d01-0039-4353-a970-f864db86e85d" />

P.S. I have a pre-configured build, though it is in Russian only. However, I’ve set it up so that you can add any other version, provided that the aforementioned files are included.
I will also provide a separate download for the DLC folder; simply unpacking these files into the "Assets" folder isn't enough, as you would also need to generate the `.header` files—something you wouldn't be able to do on your own. The file sizes are quite small: the entire DLC folder is 93.2 MB, while the game image in the "Data" folder is 5.04 GB.

3)
Run Launcher.exe or splatterhouse.exe and play. The first boot takes a little longer while the shader cache is loaded


Nuances
1) F3	Debug overlay (FPS, frame stats) — since any other overlay displays incorrect frame data.
2) Alt+Enter or F11 — switch between full-screen and windowed mode
3) My tester friend assured me that the game works with both a keyboard and mouse, as well as a gamepad. (I do NOT have a gamepad.) The intention was for it to be played using a keyboard and mouse. Just keep that in mind.
