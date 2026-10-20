# IDEA 2027 Workshop

Planned website: https://idea2027.github.io/ (not published yet)

Repository: https://github.com/idea2027/idea2027.github.io

## Local editing

This is a plain HTML website. Edit `index.html` and add assets as needed.
No build tools or dependencies are required.

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
