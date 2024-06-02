# Adding Your Own Music to True Music Mod

## Singleplayer Instructions

### Step-by-Step Guide

1. **Video Tutorial:**
   Watch the video tutorial for a visual guide: [YouTube Tutorial](https://youtu.be/9DZghSBPOy4)

2. **Locate the Music Folder:**
   Navigate to the directory:
   `\workshop\content\108600\2613146550\mods\True Music\media\yourMusic`

3. **Extract Music Files:**

- Extract the contents of `yourMusic.rar` or `yourMusic.zip`.
- If your file is named `yourMusic.zi`, rename it to `yourMusic.zip` before extraction.
- Extract the files to the `yourMusic` folder.

4. **Place Audio Files:**

- Put your audio files (mp3, wav, ogg) into the appropriate folders:
  - `TCBoombox`
  - `TCVinylplayer`

5. **Optional: Add Vinyl Cover Photos:**

- Place jpg cover photos in the `TCVinylplayer` folder.
- The cover photo should have the same name as the music track file.
- Example:
  - Track file: `AC DC - Highway To Hell (1979).mp3`
  - Cover file: `AC DC - Highway To Hell (1979).jpg`
- You can find cover images by searching: `"AC DC - Highway To Hell vinyl cover"`

6. **Run the Converter:**

- Run `AddYourMusicToTheMod.exe`.
- Depending on the folder where the files are placed, either a cassette or vinyl will be generated.

7. **In-Game:**

- Your cassettes and vinyl records will start spawning in the game world. You'll need to find them while playing.

## Multiplayer Instructions

### Step-by-Step Guide

1. **Video Tutorial:**
   Watch the video tutorial for a visual guide: [YouTube Tutorial](https://youtu.be/b7SUjPzmgfM)

2. **Create a New Mod:**

- Use the template to create a new mod: [Mod Template](https://disk.yandex.com/d/iS8o8ZxnV7UxLA)

3. **Modify `mod.info`:**

- Change the ID to your own in the `mod.info` file.

4. **Rename Files to Avoid Conflicts:**

- To prevent conflicts with other True Music addons, rename the following files by adding your mod Workshop ID to their names:
  ```
  media\lua\server\Items\TCGLoadingTCBoombox.lua
  media\lua\server\Items\TCGLoadingTCVinylplayer.lua
  media\lua\shared\TCGMusicDefenitionsTCBombox.lua
  media\lua\shared\TCGMusicDefenitionsTCVinylplayer.lua
  media\scripts\TCGMusicScriptTCBoombox.txt
  media\scripts\TCTCGMusicScriptTCVinylplayer.txt
  media\scripts\TCGSoundsTCBombox.txt
  media\scripts\TCGSoundsTCVinylplayer.txt
  ```
  - Example with Workshop ID:
    ```
    media\lua\server\Items\TCGLoadingTCBoombox2722332157.lua
    media\lua\server\Items\TCGLoadingTCVinylplayer2722332157.lua
    media\lua\shared\TCGMusicDefenitionsTCBombox2722332157.lua
    media\lua\shared\TCGMusicDefenitionsTCVinylplayer2722332157.lua
    media\scripts\TCGMusicScriptTCBoombox2722332157.txt
    media\scripts\TCTCGMusicScriptTCVinylplayer2722332157.txt
    media\scripts\TCGSoundsTCBoombox2722332157.txt
    media\scripts\TCGSoundsTCVinylplayer2722332157.txt
    ```

5. **Distribute the Mod:**

- Send the mod to all users on the server. You are allowed to publish a mod created from the template.

6. **Uploading to Workshop:**

- If you want to upload your mod to the Workshop, delete the following folders and files:
  ```
  \media\yourMusic\audioConverter
  \media\yourMusic\pictureConverter
  \media\yourMusic\AddYourMusicToTheMod.exe
  \media\yourMusic\DeleteYourMusicFromTheMod.exe
  ```

## Additional Tools

- **YouTube Playlist Downloader:**
  Download music from YouTube playlists using this tool: [GitHub Repository](https://github.com/shaked6540/YoutubePlaylistDownloader?tab=readme-ov-file)
