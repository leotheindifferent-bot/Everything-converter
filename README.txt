# Everything Converter

A Windows desktop media converter for common audio, video and still-image formats.

## Download and run

Use `EverythingConverter.exe`. It is a single-file Windows app and does not require Python. The window can be scrolled when it is smaller than the full layout.

## Supported input types

- Video: MP4, M4V, MKV, MOV, AVI, WebM, WMV, FLV, MPEG, MPG, TS, MTS, M2TS, 3GP and GIF
- Audio: MP3, WAV, FLAC, M4A, AAC, OGG, OPUS, WMA, AIFF and AIF
- Images: PNG, JPG/JPEG, WebP, BMP, TIF and TIFF

Available outputs include MP3, WAV, FLAC, M4A, AAC, OGG, OPUS, WMA, AIFF, MP4, MKV, MOV, WebM, AVI, GIF, JPG, PNG, WebP, BMP and TIFF.

Converting a video to an image saves one frame. Converting a still image to a video creates a five-second clip. Audio and image files cannot be converted into a video with sound unless they contain the required media streams. This is a media converter; it does not convert Office documents or archives.

## Options

- **Bitrate preset** controls audio quality for lossy audio formats.
- **Target size per MP3** estimates an MP3 bitrate for the requested size. Final size can vary slightly; very small targets may not be possible for long recordings.
- **Parallel jobs** sets how many separate files are processed at once.
- **Use hardware acceleration** selects an available GPU video encoder for compatible video outputs. Audio conversions remain on the CPU. If the GPU encode fails, the app retries on CPU.
- Hover over controls for short explanations.

## FFmpeg

If FFmpeg is missing, choose **Install FFmpeg…** in the app. It asks before opening a Windows command window and installing the WinGet package `Gyan.FFmpeg` for your Windows user. Follow any prompts in that window. If WinGet is unavailable, install Microsoft's App Installer or get FFmpeg through [the official FFmpeg download page](https://www.ffmpeg.org/download.html).

## Run from source

Python 3.9+ with Tkinter is required. Keep `EverythingConverter.ico` beside `mp4_to_mp3_converter.py` for the window icon, then run:

```powershell
py .\mp4_to_mp3_converter.py
```
