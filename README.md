# SS Elevators — Website

Static one-page website for **SS Elevators**, an ISO 9001:2015 certified elevator
manufacturer and service provider operating across Telangana and Andhra Pradesh
since 2018.

Live site: _add the URL here once deployed_

## Stack

Plain HTML + CSS + vanilla JavaScript. No framework, no build step, no
dependencies. Any static host serves it as-is.

## Structure

```
index.html            entire page (~45 KB)
assets/               logo, project photos, 2 project videos, social share image
favicon.ico  favicon-32.png  apple-touch-icon.png
robots.txt  sitemap.xml
_headers              cache rules (read automatically by Netlify)
netlify.toml          deploy config
```

## Deploying to Netlify

**From this repo (recommended — redeploys on every push):**

1. Netlify → *Add new site* → *Import an existing project* → GitHub → pick this repo.
2. Leave the build command empty. Publish directory: `.`
3. Deploy.

**Manual, no account needed (quick client preview):**

Drag the project folder onto <https://app.netlify.com/drop>.

## After the first deploy

Replace every occurrence of `REPLACE-WITH-YOUR-DOMAIN` with the live host
(no scheme, no trailing slash) in:

- `index.html` — `<link rel="canonical">` and `og:image`
- `robots.txt` — sitemap line
- `sitemap.xml` — `<loc>`

The `og:image` URL must be absolute, otherwise WhatsApp and LinkedIn link
previews show a blank card instead of the SS Elevators logo.

## What's already set up

- Page title and meta description targeting *elevator installation Hyderabad /
  Telangana / Andhra Pradesh*
- `LocalBusiness` JSON-LD structured data — name, address, phone, services, area served
- Open Graph / Twitter card for link previews
- Favicon and iOS home-screen icon
- Photos lazy-load; videos use `preload="none"` so they cost nothing until played
- Renders fully with JavaScript disabled — no content is hidden behind a script

## Contact

SS Elevators · #1-9-1, Srinivas Nagar, Temple Alwal, Secunderabad 500010, Telangana
Phone 7799225492 · sselevators.kumar@gmail.com
