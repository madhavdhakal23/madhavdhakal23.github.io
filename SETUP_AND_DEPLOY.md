# Dr. Madhav Dhakal — Personal Website (al-folio)

This is a customized [al-folio](https://github.com/alshedivat/al-folio) academic website,
already populated with Dr. Dhakal's bio, photo placeholder, publications, news, and full CV.

## What's already done

- **Home / About** (`_pages/about.md`) — profile photo + the bio, affiliation, and contact info.
- **Publications** (`_bibliography/papers.bib`) — 20 peer-reviewed journal articles + 1 book chapter,
  auto-grouped by year, with Dr. Dhakal's name in **bold**. (Submitted manuscripts were intentionally left out.)
- **CV** (`_pages/cv.md`) — education, experience, awards, grants, presentations, invited talks,
  mentorship, training, affiliations, and service. (The "Skills/Core Competencies" and
  "Submitted Manuscripts" sections were intentionally left out, as requested.)
- **News** (`_news/`) — five recent highlights shown on the homepage.
- Site title, description, footer, and favicon set in `_config.yml`.

## 3 things YOU need to do

### 1. Add the real photo
Replace the placeholder at `assets/img/prof_pic.jpg` with Dr. Dhakal's actual photo.
Keep the filename **`prof_pic.jpg`** (a square image around 800×800 px looks best).

### 2. Set your web address in `_config.yml`
Find these two lines near the top and edit them:
```yaml
url: https://USERNAME.github.io     # <- your GitHub username
baseurl:                            # <- see below
```
- If you deploy to **`USERNAME.github.io`** (a user site): leave `baseurl:` blank.
- If you deploy to a **project repo** (e.g. `USERNAME.github.io/dhakal-site`): set `baseurl: /dhakal-site`.

### 3. (Optional) Add Google Scholar / ORCID
In `_data/socials.yml`, fill in `scholar_userid:` and `orcid_id:` to show those icons.

> The **Download CV** button serves `assets/pdf/Madhav_Dhakal_CV.pdf`, which is the full official CV.
> If you'd rather link a trimmed version, just replace that PDF file (keep the same name).

## How to publish it (free, recommended: GitHub Pages)

1. Create a free account at https://github.com if you don't have one.
2. Create a new **public** repository named `USERNAME.github.io` (use your own username).
3. Upload all of these files to that repository (drag-and-drop in the browser works, or use `git`).
4. In the repo: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
   al-folio includes a workflow that builds the site automatically.
5. Wait 2–3 minutes. Your site will be live at `https://USERNAME.github.io`.

Full official instructions: https://github.com/alshedivat/al-folio#installation

## How to preview it on your own computer (optional)

al-folio is a Jekyll site. The easiest local preview uses Docker:
```bash
docker compose up
```
then open http://localhost:8080. (Requires Docker Desktop.)
Or install Ruby + Jekyll and run `bundle install` then `bundle exec jekyll serve`.

## Where to edit things later

| To change…             | Edit this file                |
|------------------------|-------------------------------|
| Bio / photo / contact  | `_pages/about.md`             |
| Publications           | `_bibliography/papers.bib`    |
| CV content             | `_pages/cv.md`                |
| News on homepage       | files in `_news/`             |
| Site title / footer    | `_config.yml`                 |
| Social/email icons     | `_data/socials.yml`           |
