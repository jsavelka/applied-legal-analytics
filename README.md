# Applied Legal Data Analytics and AI

Static course website. Open `index.html` to reach the Spring 2027 edition.
No build, package installation, or JavaScript is required.

## Editing and previewing

Edit `legalanalytics2027.html` for the current course and `course.css` for its
styling. `index.html` redirects to the current edition using a relative URL and
includes a fallback link. Earlier editions (2020–2025) retain their course
content and use relative navigation links. The 2019 edition remains externally
hosted. There was no 2026 edition.

The 2027 course content is carried over from 2025, including the schedule,
instructors, requirements, and registration contact. Edition and copyright
years have been updated. Historical references to the 2020 student paper remain.

To preview over HTTP, run this in the site directory:

```sh
python3 -m http.server 8000
```

Then visit http://localhost:8000/.

## Suggested hosting

Use a separate GitHub repository, for example `applied-legal-analytics`, with
GitHub Pages enabled. A project site can coexist with the personal website in
`jsavelka.github.io`; it does not require replacing that website.

1. Create the course repository and upload the site files, including `.nojekyll`.
2. In Settings → Pages, choose **Deploy from a branch** and the publishing
   branch (usually `main`) with **/(root)** as the folder.
3. Use the URL reported by Pages. Without a custom domain, the expected URL is
   `https://jsavelka.github.io/applied-legal-analytics/`.

If the personal Pages site uses a custom domain, GitHub may serve the project
under that domain. A course-owned organization or custom domain is another
option if independent ownership or branding is desired.

Internal course links use explicit `.html` filenames and relative paths so the
site also works under a subdirectory or on another static host. The current
edition's stylesheet is local; the archives retain their existing mini.css CDN
stylesheet. `jurix2024.html` and `alaai2021schedule.html` are legacy files retained
without changes.

After choosing a destination, update any links to the course on the personal
website. Old course URLs on the personal domain will need redirects in that
website's repository if they should keep working; moving these files alone
cannot redirect those URLs.

References:
- https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages
