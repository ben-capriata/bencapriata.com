# bencapriata.com

Static portfolio and consulting website for Ben Capriata. It is deliberately dependency-free: there is no build command and no package manager.

## Pages

- `/` — snap-scrolling landing page
- `/work/` — detailed portfolio and consulting page
- `/404.html` — custom not-found page

## Preview locally

From the repository root:

```sh
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploy

Any static host can publish this repository. Set the project root as the output directory and leave the build command empty.

### Cloudflare Pages

1. Import the Git repository into Cloudflare Pages.
2. Choose the static/HTML preset, use no build command, and set the output directory to `/`.
3. Add `bencapriata.com` as the custom domain.
4. In Porkbun DNS, add the DNS records Cloudflare provides and remove conflicting records for the same host.

### GitHub Pages

The included `CNAME` file points Pages at `bencapriata.com`. Enable Pages for the `main` branch, then add the DNS records GitHub provides in Porkbun.

## Before publishing

- Confirm the claims, role title, and contact email.
- `og.png` is the social sharing image and should remain 1200×630.
- The verified LinkedIn and DHIS2 Community profiles are linked. GitHub was omitted because no public profile could be confidently verified.

