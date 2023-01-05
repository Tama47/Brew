# Brew

### mpv
```bash
mpv --player-operation-mode=pseudo-gui &
```

### speedtest
```bash
curl ifconfig.me && echo
speedtest --server-id=50679
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
yt-dlp --write-sub --skip-download 
```
Download from a list:
```bash
yt-dlp --embed-thumbnail -a list.txt
```
Download Video and Subs:
```bash
yt-dlp --embed-thumbnail --write-sub 
```
Download Thumbnail Only:
```bash
yt-dlp --write-thumbnail --skip-download 
```
Download Audio Only (MP3):
```bash
yt-dlp --extract-audio --audio-format mp3 
```
Download Best Video and Audio (MP4):
```bash
yt-dlp --embed-thumbnail -f "bestvideo[ext=mp4]+bestaudio[ext=m4a]" 
```

### ffmpeg
Input
```bash
ffmpeg -i 
```
Trim
```bash
-ss  -to 
```
Extract Subtitles:
```bash
~/Downloads/eng.ass
```
Convert Video to MP3:
```bash
~/Downloads/theme.mp3
```
Trim Subtitles:
```bash
~/Downloads/eng.ass
```
Trim Video (no encode):
```bash
-c copy ~/Downloads/output.mp4
```
Trim Video (re-encode):
```bash
-async 1 ~/Downloads/output.mp4
```
