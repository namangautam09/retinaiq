# Process Live video

Paste the demo video here (any file name), then run `python main.py export-static` again.

- Format: .mp4 (H.264) plays everywhere; .webm also works. Convert a .mov first.
- Size: under 25 MB (Cloudflare Pages file limit). To shrink or convert:
  ffmpeg -i IN -vcodec libx264 -crf 28 -preset slow -movflags +faststart -an OUT.mp4
- Optional: a .jpg/.png here is used as the poster frame shown before the video plays.
