# IDEA 2027 Workshop

Website: https://idea2027.github.io/

Repository: https://github.com/idea2027/idea2027.github.io

## Local editing

This is a plain HTML website. Edit the HTML pages and shared assets directly.
No build tools or dependencies are required.

| File | Content |
| --- | --- |
| `index.html` | Short overview, important dates, reviewer-call link |
| `cfp.html` | Call for papers and submission guidance |
| `committee.html` | Organizers and Call for Reviewers |
| `program.html` | Planned format and discussion panelist placeholder |
| `papers.html` | Oral and poster presentation placeholders |
| `keynote.html` | Confirmed keynote speakers |
| `assets/style.css` | Shared design and responsive layout |
| `assets/site.js` | Mobile navigation and section highlighting |

Navigation and footer are plain HTML repeated across the six pages; update all
pages when changing either. Dates appear on both Home and CfP and should be kept consistent. Detailed
topics and submission guidance live on CfP; organizer profiles live on Committee.

## Content and design sources

First-draft content is adapted from the organizers' supplied IDEA workshop
proposal. Submission (January 4), notification (February 1), and camera-ready
(February 16) dates in 2027 follow HCRS 2027 at the organizer's request; deadlines
use AoE. Unconfirmed talk details, submission rules, and program times remain
marked as to be announced. The proposal PDF is not included in this repository.

Layout and visual direction follow https://hcrs2027.github.io/ as requested.
The current Dublin city banner is the image selected by the organizer:
https://content.r9cdn.net/rimg/dimg/43/32/a04a5913-city-7362-163d136d1df.jpg?width=1366&height=768&crop=true.

Submission guidance allows publication in the ACM Web Conference 2027 Companion
Proceedings, with an author opt-out. The CfP covers three topic
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

The repository is public and GitHub Pages is enabled with HTTPS enforced.
GitHub publishes automatically from the root of the `main` branch after each
push. Publication may take a few minutes; check Actions and Settings → Pages
for deployment status.

The `.nojekyll` file keeps publication as a plain static website.
