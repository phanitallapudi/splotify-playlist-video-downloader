
# Spotify to Youtube Video Downloader

This Python script allows you to download YouTube videos for a given playlist of songs fetched from Spotify. It uses the `pytube`, `spotipy`, and `youtubesearchpython` libraries to achieve this functionality.


## Requirements

Before running the script, make sure you have the following:
- Python 3.x
- `pytube` library: To download YouTube videos.
- `spotipy` library: To interact with the Spotify Web API and fetch playlist data.
- `youtube-search-python` library: To search for YouTube videos based on song names.
- Spotify Developer Account: Obtain the required credentials (client_id, client_secret, and redirect_uri) by creating a new Spotify application in the Spotify Developer Dashboard.
```
$ pip install pytube
```
```
$ pip install spotipy
```
```
$ pip install youtube-search-python
```



## How to use
- Install the required dependencies by running:
```bash
pip install pytube spotipy youtube-search-python
```
- Create a Spotify Developer account and obtain the required credentials (Client ID, Client Secret, and Redirect URI) from the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/).
 - Replace the placeholder values client_id_here, client_secret_here, and redirect_url_here in the script with your Spotify application credentials.
 - Run the script using Python:
 ```bash
$ python main.py
 ```
 - When prompted, enter the URL of the Spotify playlist you want to fetch the songs from.
 - The script will fetch the song names from the playlist and search for their corresponding YouTube videos. The highest resolution video for each song will be downloaded and saved in the specified path.
 - The downloaded videos will be saved in the `./videos/` directory by default. You can change the `save_path` variable in the script to modify the download location.


## Output

The script will retrieve the names of songs from the specified playlist and display them on the console in the format: index. song_name.

Note: Make sure the playlist you want to fetch songs from is set to private.

Enjoy exploring your Spotify playlists download songs!

```
$ python main.py 
  
  Enter the url of the playlist you want to: <url here>

  1. "<song_1_name>" with url : "<song_1_url>" downloaded successfully
  2. "<song_2_name>" with url : "<song_2_url>" downloaded successfully
  ....
```
## Disclaimer

Please use this script responsibly and respect the copyrights of the content creators. Make sure to comply with YouTube's Terms of Service and Spotify's Developer Terms.

## Acknowledgement

Happy downloading! If you encounter any issues or have suggestions for improvements, feel free to [open an issue](https://github.com/phanitallapudi/spotify-playlist-video-downloader/issues) or contribute to the project by creating a pull request.