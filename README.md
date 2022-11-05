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
List Format:
```bash
yt-dlp -F 
```
List Subs:
```bash
yt-dlp --list-subs 
```
Download from list:
```bash
yt-dlp -a list.txt
```
Download Video and Subs:
```bash
yt-dlp --write-sub 
```
Download Video and Embed Subs:
```bash
yt-dlp --embed-subs 
```
Download Subs Only:
```bash
yt-dlp --skip-download --write-sub 
```
Download Audio:
```bash
yt-dlp --extract-audio --audio-format mp3 
```

Download Best Youtube Video and Audio
```bash
yt-dlp -f "bestvideo[ext=mp4]+bestaudio[ext=m4a]" 
```
