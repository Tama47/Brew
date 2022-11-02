# Brew

### speedtest
```bash
curl ifconfig.me && echo
speedtest --server-id=50679
```

### mpv
```bash
mpv --ytdl-raw-options=cookies=crunchyroll.txt --slang=en-US 
```
Open mpv:
```bash
mpv --player-operation-mode=pseudo-gui
```

### ffmpeg
Extract Subs:
```bash
ffmpeg -i subs.ass
```

### yt-dlp
Download Video:
```bash
yt-dlp --cookies crunchyroll.txt 
```
List Subs:
```bash
yt-dlp --cookies crunchyroll.txt --list-subs 
```
Download Video and Subs:
```bash
yt-dlp --cookies crunchyroll.txt --write-sub --sub-langs en-US --sub-format ass 
```
Download Video and Embed Subs:
```bash
yt-dlp --cookies crunchyroll.txt --embed-subs --sub-langs en-US --sub-format ass 
```
Download Subs Only:
```bash
yt-dlp --cookies crunchyroll.txt --skip-download --write-sub --sub-langs en-US --sub-format ass 
```
Download Best Youtube Video and Audio
```bash
yt-dlp --merge-output-format mp4 -f "bestvideo+bestaudio[ext=m4a]/best" --embed-thumbnail --add-metadata 
```
