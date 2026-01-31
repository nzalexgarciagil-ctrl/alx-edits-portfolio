# Video Setup Instructions

## Current Status ✅

Your portfolio now has:
1. **Compact Navigation Bar** - Logo hides when scrolling down, navigation links remain visible
2. **Improved Spacing** - Reduced gap between hero/award section and featured work
3. **HTML5 Video Structure** - Ready to accept video files with Instagram fallbacks

## Next Steps: Adding Instagram Videos

Since GitHub API cannot upload binary video files, you'll need to add the videos manually. Here's how:

### Method 1: Download Instagram Videos (Recommended)

#### Tools to Download Instagram Reels:
1. **SnapInsta** (https://snapinsta.app/)
   - Paste Instagram reel URL
   - Click "Download"
   - Save as MP4

2. **Instagram Video Downloader** (https://igram.io/)
   - Paste reel URL
   - Download video

3. **4K Video Downloader** (Desktop App)
   - Free software for Mac/Windows
   - Can download multiple videos

### Videos to Download:

1. **Giltrap Porsche**: https://www.instagram.com/reel/DIPWWsYzTCL/
   - Save as: `giltrap-porsche.mp4`
   
2. **Mad Soundz Racing**: https://www.instagram.com/reel/DTRqIr_AoI4/
   - Save as: `mad-soundz-racing.mp4`
   
3. **Dspec Racing**: https://www.instagram.com/reel/DLstV4GT6Vp/
   - Save as: `dspec-racing.mp4`
   
4. **RX7 Cinematic**: https://www.instagram.com/reel/DI7QiJNz86c/
   - Save as: `rx7-cinematic.mp4`

### Method 2: Add Videos to Repository

#### Option A: Using GitHub Web Interface

1. Go to your repository: https://github.com/nzalexgarciagil-ctrl/alx-edits-portfolio
2. Click "Add file" → "Create new file"
3. Type `videos/.gitkeep` to create the videos folder
4. Commit the file
5. Navigate to the `videos` folder
6. Click "Add file" → "Upload files"
7. Drag and drop your 4 video files
8. Commit the changes

#### Option B: Using Git Command Line

```bash
# Clone repository
git clone https://github.com/nzalexgarciagil-ctrl/alx-edits-portfolio.git
cd alx-edits-portfolio

# Create videos folder
mkdir videos
cd videos

# Move your downloaded videos here
# Then add and commit
git add .
git commit -m "Add portfolio videos"
git push
```

### Method 3: Optional - Create Poster Images

For better loading experience, create poster/thumbnail images:

1. Take a screenshot from each video at an interesting frame
2. Save as JPG (keep file size under 200KB)
3. Name them:
   - `giltrap-porsche-poster.jpg`
   - `mad-soundz-poster.jpg`
   - `dspec-racing-poster.jpg`
   - `rx7-cinematic-poster.jpg`
4. Upload to the `videos` folder

### File Structure After Setup:

```
alx-edits-portfolio/
├── index.html
├── styles.css
├── videos/
│   ├── giltrap-porsche.mp4
│   ├── giltrap-porsche-poster.jpg (optional)
│   ├── mad-soundz-racing.mp4
│   ├── mad-soundz-racing-poster.jpg (optional)
│   ├── dspec-racing.mp4
│   ├── dspec-racing-poster.jpg (optional)
│   ├── rx7-cinematic.mp4
│   └── rx7-cinematic-poster.jpg (optional)
└── VIDEO_SETUP_INSTRUCTIONS.md
```

## How the Fallback System Works

The site is smart:
- **If videos are present**: HTML5 video players will show
- **If videos are missing**: Instagram embeds will display automatically
- **Both work**: Users can watch embedded videos OR click "View on Instagram"

## Video Optimization Tips

### Compress Videos for Web:
- **Max file size**: 10-20 MB per video
- **Resolution**: 1080p (1920x1080) is ideal
- **Format**: MP4 with H.264 codec
- **Tools**:
  - HandBrake (free, desktop)
  - Online: CloudConvert, Clideo
  - FFmpeg command: 
    ```bash
    ffmpeg -i input.mp4 -vcodec h264 -acodec aac -b:v 2M output.mp4
    ```

## Testing

After adding videos:
1. Visit your Vercel site
2. Scroll down to check navigation compact feature ✅
3. Check video players appear
4. Verify fallback to Instagram embeds if videos don't load
5. Test on mobile devices

## Troubleshooting

### Videos not showing?
- Check file names match exactly (case-sensitive)
- Verify videos are in `/videos/` folder
- Check video format is MP4
- Ensure videos are committed and pushed to GitHub
- Wait for Vercel to rebuild (automatic, ~1-2 minutes)

### Instagram embeds not loading?
- Clear browser cache
- Check internet connection
- Instagram embeds require JavaScript enabled

## Features Implemented ✅

1. ✅ **Navigation scroll detection** - Logo hides on scroll
2. ✅ **Improved spacing** - Reduced hero to work section gap
3. ✅ **HTML5 video structure** - Ready for video files
4. ✅ **Instagram fallbacks** - Shows Instagram embeds if videos missing
5. ✅ **Responsive design** - Works on all devices
6. ✅ **Performance optimized** - Throttled scroll events
7. ✅ **Smooth animations** - Professional transitions

## Need Help?

If you encounter issues:
1. Check Vercel deployment logs
2. Inspect browser console for errors (F12)
3. Verify file paths and names
4. Test with a single video first

---

**Note**: The current site is fully functional with Instagram embeds. Adding videos is optional but recommended for better performance and user experience.