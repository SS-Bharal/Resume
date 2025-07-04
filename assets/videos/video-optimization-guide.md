# Video Optimization Guide for GitHub

## Current Issue:
Your video is 34MB, which is large for web hosting and GitHub repositories.

## Optimization Targets:
- **Target Size**: 10-15MB for web
- **Resolution**: 1280x720 (HD) is sufficient
- **Bitrate**: 1-1.5 Mbps for good quality
- **Duration**: Keep under 3 minutes

## Tools for Optimization:

### 1. HandBrake (Free, Cross-platform)
```
Download: https://handbrake.fr/
Settings:
- Format: MP4
- Resolution: 1280x720
- Bitrate: 1000-1500 kbps
- Audio: AAC, 128 kbps
```

### 2. FFmpeg (Command Line)
```bash
ffmpeg -i "Veggie Stoker.mp4" -c:v libx264 -crf 23 -preset medium -c:a aac -b:a 128k -vf scale=1280:720 "veggie-stoker-demo.mp4"
```

### 3. Online Tools:
- **CloudConvert**: https://cloudconvert.com/
- **Online Video Converter**: https://www.onlinevideoconverter.com/
- **Convertio**: https://convertio.co/

## Recommended Settings:
- **Codec**: H.264
- **Resolution**: 1280x720
- **Frame Rate**: 30fps
- **Bitrate**: 1000-1500 kbps
- **Audio**: AAC, 128 kbps
- **Container**: MP4

## Alternative: Use External Hosting
Consider hosting the video on:
- YouTube (unlisted)
- Vimeo
- Google Drive
- Dropbox
- AWS S3

Then embed using iframe or direct link. 