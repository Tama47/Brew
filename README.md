# Brew

### speedtest
```bash
speedtest --server-id=50679
```

### mpv
```bash
mpv --ytdl-raw-options=cookies=crunchyroll.txt --slang=en-US 
```
```bash
mpv --ytdl-raw-options=cookies=hidive.txt --slang=english-subs 
```

### yt-dlp
Download video
```bash
yt-dlp --cookies hidive.txt 
```
```bash
yt-dlp --cookies crunchyroll.txt 
```
```bash
yt-dlp --cookies hidive.txt --list-subs 
```
```bash
yt-dlp --cookies crunchyroll.txt --list-subs 
```
```bash
yt-dlp --cookies crunchyroll.txt --write-sub --sub-langs en-US --sub-format ass 
```
```bash
yt-dlp --cookies crunchyroll.txt --embed-subs --sub-langs en-US --sub-format ass 
```
```bash
yt-dlp --cookies crunchyroll.txt --skip-download --write-sub --sub-langs en-US --sub-format ass 
```
```bash
yt-dlp --cookies hidive.txt --skip-download --write-sub --sub-langs english-subs --sub-format vtt 
```
