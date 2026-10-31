# Recomp Splatterhouse 2010 REMASTER (Xbox360 ver.) on PC!

FINAL - RELEASE !

My goal was to create something that feels less like a simple recompiler and more like a full-fledged Remaster—a version that, if it ever needs a patch, would only require a minor one.

I’ll record some new videos soon to clearly show what has changed during this time.

NEW VIDEO !
https://www.youtube.com/watch?v=PlEoK5pK-70

Take my word for it: if it seems like the video is lagging, it’s all BECAUSE OF OBS! ^_^

Sincerely apologize for the lag during the video recording; OBS was consuming more resources than the game itself—my so-called "tester" decided to take the day off! -_- Regardless, I wanted to show that everything is working as intended: the DLCs, the in-game buttons, and—most importantly—an UNLOCKED, consistent, and stable 60 FPS, where the game doesn't end up running at half or double speed!

The video shows the bulk of the work that has been done.
As I mentioned, my PC is weak—you can even see in the video that OBS is consuming MORE resources than the game itself ^_^. I put a huge amount of effort into achieving this result; the whole process took me a month! It’ll be released in a couple of days.

The recompiler itself will be available (TODAY!)

I ran it and played it on a system with a 1050 Ti, an i5-2550K, and 24 GB of RAM; I’m sure many people have better PCs, but if it worked for me, it should work for others too.

I’m not great at making posts look fancy, so I’ll just stick to the facts -_-

#Quick start / Installation instructions (what you need to do)

1)Download the release and extract it anywhere.
<img width="720" height="309" alt="image" src="https://github.com/user-attachments/assets/40fb0042-888e-45f2-bf96-31c87ce8ed87" />


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

8)Functionality has been verified on an ENG build, which is publicly known as a (PROTOTYPE) Sep 16, 2010 build!
<img width="1359" height="767" alt="image" src="https://github.com/user-attachments/assets/8870dd57-5819-4cec-b61e-88804af2452a" />


#How do I update from version v# to the new one?

An auto-patch feature is planned for the launcher, but for now, you simply need to download the files and replace the existing ones.


#Current unresolved issues causing difficulties:
1) I cannot change the QTE display—which shows the position of the analog sticks—to show keyboard keys instead. This is practically impossible because, when dumping the textures, the stick position is always captured as a single, static "button" icon, lacking any directional information. Consequently, it is currently not possible to assign four distinct keys (even if I were to create a script that interprets the entire left or right analog stick as a single button press). I will return to addressing this problem after the release.
2) Although I have managed to achieve some optimization, I haven't been able to ensure that the game processes shaders at startup (i.e., during the initial launch). As a result, your first experience with the game might include micro-stutters, which occur because new shaders are being generated on the fly. I will try to address this issue.
3) I wasn’t happy with the low quality of the textures and shadows in the game; I wanted to improve at least the shadow quality, but it turned out to be a bit more complicated than I’d anticipated. That said, I haven’t abandoned the idea—I’d like to add a quality selection option (low/medium/high) to the launcher, though I’ll likely address this after the release.

   As for FPS—if you’re told that the author has the FPS counter working and it shows 60 frames, don’t take their word for it; the readings from the game’s built-in debug menu (or recompiler overlay) and those from tools like MSI Afterburner (RivaTuner) are often misleading. Do not take such information seriously until it has been verified.


