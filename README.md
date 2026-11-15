# jannahkarim.online

Portfolio of Jannah Karim Seifeldin, Product Designer.
A plain HTML/CSS/JS site. No build step, so GitHub Pages serves it as is.

## What's in here

- `index.html`: the whole site (home, projects, about, contact and the CV page at `#cv`)
- `images/`: the fluted-glass textures and the paper grain
- `Jannah-Seifeldin-CV.pdf`: the file behind the "Download PDF" button
- `CNAME`: tells GitHub Pages to serve the site at jannahkarim.online

## Put it online with GitHub Pages

1. On GitHub, create a new **public** repository.
2. Click **Add file → Upload files**. Drag in everything from this folder (not the zip itself), then click **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, pick `main` and `/ (root)`, and click **Save**.
4. On the same page, check that **Custom domain** says `jannahkarim.online`. If it doesn't, type it in and click **Save**.

## Point the GoDaddy domain at it

In GoDaddy, open the domain's **DNS** settings:

1. Delete any existing **A** records for `@`, and turn off any GoDaddy website or domain forwarding connected to the domain.
2. Add four **A** records, each with name `@`:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
3. Add (or edit) a **CNAME** record with name `www`, pointing to `YOUR-GITHUB-USERNAME.github.io`.

DNS changes can take anywhere from a few minutes to a day. Once the site loads, go back to **Settings → Pages** and tick **Enforce HTTPS**.

## Adding project screenshots later

1. Upload the image into the `images/` folder.
2. In `index.html`, find the "Coming soon" spot for that project. Put `<img src="images/your-file.jpg" alt="What the screen shows">` inside it, then delete the words `Coming soon` and `disabled`.
