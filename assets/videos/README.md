# Avatar Videos

This directory should contain the video files for the avatar:

## Required Videos

1. `idle.mp4` - The idle state video of the avatar (looping)

## Video Requirements

- Format: MP4
- Resolution: 720p or higher recommended
- Duration: For idle video, a 5-10 second loop works well

## How to Add Videos

1. Place your `idle.mp4` file in this directory
2. The avatar component will automatically use this video for the idle state
3. The talking state video is generated dynamically through the D-ID API

## Placeholder

If you don't have an idle video yet, you can use a static image and convert it to a video:

1. Use a tool like FFmpeg to convert an image to a video:
   ```
   ffmpeg -loop 1 -i your_avatar_image.jpg -c:v libx264 -t 10 -pix_fmt yuv420p idle.mp4
   ```
   This will create a 10-second video from your image.

2. Or use online services that can convert images to videos.