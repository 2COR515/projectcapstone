# Capstone Portfolio

A professional single-page portfolio website showcasing my capstone project.

## 🎓 Features

- **Profile Section**: Personal introduction with photo and bio
- **Video Presentation**: Embedded project video
- **Project Documentation**: PDF viewer with download option
- **Project Links**: Curated list of related resources
- **Responsive Design**: Optimized for desktop and mobile (9:16 vertical view)

## 📁 Structure

```
Portfolio/
├── index.html          # Main portfolio page
├── assets/
│   ├── profile.jpg     # Profile photo
│   ├── video.mp4       # Project video
│   └── report.pdf      # Project documentation
└── .github/
    └── copilot-instructions.md
```

## 🚀 Quick Start

### Local Development

1. Clone this repository
2. Install dependencies (optional): `npm install`
3. Start the Node.js server: `npm start`
4. Open your browser to: `http://localhost:3000`

### Setup Your Portfolio

1. **Add Your Profile Photo**: Place your photo as `assets/profile.jpg`
2. **Add Your Documents**: Place PDF reports in the `assets/` folder
3. **Upload Videos to YouTube**: 
   - Upload your large video files (`.mp4`) to YouTube
   - Copy the YouTube video links
   - Add them using the "🔗 Project Links" section in the portfolio
   - You can add multiple YouTube links for different videos
4. **Update Personal Information**: 
   - Click "Edit Profile" button on the website to update:
     - Name, bio, and contact details
     - Social media links

## 🌐 GitHub Pages Deployment

1. Go to repository Settings → Pages
2. Select main branch as source
3. Click Save
4. Your site will be available at: `https://yourusername.github.io/repository-name/`

## 📝 Customization

Edit the following in `index.html`:
- Profile name and bio (lines 440-446)
- Social media links (lines 448-452)
- Contact email (line 513)
- Project links in the Project Links section

## 💡 Notes

- All assets use relative paths (`./assets/...`) for GitHub Pages compatibility
- **Video files are excluded from Git** (see `.gitignore`) due to large size
  - Upload videos to YouTube and add links via the portfolio's Project Links section
  - The portfolio supports multiple YouTube links
- Design is optimized for professional academic presentation
- Node.js server is optional - the portfolio also works by opening `index.html` directly

## 📹 Adding YouTube Video Links

Since video files are too large for GitHub (100MB limit), follow these steps:

1. **Upload your videos to YouTube**:
   - Go to [YouTube Studio](https://studio.youtube.com)
   - Upload your project videos
   - Set visibility as needed (Public/Unlisted/Private)

2. **Add links to your portfolio**:
   - Open your portfolio in a browser
   - Scroll to the "🔗 Project Links" section
   - Enter each YouTube URL (e.g., `https://youtube.com/watch?v=...`)
   - Click "Add Resource" for each video
   - You can add multiple links for all your videos

3. **Example YouTube URLs**:
   ```
   https://youtube.com/watch?v=VIDEO_ID_1
   https://youtube.com/watch?v=VIDEO_ID_2
   https://youtube.com/watch?v=VIDEO_ID_3
   ```

## 📄 License

This portfolio template is free to use for educational purposes.
