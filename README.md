# ALX.Edits Portfolio Website

Professional automotive videography portfolio for Alex Garcia Gil showcasing high-energy visuals and engaging content.

## 🎬 Features

- **Compact Navigation**: Logo automatically hides when scrolling, keeping navigation links visible
- **Responsive Design**: Optimized for all devices (desktop, tablet, mobile)
- **Glass-morphic UI**: Modern design with blur effects and smooth animations
- **Video Showcase**: HTML5 video support with Instagram fallbacks
- **Client Portfolio**: Showcase of industry-leading clients
- **Contact Section**: Easy-to-reach contact information

## 📂 Project Structure

```
alx-edits-portfolio/
├── index.html          # Main HTML file
├── styles.css          # Stylesheet with responsive design
├── README.md           # This file
└── videos/            # Video files directory (you need to create this)
    ├── giltrap-porsche.mp4
    ├── giltrap-porsche-poster.jpg
    ├── mad-soundz-racing.mp4
    ├── mad-soundz-poster.jpg
    ├── dspec-racing.mp4
    ├── dspec-racing-poster.jpg
    ├── rx7-cinematic.mp4
    └── rx7-cinematic-poster.jpg
```

## 🎥 Adding Video Files

The site is currently using Instagram embeds as fallbacks. To use native HTML5 videos:

### Method 1: Using Online Tools
1. Use a service like [SaveFrom.net](https://savefrom.net/) or [SnapInsta](https://snapinsta.app/)
2. Paste the Instagram Reel URLs:
   - https://www.instagram.com/reel/DIPWWsYzTCL/
   - https://www.instagram.com/reel/DTRqIr_AoI4/
   - https://www.instagram.com/reel/DLstV4GT6Vp/
   - https://www.instagram.com/reel/DI7QiJNz86c/
3. Download videos in MP4 format

### Method 2: Using Browser Extensions
- Install Instagram video downloader extensions (Chrome/Firefox)
- Navigate to each reel and download

### Method 3: Using Command Line (yt-dlp)
```bash
# Install yt-dlp
pip install yt-dlp

# Download videos
yt-dlp https://www.instagram.com/reel/DIPWWsYzTCL/ -o "giltrap-porsche.mp4"
yt-dlp https://www.instagram.com/reel/DTRqIr_AoI4/ -o "mad-soundz-racing.mp4"
yt-dlp https://www.instagram.com/reel/DLstV4GT6Vp/ -o "dspec-racing.mp4"
yt-dlp https://www.instagram.com/reel/DI7QiJNz86c/ -o "rx7-cinematic.mp4"
```

### Adding Files to Repository
1. Create a `videos` folder in your repository root
2. Upload the downloaded MP4 files with these exact names:
   - `giltrap-porsche.mp4`
   - `mad-soundz-racing.mp4`
   - `dspec-racing.mp4`
   - `rx7-cinematic.mp4`

3. **(Optional)** Create poster images (thumbnail screenshots):
   - `giltrap-porsche-poster.jpg`
   - `mad-soundz-poster.jpg`
   - `dspec-racing-poster.jpg`
   - `rx7-cinematic-poster.jpg`

4. Commit and push:
```bash
git add videos/
git commit -m "Add portfolio video files"
git push origin main
```

## 🚀 Deployment

This site is deployed on **Vercel** with automatic deployments:
- Every push to `main` branch triggers a new deployment
- Site automatically rebuilds with new changes
- Typically deploys in 30-60 seconds

## ✅ Recent Updates

- ✅ Compact navigation on scroll (hides logo, keeps links)
- ✅ Fixed spacing between award section and featured work
- ✅ Added HTML5 video structure with Instagram fallbacks
- ✅ Removed "LZ World Tour" from client list
- ✅ Optimized scroll detection with requestAnimationFrame
- ✅ Mobile-responsive navigation improvements

## 🎨 Design Features

- **Color Scheme**: Black background with electric blue (#0066ff) accents
- **Typography**: System fonts for optimal performance
- **Animations**: Smooth transitions and fade-in effects
- **Glass-morphism**: Frosted glass effects on cards and navigation

## 📱 Mobile Optimization

- Touch-friendly navigation
- Responsive video players
- Optimized layouts for small screens
- Smooth scroll behavior

## 🏆 Award

Winner of 2024 Mad Mike Summer Bash Best Moving Picture Award

## 📧 Contact

- **Email**: alx.medianz@gmail.com
- **Phone**: 020 454 5459
- **Instagram**: [@alx.edits](https://www.instagram.com/alx.edits)

## 🔧 Technical Stack

- HTML5
- CSS3 (with CSS Variables)
- Vanilla JavaScript
- Instagram Embed API (fallback)
- Vercel (Hosting)

---

**Built by Alex Garcia Gil** | Professional Automotive Videographer | 2026