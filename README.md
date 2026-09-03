# Personal website

Live site: https://kys-sheng.github.io

All page content lives in `_data/*.yml` — edit those files, not the `.html` ones, to update the site.

| File | Controls |
|---|---|
| `_data/profile.yml` | Name, Mandarin name, bio, photo, office/contact info, link row (email/arXiv/InspireHEP/GitHub/Scholar) |
| `_data/publications.yml` | Publications page + "Recent publications" on Home |
| `_data/cv.yml` | Full CV page (education, positions, teaching, awards, skills) — also points to your CV PDF |
| `_data/tools.yml` | Tools page (each entry: name, description, website/GitHub/HuggingFace links) |
| `_data/talks.yml` | Talks page (each entry: title, event, date, Indico/slides links) — also the QR code image path |

To add a new publication, tool, or talk, copy an existing entry in the file and edit it — the layout picks it up automatically.

To add your QR code: drop the image anywhere under `assets/` and set the `qr_code:` field in `talks.yml` to that path.

To add your real photo: replace `assets/profile-placeholder.svg` with your image (e.g. `assets/profile.jpg`) and update the `photo:` field in `profile.yml` to match.

To add your CV: drop the PDF at `assets/cv.pdf` (or change the `pdf:` field in `cv.yml` if you name it differently).

This is a Jekyll site, which GitHub Pages builds automatically on push — no build step to run yourself.
