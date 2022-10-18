# Brew

### mpv

mpv --ytdl-raw-options=cookies=crunchyroll.txt --slang=en-US 

mpv --ytdl-raw-options=cookies=hidive.txt --slang=english-subs 

## yt-dlp
```bash
yt-dlp --cookies hidive.txt --list-subs
```
```bash
yt-dlp --cookies hidive.txt --list-subs 
```
yt-dlp --cookies crunchyroll.txt --list-subs 



yt-dlp --cookies crunchyroll.txt --write-sub --sub-langs en-US --sub-format ass 

yt-dlp --cookies crunchyroll.txt --embed-subs --sub-langs en-US --sub-format ass 

yt-dlp --cookies crunchyroll.txt --skip-download --write-sub --sub-langs en-US --sub-format ass 

yt-dlp --cookies hidive.txt --skip-download --write-sub --sub-langs english-subs --sub-format vtt 
