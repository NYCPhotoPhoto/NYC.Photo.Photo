# NYC.PHOTO — portfolio website

A single-file photography portfolio (Couples + Graduation). Everything lives in
`index.html`. No build step, no dependencies.

## See it locally
Just double-click `index.html` to open it in your browser.
(Or run `python3 -m http.server` in this folder and visit http://localhost:8000)

## 1. Add your details
Open `index.html`, find the block marked **☆ EDIT THIS BLOCK ☆** near the bottom,
and fill in your name, email, Instagram, location, and start year.

## 2. Add your photos
1. Drop image files into the **`images/`** folder.
   - Use small-ish web files (~1600px on the long edge, JPG, under ~500 KB each)
     so the site loads fast. The huge camera originals will be slow.
2. In `index.html`, find the **☆ YOUR PHOTOS LIVE HERE ☆** list and add a line:
   ```js
   { title:"Maya & Daniel", location:"Central Park", category:"Couples", focal:"85mm", src:"images/maya-daniel.jpg", alt:"Maya and Daniel hugging in Central Park" },
   ```
   - `category` must be `"Couples"` or `"Graduation"`.
   - Leave `src:""` to keep a styled placeholder.
3. For the big hero photo set `COVER.src`, and for your About portrait set `PORTRAIT.src`.

## 3. Publish it (free options)
- **Netlify Drop** — go to app.netlify.com/drop and drag this `website` folder in. Done.
- **GitHub Pages** — push this folder to a repo, enable Pages on the `main` branch.
- **Cloudflare Pages / Vercel** — connect the repo or drag-and-drop.

Then point your own domain (e.g. nycphoto.com) at it later.
