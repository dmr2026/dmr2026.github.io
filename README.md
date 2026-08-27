# DMR workshop website

Sources for the website of the International Workshop on Designing Meaning Representations,
published with GitHub Pages at <https://dmr2026.github.io/>.

The site covers **all editions of DMR in one place** rather than one site per year.

## Layout

```
_config.yml            site title/description, build settings
_data/editions.yml     one entry per DMR edition — drives the home page table,
                       the "Past Editions" page and the per-edition navigation
_layouts/default.html  page template (two-tier navigation: site-level + per edition)
_layouts/redirect.html used by the root-level stubs that keep pre-2027 URLs working
index.md               DMR home page (all editions)
editions.md            /editions/ — archive of past editions
2027/                  DMR 2027 pages
2026/                  DMR 2026 pages (archived)
assets/                images
*.html (root)          redirects from the old flat URLs to /2026/...
```

## Adding a new edition

1. Add an entry at the top of `_data/editions.yml` with `local: true`, its `nav:` list, and
   `status: upcoming`. Set the previous edition's `status: past` and add its `proceedings:` link.
2. Create a `YYYY/` directory with `index.md`, `committees.md`, `submissions.md`, `venue.md`
   (plus `program.md` / `shared-task.md` when they exist). Every page needs front matter:

   ```yaml
   ---
   title: "Committees"
   edition: 2028
   permalink: /2028/committees/
   ---
   ```

3. Link images and other pages through `relative_url`, e.g.
   `{{ '/assets/photo.jpg' | relative_url }}`, so the site stays portable.

Nothing else needs editing — the navigation and edition lists are generated from `_data/editions.yml`.

## Local preview

```
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000/>.

## Working documents

`dmr_documents/` (reviewer lists, correspondence, proceedings material) is deliberately
git-ignored and excluded from the build — it must not be published.
