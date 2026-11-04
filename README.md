# Doctor Unknown

## What the owner needs to know

The website runs on GitHub Pages. You do not need to run commands to keep it online.
The preview and validation commands are for whoever makes website changes.

- Keep the domain registration renewed and account recovery details current.
- After changes, review the live site on a phone and computer and report broken links or missing inquiries promptly.
- The contact link opens the visitor's email app. Test delivery to unknown@doctorunknown.com, including its private relay.

Developer instructions: see [For developers](#for-developers) below.

**Future business coming soon.**

**Website:** [doctorunknown.com](https://doctorunknown.com)
**Contact (private relay):** unknown@doctorunknown.com

## Files

| File | Purpose |
|---|---|
| `index.html` | The complete single-page website. All styles, scripts and artwork are contained in this one file. |
| `README.md` | This file. |
| `CNAME` | Created by GitHub Pages when the custom domain is set. Do not delete. |
| `robots.txt` | Instructions for search engine crawlers. |
| `sitemap.xml` | Sitemap submitted to search engines. |

## Hosting

The site is served by GitHub Pages from the `main` branch, root folder, with the custom domain `doctorunknown.com`. No build step is required.

---

## Legal Notice

*Last updated: November 1, 2026*

### Status of the project

Doctor Unknown is a future business in development. It is not a registered corporation, limited liability company, partnership or other legal entity, and it is not registered to do business in any state.

This website and repository are for informational purposes only. No goods or services are offered, sold or accepted through this website or by its owner at this time. The name "Doctor Unknown" is a brand name. It does not mean that the owner holds a medical license, doctoral degree or other professional credential, and nothing on the website is medical, professional or other advice.

### Ownership

The domains **doctorunknown.com** and **www.doctorunknown.com** are registered to and held by **Andrew Nahmias**, professionally known as **Andrew Jourdan** (the "Owner").

Except for the third-party material listed below, the following are the property of the Owner:

- the name **Doctor Unknown**;
- the Doctor Unknown logo, including the open hexagon "hex key" mark with its Staff of Hermes, and its placement beside the Doctor Unknown lettering;
- the unknown-molecule background artwork;
- the website's design, layout, text, code, color scheme and organization.

### Trademarks

Doctor Unknown™ is an unregistered trademark claimed by the Owner. It has not been registered with the United States Patent and Trademark Office or any other trademark office.

### Copyright

© 2026 Andrew Nahmias (Andrew Jourdan). All rights reserved.

This repository is public so that the website can be hosted on GitHub Pages. Public visibility is not a license. Apart from the limited rights that GitHub's Terms of Service give other GitHub users to view and fork public repositories within GitHub, no license is granted to copy, modify, distribute, publicly display or create derivative works from any part of this website or repository, in whole or in part, without the Owner's prior written permission. Requests for permission may be sent to unknown@doctorunknown.com.

### Third-party material

The following are not owned by the Owner and are used under their own terms:

- **Fonts:** Fraunces and Instrument Sans are loaded from Google Fonts and licensed under the SIL Open Font License 1.1.

### No warranty

This website and repository are provided "as is," without warranties of any kind.


## For developers

### Local preview

Use Python 3.12 or newer for the documented commands. This static site has no package installation or build step.
From the repository root, run:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000/; stop the preview with Ctrl+C.
An internet connection is needed for externally loaded fonts.

### Validation and publishing


Run `python3 scripts/check_site.py` before opening a pull request. GitHub Actions checks metadata, local links, sitemap, robots and the domain file. Main requires pull requests and passing Site checks; force pushes and deletion remain blocked. Review mobile and desktop layouts and the contact link before publishing.

Registrar transfer lock, auto-renewal, DNSSEC, GitHub Pages ownership verification and actual mailbox delivery require separate verification.
