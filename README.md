# SpotiPod
A tool for exporting your Spotify Liked Songs to an iPod.

# Installation

1. Download the script file from the Releases tab and place it in a folder. Preferably named "SpotiPod" - doesn't really matter tho).
2. Go to the [Spotify for Developers Dashboard](https://developer.spotify.com/dashboard) and click "Create App".
3. Set the app name to SpotiPod, the description to *literally anything* and the Redirect URI to "http://127.0.0.1:8000/callback".
4. Select "Web API".
5. Copy your Client ID and Client Secret.
6. Open the SpotiPod python script in *any* text editor.
7. Near the top of the file, change the CLIENT_ID and CLIENT_SECRET to the Client ID + Client Secret from Spotify.
8. Install the browser extenstion [cookies.txt](https://addons.mozilla.org/en-US/firefox/addon/cookies-txt/) (there are Chromium alternatives, but you should be using Firefox anyway).
9. Go to [the YouTube Music website](https://music.youtube.com).
10. Open the newly downloaded cookies.txt extention, and click "Current Site".
11. Save the cookies.txt file in the SpotiPod folder.
12. Run the script.
13. Log in to Spotify in the browser window it creates. If you are already signed in to [Spotify's Website](https://open.spotify.com), the window will skip asking for sign in.

> [!NOTE]
> You may need to regenerate cookies.txt often. 

# Usage

1. When you run the script, after authenticating, you must choose if you want to download the songs or not.
   > [!NOTE]
   > Choosing to not download the songs will ONLY create the liked_songs.csv file, instead of both the CSV and the "music" folder.
2. The script will then proceed in generating the CSV (and downloading the music if asked).
3. After the script is complete, listen to all songs in the "TO_CHECK" folder, and decide which you would like to keep.
4. Import the downloaded songs into iTunes.