#Splatterhouse (2010) for PC: Features in the 1.0 Release
Oct 31, 2026 · A brief summary: what works, how it’s structured, and what didn’t make the cut.
1. Port Foundation
• Static recompilation of the Xbox 360 version (using ReXGlue SDK 0.10.0): the game code has been converted into native C++. This is not an emulator.
• D3D12 graphics using ROV mode: replicates the console’s video memory (eDRAM). (The alternative RTV mode resulted in a dark image and only 15–20 FPS.)
• Manual recompilation fixes: several functions missed by the code generator were implemented manually (without them, the 3D scene would remain black); support for compressed .gfx files (XCTD) has been added.
• Portability: game assets, save files (Profile), shaders (Cache), and logs are located alongside the executable. No installation is required; the folder can be moved freely.
• DLC: folders within `assets\DLC` are automatically loaded at startup (masks and arenas have been verified).
• Pre-compiled shader cache included: reduces stuttering during the initial launch.
• Option to skip the logo/intro sequence.
2. Visuals and Graphics
• Borderless full-screen mode (F11 and Alt+Enter) with proper VSync.
• FSR 1 upscaling with various quality presets; independent settings for internal resolution, window resolution, and monitor selection.
• Anisotropic filtering, anti-aliasing, and five texture pool size presets.
• Adjustable sliders for brightness, contrast, saturation, gamma, and FSR sharpness. Bloom (glow from bright light sources) can be toggled on or off. • Field of View (FOV): slider ranging from 50–100, with a default of 73. Values ​​above 85 are unstable; walls and objects may disappear near the edges of the screen.
• F3 Overlay: displays the output frame rate and the game’s internal "guest" frame rate.
3. Frame Rate
• The game is internally capped at 30 FPS. Unlocking it to 60 FPS involves relaxing the internal frame limiter and changing the game logic step from 1/30 to 1/60.
• The launcher includes a "60 FPS (instead of 30)" checkbox. When disabled, the game runs at the original 30 FPS.
• Limitation: Since the logic step is fixed, the game will run slightly slower than normal if the frame rate drops below 60 FPS. A version that dynamically adjusts the logic step based on actual frame time has been written but not yet tested.
4. Controls
• Keyboard and Mouse Mode: the mouse controls the right analog stick, the scroll wheel navigates menus, and the F9 key toggles the cursor’s visibility.
• All buttons can be remapped via the launcher; a dedicated tab provides a visual layout diagram.
• In-game key prompts: Xbox controller icons are replaced with keyboard and mouse equivalents based on your custom key bindings (via texture swapping during load). The full controller diagram in the "Controls" menu has also been updated. Specific icons have been created for WASD, the A/D pair used in the journal, and the down arrow on the D-pad.
• By default, the right analog stick is mapped to Numpad 8 / 5 / 4 / 6.
5. Launcher
• Tabs: Graphics, Display, Controls, Audio, Language, DLC, Debug, Updates, and Layout. • Russian and English interface: a RU/ENG toggle is provided; the default language is determined by the Windows system language.
• All settings are stored in `splatterhouserecomp.toml`. Technical parameters are hidden; the launcher will automatically restore them if they are deleted.
• The in-game language can be selected independently; audio can be muted.
6. Installation, File Verification, and Updates
• Users must extract files from their own game disc image and place them into the `assets` folder (instructions are provided in the README, available in both Russian and English).
• The `default.xex` file is verified via SHA-256 hash upon launching the application and when clicking "Play." If the file belongs to a different version of the game, the launcher will notify the user and prompt them to select the correct file from their disk. It verifies the hash, copies the file, and renames the original as `default.xex.orig`. No external data is downloaded.
• Updates: The launcher checks GitHub Releases for the latest archive (e.g., `SplatterhouseRecomp <version>.zip`), downloads it, verifies the checksum, replaces the existing files, and moves the previous version to a `Backup` folder. Settings, save files, and the `assets` directory remain unaffected. This has been tested for the update from version 0.9 to 1.0.
• Release build: The `make_release.bat` script generates a clean archive (excluding logs, user profiles, and game assets).
7. Exclusions and Limitations
• Shadows remain at a low resolution; the game's configuration files are encrypted, so adjustments would require modifications at the rendering level.
• Ambient Occlusion (AO), HDR, motion blur, and frame generation are not implemented.
• Non-16:9 aspect ratios are displayed with letterboxing/pillarboxing; native widescreen support has not been implemented.
• Quick save/load functionality (F5/F6) is not implemented; mouse clicks within the menu interface are not supported. • The "START" icons and the icons representing a press of the right analog stick—as well as text prompts like "press START"—remain in their console-style format. In QTE sequences, the stick icons do not indicate direction; instead, a yellow arrow is used to show the required direction.
• The size of the key/button icon on the loading screens does not match the size of the icons used elsewhere.
• The primary testing was conducted using the Russian version of the game on a single computer (i5, GTX 1050 Ti).

