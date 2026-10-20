# IDEA 2027 Workshop

Planned website: https://idea2027.github.io/ (not published yet)

Repository: https://github.com/idea2027/idea2027.github.io

## Local editing

This is a plain HTML website. Edit the HTML pages and shared assets directly.
No build tools or dependencies are required.

| File | Content |
| --- | --- |
| `index.html` | Overview, dates, topics, program highlights, organizers |
| `cfp.html` | Call for papers and submission guidance |
| `committee.html` | Organizers and confirmed Program Committee |
| `program.html` | Planned format and discussion panelists |
| `papers.html` | Accepted papers placeholder |
| `keynote.html` | Confirmed keynote speakers |
| `assets/style.css` | Shared design and responsive layout |
| `assets/site.js` | Mobile navigation and section highlighting |

Navigation and footer are plain HTML repeated across the six pages; update all
pages when changing either. Dates and submission guidance appear on both Home
and CFP and should be kept consistent.

## Content and design sources

First-draft content is adapted from the organizers' supplied IDEA workshop
proposal. Unconfirmed dates, talk details, submission rules, and program times
remain marked as to be announced. Organizer portraits use initials until photos
are supplied. The proposal PDF is not included in this repository.

Layout and visual direction follow https://hcrs2027.github.io/ as requested.
The Dublin banner is retained from that reference at
https://hcrs2027.github.io/img/hero-beckett-bridge-dusk-full.jpg.
Confirm image attribution or replace the banner before public release.

To preview locally:

```sh
cd /Users/rogerzheli/Desktop/code/idea2027.github.io
python3 -m http.server 8000
```

Open http://localhost:8000 in your browser. Press Ctrl+C to stop the server.

## Publish changes

Run these commands inside this repository, not its parent directory:

```sh
cd /Users/rogerzheli/Desktop/code/idea2027.github.io
git status
git add index.html
# Add any other intended website files explicitly as well.
git commit -m "Update workshop website"
git push origin main
```

The repository is currently private and GitHub Pages is not enabled.
On GitHub Free for organizations, Pages requires a public repository.
When ready to publish, make the repository public or use a plan that supports
Pages from private repositories, then configure Settings → Pages to deploy
from the root of the `main` branch. Once enabled, pushes publish automatically.

The `.nojekyll` file keeps publication as a plain static website.
