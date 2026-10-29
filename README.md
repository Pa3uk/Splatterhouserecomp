# Recomp Splatterhouse 2010 (Xbox360 ver.)

Currently in the final stage of testing; If everything goes well, I’ll try to put out a RELEASE in a couple of days.

There are 3 unresolved tasks left that I want to implement (if I can manage the time). Other aspects will be refined after the release. My goal was to create something that feels less like a simple recompiler and more like a full-fledged Remaster—a version that, if it ever needs a patch, would only require a minor one.

I’ll record some new videos soon to clearly show what has changed during this time.

TEST (OLD video!) - Recomp Splatterhouse 2010 (Xbox 360 ver.)
https://www.youtube.com/watch?v=U16HddhCwrY

Launcher TEST (OLD video!) - Recomp Splatterhouse 2010 (Xbox 360 ver.)
https://www.youtube.com/watch?v=_E1lbWy0F1I

NEW VIDEO !
https://www.youtube.com/watch?v=eyB5PLZPbBc
The video shows the bulk of the work that has been done.
As I mentioned, my PC is weak—you can even see in the video that OBS is consuming MORE resources than the game itself ^_^. I put a huge amount of effort into achieving this result; the whole process took me a month! It’ll be released in a couple of days.

The recompiler itself will be available (towards the end of the week!)

I ran it and played it on a system with a 1050 Ti, an i5-2550K, and 24 GB of RAM; I’m sure many people have better PCs, but if it worked for me, it should work for others too.

#Quick start (what you need to do)

1)Download the release and extract it anywhere.
<img width="931" height="367" alt="image" src="https://github.com/user-attachments/assets/8dcdcd8f-90e6-40d1-a8a3-213502113981" />

2)Next, you need to unpack the game files to obtain the asset files containing the game content:
$SystemUpdate
data
AvatarAssetPack
default.xex
nxeart
DLC
<img width="698" height="254" alt="image" src="https://github.com/user-attachments/assets/16701d01-0039-4353-a970-f864db86e85d" />

P.S. I have a pre-configured build, though it is in Russian only. However, I’ve set it up so that you can add any other version, provided that the aforementioned files are included.
I will also provide a separate download for the DLC folder; simply unpacking these files into the "Assets" folder isn't enough, as you would also need to generate the `.header` files—something you wouldn't be able to do on your own. The file sizes are quite small: the entire DLC folder is 93.2 MB, while the game image in the "Data" folder is 5.04 GB.
3)Run Launcher.exe (for settings) or splatterhouse.exe and play. The first boot takes a little longer while the shader cache is loaded


#Nuances

1) F3	Debug overlay (FPS, frame stats) — since any other overlay displays incorrect frame data.
2) Alt+Enter or F11 — switch between full-screen and windowed mode
3) My tester friend assured me that the game works with both a keyboard and mouse, as well as a gamepad. (I do NOT have a gamepad.) The intention was for it to be played using a keyboard and mouse. Just keep that in mind.
4) Cache, logs, and Profile are created automatically within the game folder.
5) Also, you might experience (micro-)stuttering throughout the game; this is due to the cache. I’m not sure how to force the game to generate the entire cache upon its first launch, but once I’ve finished the game, I might include a cache file in the download—that could help mitigate the issue.
6) I’m not sure if it’s okay to include files from a file-sharing service, but these would be ready-to-use archives of a build that I’ve already tested.
To be more precise, I’m referring to a ready-made "assets" archive that you’ll just need to unpack alongside the other files.Which are split into  archives 
<img width="1008" height="191" alt="image" src="https://github.com/user-attachments/assets/a5ba9f1b-2215-4e3f-9765-789a2fde4ce4" />
If that’s not allowed, the most I can do is include the DLC files—otherwise, you won’t have them. You’ll need to place (extract) them into that same 'assets' folder.
The DLC folder will need to be unpacked here (your DLC files will 100% likely not work if they do not have a .header file)
<img width="996" height="342" alt="image" src="https://github.com/user-attachments/assets/22d25103-bb4c-49f6-a481-64e3ab6df185" />

#How do I update from version v# to the new one?

An auto-patch feature is planned for the launcher, but for now, you simply need to download the files and replace the existing ones.
