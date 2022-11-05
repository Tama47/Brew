# Brew

### speedtest
```bash
curl ifconfig.me && echo
speedtest --server-id=50679
```

### mpv
```bash
mpv --player-operation-mode=pseudo-gui
```

### ffmpeg
Extract Subs:
```bash
ffmpeg -i subs.ass
```

### yt-dlp
List Formats:
```bash
yt-dlp -F 
```
List Subtitles:
```bash
yt-dlp --list-subs 
```
Download Subs Only:
```bash
yt-dlp --skip-download --write-sub 
```
Download from a list:
```bash
yt-dlp --embed-thumbnail -a list.txt
```
Download Video and Subs:
```bash
yt-dlp --write-sub --embed-thumbnail 
```
Download Video and Embed Subs:
```bash
yt-dlp --embed-subs --embed-thumbnail 
```
Download Thumbnail Only:
```bash
yt-dlp --skip-download --embed-thumbnail 
```
Download Audio Only (MP3):
```bash
yt-dlp --extract-audio --audio-format mp3 
```
Download Best Video and Audio (MP4):
```bash
yt-dlp --embed-thumbnail -f "bestvideo[ext=mp4]+bestaudio[ext=m4a]" 
```