#RU
Splatterhouse (2010) для ПК: что реализовано в релизе 1.0
31 окт. 2026 г. · краткая сводка по факту: что работает, как устроено и что осталось за бортом
1. Основа порта
• Статическая рекомпиляция Xbox 360-версии (ReXGlue SDK 0.10.0): код игры переведён в нативный C++. Это не эмулятор.
• Графика D3D12 в режиме ROV: воспроизводит видеопамять консоли (eDRAM). Режим RTV давал тёмную картинку и 15–20 FPS.
• Ручные доработки рекомпиляции: несколько функций, пропущенных кодогенератором, дописаны вручную (без них 3D-сцена оставалась чёрной); добавлена поддержка сжатых .gfx-файлов (XCTD).
• Портативность: рядом с exe лежат assets (файлы игры), Profile (сохранения), Cache (шейдеры), logs. Установка не нужна, папку можно перенести.
• DLC: папки из assets\DLC подключаются автоматически при запуске (маски и арены проверены).
• Готовый кэш шейдеров в раздаче: меньше подвисаний при первом запуске.
• Пропуск заставки с логотипами (опция).
2. Картинка и графика
• Полный экран без рамки (F11 и Alt+Enter), настоящий VSync.
• Масштабирование FSR 1 с режимами качества, отдельно внутреннее разрешение, разрешение окна, выбор монитора.
• Анизотропная фильтрация, сглаживание, пять пресетов размера пула текстур.
• Ползунки: яркость, контраст, насыщенность, гамма, резкость FSR. Свечение ярких источников (Bloom) включается и выключается.
• Угол обзора (FOV): ползунок 50–100, по умолчанию 73. Выше 85 нестабильно: по краям экрана могут пропадать стены и объекты.
• Оверлей F3: частота кадров вывода и «гостевая» частота самой игры.
3. Частота кадров
• Внутри игра ограничена 30 кадрами. Разблокировка до 60 FPS: ослаблен внутренний ограничитель кадров и шаг игровой логики изменён с 1/30 на 1/60.
• В лаунчере галочка «60 FPS (вместо 30)». Выключена — оригинальные 30 FPS.
• Ограничение: шаг логики фиксированный, поэтому при просадках ниже 60 FPS игра идёт чуть медленнее обычного. Вариант с подстройкой шага под реальное время кадра написан, но не проверялся.
4. Управление
• Режим «клавиатура и мышь»: мышь управляет правым стиком, колесо листает меню, F9 показывает или прячет курсор.
• Все кнопки переназначаются в лаунчере; на отдельной вкладке есть схема раскладки в виде картинки.
• Подсказки клавиш прямо в игре: иконки кнопок Xbox заменяются на клавиатурные и мышиные в соответствии с вашими назначениями (подмена текстур при загрузке). Полная схема геймпада в меню Controls тоже заменена. Отдельные иконки сделаны для WASD, пары A/D в дневнике и стрелки вниз на крестовине.
• Правый стик по умолчанию на Numpad 8 / 5 / 4 / 6.
5. Лаунчер
• Вкладки: графика, картинка, управление, звук, язык, DLC, отладка, обновления, схема.
• Русский и английский интерфейс: кнопка RU/ENG, язык по умолчанию выбирается по языку Windows.
• Все настройки хранятся в splatterhouserecomp.toml. Технические параметры скрыты, лаунчер сам восстанавливает их, если их удалить.
• Язык игры выбирается отдельно; звук можно отключить.
6. Установка, проверка файлов и обновления
• Игрок сам извлекает файлы из своего образа и кладёт их в assets (инструкция в README, русский и английский текст).
• Проверка default.xex по SHA-256 при открытии лаунчера и при нажатии «Играть». Если файл от другой версии игры, лаунчер объясняет это и предлагает выбрать подходящий файл с диска. Он проверяет хэш, копирует файл и сохраняет прежний как default.xex.orig. Ничего не скачивается.
• Обновления: лаунчер смотрит GitHub Releases, находит самый новый архив вида «SplatterhouseRecomp <версия>.zip», скачивает его, сверяет контрольную сумму, заменяет файлы и сохраняет предыдущую версию в папке Backup. Настройки, сохранения и assets не затрагиваются. Проверено на обновлении 0.9 → 1.0.
• Сборка релиза: make_release.bat собирает чистый архив (без логов, профиля и файлов игры).
7. Не вошло и ограничения
• Тени остаются низкого разрешения: конфигурационные файлы игры зашифрованы, потребуется правка на уровне отрисовки.
• Окружающее затенение (AO), HDR, размытие в движении и генерация кадров не реализованы.
• Режимы не 16:9 показываются с полосами; настоящая поддержка широкоэкранного режима не сделана.
• Быстрое сохранение и загрузка (F5/F6) не реализованы; клики мышью по пунктам меню не работают.
• Иконки START и нажатия правого стика, а также текстовые подсказки вроде «нажмите СТАРТ», остались консольными. В QTE иконки стиков не различают направление: направление показывает жёлтая стрелка.
• Размер иконки клавиши на экранах загрузки не совпадает с остальными.
• Основное тестирование проводилось на русской версии игры и на одном компьютере (i5, GTX 1050 Ti).
