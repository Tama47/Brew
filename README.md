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
Extract Subtitles:
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
Download from a list:
```bash
yt-dlp -a list.txt
```
Download Video and Subtitles:
```bash
yt-dlp --write-sub 
```
Download Video and Embed Subtitles:
```bash
yt-dlp --embed-subs 
```
Download Subtitles Only:
```bash
yt-dlp --skip-download --write-sub 
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
yt-dlp -f "bestvideo[ext=mp4]+bestaudio[ext=m4a]" 
```
