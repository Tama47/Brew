# Brew

### speedtest
```bash
curl ifconfig.me && echo
speedtest --server-id=50679
```

### mpv
mpv ytdl
```bash
mpv --slang=en-US 
```
Open mpv:
```bash
mpv --slang=en-US --player-operation-mode=pseudo-gui
```

### ffmpeg
Extract Subs:
```bash
ffmpeg -i subs.ass
```

### yt-dlp
Download Video:
```bash
yt-dlp 
```
List Format:
```bash
yt-dlp -F 
```
List Subs:
```bash
yt-dlp --list-subs 
```
Download Audio:
```bash
yt-dlp --extract-audio --audio-format mp3 
```
Download Video and Subs:
```bash
yt-dlp --write-sub --sub-langs en-US --sub-format ass 
```
Download Video and Embed Subs:
```bash
yt-dlp --embed-subs --sub-langs en-US --sub-format ass 
```
Download Subs Only:
```bash
yt-dlp --skip-download --write-sub --sub-langs en-US --sub-format ass 
```
Download Best Youtube Video and Audio
```bash
yt-dlp -f "bestvideo[ext=mp4]+bestaudio[ext=m4a]" --embed-thumbnail --add-metadata 
```
Download from list:
```bash
yt-dlp --write-sub --sub-langs en-US --sub-format ass -a /Users/tama/Documents/list.txt
```
