# Recomp Splatterhouse 2010 REMASTER (Xbox360 ver.) on PC!

FINAL - RELEASE TODAY!

My goal was to create something that feels less like a simple recompiler and more like a full-fledged Remaster—a version that, if it ever needs a patch, would only require a minor one.

I’ll record some new videos soon to clearly show what has changed during this time.

NEW VIDEO !
https://www.youtube.com/watch?v=eyB5PLZPbBc

Take my word for it: if it seems like the video is lagging, it’s all BECAUSE OF OBS! ^_^

The video shows the bulk of the work that has been done.
As I mentioned, my PC is weak—you can even see in the video that OBS is consuming MORE resources than the game itself ^_^. I put a huge amount of effort into achieving this result; the whole process took me a month! It’ll be released in a couple of days.

The recompiler itself will be available (TODAY!)

I ran it and played it on a system with a 1050 Ti, an i5-2550K, and 24 GB of RAM; I’m sure many people have better PCs, but if it worked for me, it should work for others too.

I’m not great at making posts look fancy, so I’ll just stick to the facts -_-

#Quick start / Installation instructions (what you need to do)

1)Download the release and extract it anywhere.
<img width="931" height="367" alt="image" src="https://github.com/user-attachments/assets/8dcdcd8f-90e6-40d1-a8a3-213502113981" />

2)Next, you need to unpack ISO (I promised that there would be no restrictions based on game version, region, etc.; you simply need to obtain a WORKING game image in the language you want and unpack it) game files to obtain the asset files containing the game content:
$SystemUpdate
data
AvatarAssetPack
default.xex
nxeart
DLC
<img width="698" height="254" alt="image" src="https://github.com/user-attachments/assets/16701d01-0039-4353-a970-f864db86e85d" />
3)Once all the files are in one place, launch the application and adjust the settings to your preference (you can change the launcher's language in the corner!). Then, click "Save and Play." If you wish to make any changes later, please do so via the launcher; otherwise, the executable file functions independently.

P.S. I have a pre-configured build, though it is in Russian only. However, I’ve set it up so that you can add any other version, provided that the aforementioned files are included. Unfortunately, trying to switch to another language in the build I provided won't make subtitles appear, because they simply aren't there. -_- This is an example of a Russian release.

I will also provide a separate download for the DLC folder; simply unpacking these files into the "Assets" folder isn't enough, as you would also need to generate the `.header` files—something you wouldn't be able to do on your own. The file sizes are quite small: the entire DLC folder is 93.2 MB, while the game image in the "Data" folder is 5.04 GB.
3)Run Launcher.exe (for settings) or splatterhouse.exe and play. The first boot takes a little longer while the shader cache is loaded


#Nuances
1)This is my first project, and I worked on it alone. Please provide constructive criticism. If you encounter an error or issue, please state exactly what you believe the problem is, where it occurred, and—ideally—include a screenshot of the moment it happened, along with the relevant log file. I will do my best to address the issue.
2) F3	Debug overlay (FPS, frame stats) — since any other overlay displays incorrect frame data. Don't use YOUR overlays; they will never tell the truth -_-
3) Alt+Enter or F11 — switch between full-screen and windowed mode.
4) My tester friend assured me that the game works with both a keyboard and mouse, as well as a gamepad. (I do NOT have a gamepad.) The intention was for it to be played using a keyboard and mouse. Just keep that in mind.
5) Cache, logs, and Profile are created automatically within the game folder.
6) Also, you might experience (micro-)stuttering throughout the game; this is due to the cache. I’m not sure how to force the game to generate the entire cache upon its first launch, but once I’ve finished the game, I might include a cache file in the download—that could help mitigate the issue.
7) I’m not sure if it’s okay to include files from a file-sharing service, but these would be ready-to-use archives of a build that I’ve already tested.
To be more precise, I’m referring to a ready-made "assets" archive that you’ll just need to unpack alongside the other files.Which are split into  archives 
<img width="1008" height="191" alt="image" src="https://github.com/user-attachments/assets/a5ba9f1b-2215-4e3f-9765-789a2fde4ce4" />
If that’s not allowed, the most I can do is include the DLC files—otherwise, you won’t have them. You’ll need to place (extract) them into that same 'assets' folder.
The DLC folder will need to be unpacked here (your DLC files will 100% likely not work if they do not have a .header file)
<img width="996" height="342" alt="image" src="https://github.com/user-attachments/assets/22d25103-bb4c-49f6-a481-64e3ab6df185" />

#How do I update from version v# to the new one?

An auto-patch feature is planned for the launcher, but for now, you simply need to download the files and replace the existing ones.


#Current unresolved issues causing difficulties:
1) I cannot change the QTE display—which shows the position of the analog sticks—to show keyboard keys instead. This is practically impossible because, when dumping the textures, the stick position is always captured as a single, static "button" icon, lacking any directional information. Consequently, it is currently not possible to assign four distinct keys (even if I were to create a script that interprets the entire left or right analog stick as a single button press). I will return to addressing this problem after the release.
2) Although I have managed to achieve some optimization, I haven't been able to ensure that the game processes shaders at startup (i.e., during the initial launch). As a result, your first experience with the game might include micro-stutters, which occur because new shaders are being generated on the fly. I will try to address this issue.
3) The game is hard-locked to 30 FPS, meaning I cannot remove this limit. If I were to try, the game would become unstable: objects might disappear, ragdoll physics could behave strangely, and the game speed might fluctuate—running either in slow motion or at double speed. In short, it would make for a very unpleasant playing experience. HOWEVER, I will try to come up with a solution to this problem.
4) I wasn’t happy with the low quality of the textures and shadows in the game; I wanted to improve at least the shadow quality, but it turned out to be a bit more complicated than I’d anticipated. That said, I haven’t abandoned the idea—I’d like to add a quality selection option (low/medium/high) to the launcher, though I’ll likely address this after the release.
