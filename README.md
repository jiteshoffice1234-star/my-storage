# My Storage

Private cloud storage powered by GitHub.

## Structure

- `videos/` - Video files (MP4, MOV, AVI, MKV)
- `images/` - Image files (PNG, JPG, PSD, SVG)
- `documents/` - Documents (PDF, DOCX, PPTX, XLSX)
- `archives/` - Archives (ZIP, RAR, 7Z)
- `pages/` - GitHub Pages static site

## Features

- **Git LFS** - Store large files up to 2GB each
- **GitHub Pages** - Static site hosting at `https://jiteshoffice1234-star.github.io/my-storage/`
- **GitHub Releases** - Distribute files via releases (up to 2GB each)
- **Private** - Only you can access this repository

## Quick Upload

```bash
# Add files to the appropriate folder
cp your-file.pdf documents/
cp your-video.mp4 videos/

# Commit and push
git add .
git commit -m "Add files"
git push
```

## Using LFS

Large files are automatically tracked via Git LFS. Just add files normally:

```bash
git add videos/large-video.mp4
git commit -m "Add large video"
git push
```

## Creating Releases

```bash
gh release create v1.0.0 --title "Release 1.0" --notes "First release" ./archives/backup.zip
```
