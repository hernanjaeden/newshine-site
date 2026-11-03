# NewShine Detailing: Landing Page

Single-page, mobile-first site in plain HTML + CSS. No build step, no dependencies.

- `index.html`: page content
- `styles.css`: dark theme with gold accents

## Preview locally

Open `index.html` in a browser, or run a static server:

```sh
npx serve .
# or
python -m http.server 8000
```

## Deploy

### GitHub Pages
1. Push this folder to a GitHub repository.
2. In the repo go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select your branch (`main`) and folder `/ (root)`, then **Save**.
4. The site goes live at `https://<user>.github.io/<repo>/` within a minute or two.

### Netlify
- **Drag and drop:** go to <https://app.netlify.com/drop> and drop this folder.
- **Git:** *Add new site → Import an existing project*, pick the repo, leave the build command empty and set the publish directory to `.`.

Add a custom domain under **Domain settings** in Netlify, or **Settings → Pages → Custom domain** on GitHub.

## Booking form

The form carries Netlify Forms attributes (`data-netlify`, honeypot), so on Netlify submissions appear under **Forms** in your dashboard with no extra code. Enable email notifications there.

GitHub Pages has no form backend. There, set the form's `action` to a service such as [Formspree](https://formspree.io) and remove the `data-netlify` attributes.

## Before going live: replace placeholders

- Phone `(902) 555-0123` and email `hello@newshinedetailing.ca` in the footer
- Facebook / Instagram links in the footer
- Prices in the Services section
- Testimonials (currently samples; use real, permitted customer quotes)
- Before/After placeholders: swap the `.ph` divs for `<img src="..." alt="...">` with descriptive alt text
