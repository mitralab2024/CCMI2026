# CCMI 2026 static site

This folder is a GitHub Pages-compatible static rebuild of the public Google Sites website:

https://sites.google.com/iu.edu/ccmi2026

## Contents

- `index.html` — Home page
- `program/` — Program page
- `registration/` — Registration page
- `abstract-submission/` — Abstract submission page
- `venue/` — Venue page
- `accomodation/` — Accommodation page, using the source site's spelling
- `accommodation/` — Redirect alias to `accomodation/`
- `contact/` — Contact page
- `assets/` — CSS, JavaScript, and images
- `.nojekyll` — Prevents GitHub Pages from processing this as a Jekyll site

## Deploy to GitHub Pages

1. Create a GitHub repository.
2. Upload the contents of this folder to the repository root.
3. In GitHub, go to **Settings → Pages**.
4. Set the source to your branch, usually `main`, and the root folder.
5. Save. GitHub will publish the site after the Pages build completes.

## Local preview

From this folder, run:

```bash
python3 -m http.server 8080
```

Then open:

```text
http://localhost:8080
```

## Maintainer notes

The Abstract Submission page on the source site appears to contain an embedded Google Form. The form's direct embed URL was not exposed in the public static page text, so the GitHub Pages version links to the original abstract-submission page. Replace that link with your Google Forms embed URL once you have it.

The `sitemap.xml` uses placeholder `example.github.io/ccmi2026` URLs. Replace those with your final GitHub Pages URL after publishing.
