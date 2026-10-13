# Born2Win Custom — Blog

A simple, fast blog for Born2Win Custom (B2W) builds. Plain HTML + CSS, no build tools. It runs free on GitHub Pages.

## What's in here

```
index.html                              Home page (hero, latest builds, gallery)
posts/off-white-chicago-cord-set.html   First build story (magazine-style Q&A feature)
css/style.css                           All the styling (colors/fonts at the top)
js/site.js                              Scroll animations, count-up numbers, photo zoom
images/                                 Photos and logo
.nojekyll                               Tells GitHub Pages to serve files as-is
```

## Put it on GitHub Pages (about 5 minutes)

1. Go to github.com and create a new repository, for example `born2win-blog`. Make it **Public**.
2. Click **Add file → Upload files**, drag in everything from this folder (keep the `css`, `images` and `posts` folders), and click **Commit changes**.
3. Go to **Settings → Pages**. Under **Source**, pick **Deploy from a branch**, choose **main** and **/(root)**, then **Save**.
4. Wait a minute or two. Your site will be live at `https://YOUR-USERNAME.github.io/born2win-blog/`.

Using the command line instead:

```bash
cd born2win-blog
git init
git add .
git commit -m "Launch Born2Win Custom blog"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/born2win-blog.git
git push -u origin main
```

Then do step 3 above.

## Add a new build post

1. Copy `posts/off-white-chicago-cord-set.html` and rename it, e.g. `posts/my-next-build.html`.
2. Change the title, text and image paths inside it.
3. Put new photos in `images/`. Keep them under ~1600px wide so pages load fast.
4. In `index.html`, copy the `<a class="card">` block under `<!-- POST CARD -->`, paste it **above** the old one (newest first), and point it at your new post.
5. Commit and push (or upload the changed files on GitHub). The site updates in about a minute.

## Change colors or fonts

Everything is at the top of `css/style.css` under `:root` — `--red`, `--ink`, `--cream`, etc.
