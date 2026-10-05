# Jaehyuk (Jay) Jang — personal website

Built with [Quarto](https://quarto.org) and published with GitHub Pages.

## Pages

| File | Page |
|---|---|
| `index.qmd` | Home (photo, bio, contact) |
| `publications.qmd` | Publications |
| `cv.qmd` | CV |
| `posts.qmd` | Blog listing |
| `posts/<name>/index.qmd` | One blog post each |
| `files/Jang_Jaehyuk_CV.pdf` | Downloadable CV |

## Publishing (one-time setup)

1. Create a public repo named exactly `YOUR-GITHUB-USERNAME.github.io`.
2. Upload everything in this folder (including the hidden `.github` folder) to the `main` branch.
3. In the repo, go to **Settings → Pages** and set **Source** to **GitHub Actions**.
4. The workflow in `.github/workflows/publish.yml` builds and deploys the site. It's live at `https://YOUR-GITHUB-USERNAME.github.io` in a minute or two.

Every later push to `main` rebuilds the site automatically.

## Adding a blog post

Copy `posts/hello-world/` to a new folder, e.g. `posts/my-new-note/`, then edit the `title`, `date`, `description` and `categories` at the top of `index.qmd` and write below it. Set `draft: true` in the header to keep a post hidden until it's ready.

## Previewing locally (optional)

Install Quarto, then run `quarto preview` in this folder.
