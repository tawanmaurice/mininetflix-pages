# MiniNetflix Pages (Static Demo)

This repo hosts a **static demo video player** using GitHub Pages.  
It’s the companion showcase to the [MiniNetflix Terraform project](https://github.com/tawanmaurice/mininetflix), which originally deployed a Netflix-style streaming setup on **AWS S3 + CloudFront**.

Because AWS resources were destroyed, this GitHub Pages site serves as a **lightweight portfolio backup**.

👉 **Live Demo:**  
[https://tawanmaurice.github.io/mininetflix-pages/](https://tawanmaurice.github.io/mininetflix-pages/)

---

## Features

- **HTML5 Video Player**  
  Plays a sample MP4 video (`demo.mp4`) stored directly in the repo.

- **Easy Swaps**  
  Replace `demo.mp4` with any other MP4 (under 100MB) and update the commit.  
  The player will automatically serve the new video.

- **Portfolio-Friendly**  
  Zero AWS costs, just static hosting via GitHub Pages.

---

## Project Structure

- `index.html` → HTML5 video player page  
- `demo.mp4` → Current demo video (replaceable)  
- `main.tf` (planned to be added here) → Terraform reference file showing how AWS S3 + CloudFront was provisioned in the original project  

---

## How to Replace the Video

1. Put your new video in the repo root and name it `demo.mp4`  
   (keep size ≤ 100MB to avoid GitHub push issues).
2. Commit and push:
   ```bash
   git add demo.mp4
   git commit -m "chore: update demo.mp4"
   git push
