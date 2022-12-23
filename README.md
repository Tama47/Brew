# Brew

### mpv
```bash
mpv --player-operation-mode=pseudo-gui
```
```bash
mpv --sub-delay=-5.098667 
```
Upscale with Anime4K Mode A for lower-end GPU:
```bash
mpv input.mp4 \
--glsl-shaders="~~/shaders/Anime4K_Clamp_Highlights.glsl:~~/shaders/Anime4K_Restore_CNN_M.glsl:~~/shaders/Anime4K_Upscale_CNN_x2_M.glsl:~~/shaders/Anime4K_AutoDownscalePre_x2.glsl:~~/shaders/Anime4K_AutoDownscalePre_x4.glsl:~~/shaders/Anime4K_Upscale_CNN_x2_S.glsl" \
--vf=gpu -vf scale=3840:2160 --o=output.mp4
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
Extract Subtitles:
```bash
ffmpeg -i  ~/Downloads/eng.ass
```
Convert Video to MP3:
```bash
ffmpeg -i  ~/Downloads/theme.mp3
```
Trim Subtitles:
```bash
ffmpeg -i  -ss  -to  ~/Downloads/eng.ass
```
Trim Video (no encode):
```bash
ffmpeg -i  -ss  -to  -c copy ~/Downloads/output.mp4
```
Trim Video (re-encode):
```bash
ffmpeg -i  -ss  -to  -async 1 ~/Downloads/output.mp4
```
