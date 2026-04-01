# idiltuzkaya.github.io

Personal website of Idil Bukre Tuzkaya — statistics student, data scientist, writer.

## Files

| File | Description |
|------|-------------|
| `index.html` | Homepage with hero, featured projects, writing preview, contact |
| `projects.html` | All research projects in detail |
| `blog.html` | Writing / essays (click to read inline) |
| `media.html` | Videos and photos |
| `cv.html` | Full CV / résumé |
| `style.css` | Shared stylesheet for all pages |

## How to publish on GitHub Pages (5 minutes)

1. Create a GitHub account if you don't have one: https://github.com
2. Create a new repository named exactly: `YOUR-USERNAME.github.io`
   - Example: if your username is `idiltuzkaya`, the repo name is `idiltuzkaya.github.io`
3. Upload all files from this folder (index.html, projects.html, blog.html, media.html, cv.html, style.css)
4. Go to Settings → Pages → Source: Deploy from branch → main → / (root) → Save
5. Wait ~2 minutes, then visit `https://YOUR-USERNAME.github.io`

Your site is live. Free, forever, no hosting fees.

## How to add content

### Add a new blog post
Open `blog.html` and:
1. Add a new `<div class="blog-item">` block in the list section
2. Add a corresponding `<div class="post-view" id="postN">` block at the bottom
3. Update the `onclick="showPost('postN')"` to match

### Add a photo
Open `media.html` and replace an emoji in a `.photo-item` with:
```html
<img src="yourphoto.jpg" style="width:100%;height:100%;object-fit:cover;">
```
Then drop `yourphoto.jpg` into the same folder.

### Add a video
1. Upload your video to YouTube or Vimeo
2. In `media.html`, update the `onclick="window.open('YOUR_LINK', '_blank')"` with your link

### Update the CV
Edit `cv.html` directly — all content is plain HTML, easy to find and change.

### Language (EN/TR)
Every piece of text has either a `data-lang="en"` or `data-lang="tr"` attribute.
To add a new bilingual element:
```html
<span data-lang="en">English text</span>
<span data-lang="tr">Türkçe metin</span>
```

## Custom domain (optional)
If you want `idiltuzkaya.com` instead of `idiltuzkaya.github.io`:
1. Buy domain from Namecheap or Google Domains (~$10/year)
2. GitHub Settings → Pages → Custom domain → enter your domain
3. Follow the DNS setup instructions

---
Built with HTML, CSS, vanilla JS. No frameworks, no build step, no dependencies.
