# Shomer site

The product page for Shomer, a smart mezuzah. Plain static files: `index.html`, stills in `img/`, and the scroll-scrubbed films as JPEG sequences in `seq/`. No build step.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deploy on Replit

1. In Replit, choose **Import from GitHub** and pick this repository.
2. Open **Deployments** (Publish), choose **Static**.
3. Leave the build command empty and set the public directory to `./`.
4. Publish. The site is served at a `*.replit.app` address; a custom domain can be added in the deployment settings.

`.replit` already declares a static deployment and long cache headers for `img/` and `seq/`.

The renders, films and the CAD model they come from live in the main Shomer project folder.
