# Project Description: YouTube Video Downloader with yt-dlp

This project is a simple yet powerful command-line tool for downloading YouTube videos using the yt-dlp library. It allows users to download videos in various formats and qualities, including HD, and ensures that both video and audio are merged seamlessly using ffmpeg.

With this tool, users can:

*   Download entire YouTube videos or audio-only files.
*   Choose specific resolutions and formats.
*   Automatically merge video and audio streams.
*   Handle playlists and batch downloads with ease.

Built using Python and powered by the robust yt-dlp library, this project is ideal for anyone looking to save YouTube content for offline viewing efficiently



##  Install the necessary tools: 
*   Install python3 
    
```bash  
    sudo apt update && apt-get install python3
    sudo apt install python3-venv
```

## Create a virtual environment :
```bash
    python3 -m venv yt-dlp-env
```

## Activate the environment :
```bash
    source yt-dlp-env/bin/activate
```
## Install yt-dlp inside the virtual environment :
```bash 
    pip install yt-dlp
```

## Install FFmpeg (for merging HD video + audio) :

##### Make sure ffmpeg is installed to merge video and audio automatically
####
```bash
    sudo apt install ffmpeg
```
# 
# 
# Download Audio-Only
##### If you just want the audio 
####
```bash
    yt-dlp -f bestaudio 'https://www.youtube.com/watch?v=VIDEO_ID'
```
####
##### Or convert it directly to MP3
####
```bash
    yt-dlp -f bestaudio --extract-audio --audio-format mp3 'https://www.youtube.com/watch?v=VIDEO_ID'
```

####
####
## Download Best HD Quality Automatically
####
####
```bash 
    yt-dlp -f 'bestvideo[height<=1080]+bestaudio/best[height<=1080]' 'https://www.youtube.com/watch?v=VIDEO_ID'
```
## If You Want to Download in 4K (if available) 
```bash
    yt-dlp -f 'bestvideo[height<=2160]+bestaudio' 'https://www.youtube.com/watch?v=VIDEO_ID'
```




####
#####
#####
## Authors

- [@ChatGPT](https://chatgpt.com)


