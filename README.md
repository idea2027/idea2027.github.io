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
| `committee.html` | Organizers and Call for Reviewers |
| `program.html` | Planned format and discussion panelists |
| `papers.html` | Oral and poster presentation placeholders |
| `keynote.html` | Confirmed keynote speakers |
| `assets/style.css` | Shared design and responsive layout |
| `assets/site.js` | Mobile navigation and section highlighting |

Navigation and footer are plain HTML repeated across the six pages; update all
pages when changing either. Dates and submission guidance appear on both Home
and CFP and should be kept consistent.

## Content and design sources

First-draft content is adapted from the organizers' supplied IDEA workshop
proposal. Submission (January 4), notification (February 1), and camera-ready
(February 16) dates in 2027 follow HCRS 2027 at the organizer's request; deadlines
use AoE. Unconfirmed talk details, submission rules, and program times remain
marked as to be announced. The proposal PDF is not included in this repository.

Layout and visual direction follow https://hcrs2027.github.io/ as requested.
The Dublin sunset banner is the image selected by the organizer from Ryanair:
https://www.ryanair.com/flights/dam2/travel-tips/city/dublin/DUBLIN_r1.jpg.

Submission guidance allows publication in the ACM Web Conference 2027 Companion
Proceedings, with an author opt-out. Home and CFP share the same three topic
areas: identifier design and learning, evaluation and comparison, and deployment
and adaptation. The topic list is indicative, with other ID-related applications
and explorations in Web systems welcome.

Portrait and profile sources:

- Roger Zhe Li and Changhong Jin photos: https://semantic-id-tutorial.github.io/presenters.html
- Roger homepage: https://www.zhe-li.me/
- Changhong profile: https://ie.linkedin.com/in/changhong-jin (no standalone homepage verified)
- Junchen Fu photo and homepage: https://junchen-fu.github.io/
- Maria Maistro photo: https://sigir2025.dei.unipd.it/organization-chairs.html; homepage: https://mmaistro.github.io/
- Joemon M. Jose photo and profile: https://www.gla.ac.uk/schools/computing/staff/joemonjose/
- Huifeng Guo photo and linked Scholar profile: https://advanced-recommender-systems.github.io/AutoML-Recommendations/
- Neil Shah photo, homepage, and updated Pinterest biography: https://nshah.net/

The reviewer-interest button currently opens an email to Roger; replace it in
Home and Committee when a dedicated IDEA reviewer form is ready.

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
