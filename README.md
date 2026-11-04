# PetWise · Path to $10M EBITDA — CreditSwan intelligence packet

Static site with one page. There is no build step and no server code.

## Files

- `index.html`: the packet. Styles, scripts and charts are inline. Charts are built lazily as each exhibit nears the screen.
- `favicon.svg`: the CreditSwan mark.
- `vercel.json`: clean URLs, plus `noindex` and security headers.

## Deploy on Vercel

**Option A: CLI**

1. Open a terminal in this folder.
2. Run `npx vercel` and follow the prompts: no framework, no build command, output directory `.`.
3. Run `npx vercel --prod` to publish.

**Option B: dashboard**

1. Push this folder to a Git repository.
2. In Vercel, choose **Add New → Project** and import the repository.
3. Set **Framework Preset** to **Other**, leave **Build Command** empty and set **Output Directory** to `.`.
4. Deploy.

## Notes

- Search engines are blocked by `noindex` in both the page and the headers. To limit who can see the site, turn on Vercel Deployment Protection.
- Fonts load from Google Fonts. The page falls back to system fonts when offline.
- Deep links work: `#overview`, `#commercial/cm-rgm`, `#roadmap/rv-milestones` and so on.
