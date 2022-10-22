# Brew

### mpv
```bash
mpv --ytdl-raw-options=cookies=crunchyroll.txt --slang=en-US 
```
```bash
mpv --ytdl-raw-options=cookies=hidive.txt --slang=english-subs 
```

### ffmpeg
Extract Subs:
```bash
ffmpeg -i subs.ass
```

### yt-dlp
Download Video:
```bash
yt-dlp --cookies hidive.txt 
```
```bash
yt-dlp --cookies crunchyroll.txt 
```
List Subs:
```bash
yt-dlp --cookies hidive.txt --list-subs 
```
```bash
yt-dlp --cookies crunchyroll.txt --list-subs 
```
Download Video and Subs:
```bash
yt-dlp --cookies crunchyroll.txt --write-sub --sub-langs en-US --sub-format ass 
```
```bash
yt-dlp --cookies hidive.txt --write-sub --sub-langs english-subs --sub-format vtt 
```
Download Video and Embed Subs:
```bash
yt-dlp --cookies crunchyroll.txt --embed-subs --sub-langs en-US --sub-format ass 
```
```bash
yt-dlp --cookies hidive.txt --embed-subs --sub-langs english-subs --sub-format vtt 
```
Download Subs Only:
```bash
yt-dlp --cookies crunchyroll.txt --skip-download --write-sub --sub-langs en-US --sub-format ass 
```
```bash
yt-dlp --cookies hidive.txt --skip-download --write-sub --sub-langs english-subs --sub-format vtt 
```
Download Best Video and Audio
```bash
yt-dlp --merge-output-format mp4 -f "bestvideo+bestaudio[ext=m4a]/best" --embed-thumbnail --add-metadata 
```
