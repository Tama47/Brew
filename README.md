# Brew

### speedtest
```bash
curl ifconfig.me && echo
speedtest --server-id=50679
```

### mpv
mpv ytdl
```bash
mpv --ytdl-raw-options=cookies-from-browser=chrome --slang=en-US 
```
Open mpv:
```bash
mpv --ytdl-raw-options=cookies-from-browser=chrome --slang=en-US --player-operation-mode=pseudo-gui
```

### ffmpeg
Extract Subs:
```bash
ffmpeg -i subs.ass
```

### yt-dlp
Download Video:
```bash
yt-dlp --cookies-from-browser chrome 
```
List Subs:
```bash
yt-dlp --cookies-from-browser chrome --list-subs 
```
Download Video and Subs:
```bash
yt-dlp --cookies-from-browser chrome --write-sub --sub-langs en-US --sub-format ass 
```
Download from list:
```bash
yt-dlp --cookies-from-browser chrome --write-sub --sub-langs en-US --sub-format ass -a /Users/tama/Documents/list.txt
```

Download Video and Embed Subs:
```bash
yt-dlp --cookies-from-browser chrome --embed-subs --sub-langs en-US --sub-format ass 
```
Download Subs Only:
```bash
yt-dlp --cookies-from-browser chrome --skip-download --write-sub --sub-langs en-US --sub-format ass 
```
Download Best Youtube Video and Audio
```bash
yt-dlp --cookies-from-browser chrome -f "bestvideo[ext=mp4]+bestaudio[ext=m4a]" --embed-thumbnail --add-metadata 
```
Download Audio:
```bash
yt-dlp --cookies-from-browser chrome --extract-audio --audio-format mp3 
```
