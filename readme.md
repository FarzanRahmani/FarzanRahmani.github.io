# Farzan Rahmani's Academic Website

Personal academic website for Farzan Rahmani, an M.Sc. student in Computer Engineering (Artificial Intelligence and Robotics) at Sharif University of Technology. The site presents research interests, publications, education, experience, honors, teaching, and contact information.

**Website:** [farzanrahmani.github.io](https://farzanrahmani.github.io/)

## Design

The website uses plain HTML and CSS, with a dark theme, responsive layouts, system fonts, keyboard navigation, and print styles. Native HTML disclosures provide selected coursework and teaching details without JavaScript. No framework, package installation, or build step is required.

## Project Structure

| Path | Purpose |
| --- | --- |
| `index.html` | Page content, profile links, search metadata, and structured profile data. |
| `style.css` | Layout, colors, typography, responsive rules, and print styles. |
| `favicon.svg` | Website icon. |
| `resume/resume.pdf` | Concise CV, linked as the primary download. |
| `resume/resume_detailed_version.pdf` | Detailed CV with the full academic and professional record. |
| `resume/farzan.jpg` | Profile portrait. |
| `robots.txt` | Crawler instructions and sitemap location; excludes `/archive/` from crawling. |
| `sitemap.xml` | Canonical homepage URL and last modification date. |
| `.nojekyll` | Allows GitHub Pages to serve the repository as static files without Jekyll processing. |
| `archive/` | Previous Jekyll website source, posts, theme files, and assets. |

The archive preserves the earlier site's source. It is not a rebuilt, independently browsable version of that site.

## Local Preview

Open `index.html` directly in a browser, or run the following command from the project root with Python 3 installed:

```sh
python -m http.server 4173 --bind 127.0.0.1
```

Visit [http://127.0.0.1:4173](http://127.0.0.1:4173). Stop the server with `Ctrl+C`.

## Updating Content

- Edit the relevant sections of `index.html` to update publications, education, experience, honors, or service.
- Update the lists inside the Education and Teaching disclosures when coursework or teaching experience changes. Keep audited courses clearly labeled and separate from graded coursework.
- Replace the PDFs in `resume/` after rebuilding the CVs. Keep their filenames stable, and update the page-count labels in `index.html` if the lengths change.
- Keep the visible profile information consistent with the description, social sharing metadata, and JSON-LD structured data in the page's `<head>`.
- Update the footer's revision month, JSON-LD `dateModified`, and sitemap `lastmod` when making substantive content changes.
- Adjust presentation in `style.css`; the current site does not depend on files in `archive/`.

Before publishing, check narrow and wide layouts, keyboard navigation, both disclosures, publication links, and CV downloads.

## GitHub Pages

To publish the site using GitHub Pages:

1. Commit and push the intended website files to the branch used for publishing.
2. In the repository's **Settings > Pages**, select **Deploy from a branch** if branch-based publishing is not already configured.
3. Select the publishing branch and **/ (root)** folder, then save.
4. Check the Pages deployment result and visit [https://farzanrahmani.github.io/](https://farzanrahmani.github.io/).

The repository includes `.nojekyll`, so the active site does not require the archived Ruby or npm tooling.

## Search Visibility

The site includes a canonical URL, descriptive page metadata, social sharing metadata, `Person` and `ProfilePage` structured data, and a sitemap. After publishing, the sitemap at [https://farzanrahmani.github.io/sitemap.xml](https://farzanrahmani.github.io/sitemap.xml) can be submitted through Google Search Console. Search ranking depends on indexing and external signals and is not guaranteed.

## Attribution

The archived website uses the [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) Jekyll theme. The existing `LICENSE` preserves the theme's MIT license and attribution to Michael Rose and contributors.
