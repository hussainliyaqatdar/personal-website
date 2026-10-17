# personal-website

Hussain Liyaqatdar's product portfolio: a single static page (`public/index.html`) with shipped work, results and experience.

## Run locally

Open `public/index.html` in a browser, or serve the folder:

```bash
cd public && python3 -m http.server 8000
```

## Product screenshots

The page looks for screenshots in `public/img/` before falling back to the live product images:

`candor.jpg`, `orange.jpg`, `spotdraft-search.jpg`, `spotdraft-analytics.jpg`, `instamart.jpg`

Add your own files with these names and they are used automatically.

## Deploy on Render

`render.yaml` describes a free static site that publishes the `public/` folder.

1. In Render, choose **New > Blueprint** and select this repository, or **New > Static Site** with these settings:
   - Build command: `echo "Static site, nothing to build"`
   - Publish directory: `public`
2. Click **Deploy**. Every push to `main` redeploys automatically.
