### Prerequisites

1. Ensure you have GitHub CLI installed on your desktop. You can download it from [here](https://cli.github.com/).

### How to Edit This Repository

1. **Fork the Repository**: Click on the "Fork" button at the top right corner of the repository page. This will create a copy of the repository in your GitHub account.

2. **Add/Edit Music**:

   - Follow the tutorial provided by the mod author to convert your music files to the required format. You can find the tutorial [here](https://youtu.be/b7SUjPzmgfM?si=Jknd_C1hbP4IK5Ko&t=45).
   - While on the `dev` branch, ensure that you have removed `.mp3` files after conversion. However, do not remove other folders at this stage.

3. **Stage Changes**: Use the following command to stage your changes:

   ```bash
   git add .
   ```

4. **Commit Changes**: Commit your changes with a descriptive message using the following command:

   ```bash
   git commit -m "<Your commit message here e.g ' Artist Name - Track Title - ADDED'>"
   ```

5. **Push Changes**: Push your changes to your forked repository with the following command:

   ```bash
   git push origin dev
   ```

6. **Switch Branch to Main**: Switch to the `main` branch using the following command:

   ```bash
   git checkout main
   ```

7. **Merge Changes**: Merge your changes from the `dev` branch to the `main` branch using the following command:

   ```bash
   git merge dev
   ```

8. **Update Music Folder**: In the `True Music Addon\Contents\mods\truemusic_addon\media\yourMusic` folder, delete everything except the `TCVinylplayer` and `TCBoombox` sub-folders.

9. **Stage Changes**: Stage your deletion changes using the following command:

   ```bash
   git add .
   ```

10. **Commit Changes**: Commit your deletion changes with a descriptive message using the following command:
    ```bash
    git commit -m "Cleanup"
    ```

Your changes will be reviewed, and upon verification, your pull request will be accepted.

### Additional Sources

- [YouTube Playlist Downloader](https://github.com/shaked6540/YoutubePlaylistDownloader)
- [Steam Workshop - True Music Addon](https://steamcommunity.com/workshop/filedetails/?id=2613146550)
