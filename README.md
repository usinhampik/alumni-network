# Alumni Network

Welcome to the Alumni Network for the Institute for Plasma Research (IPR) Gandhinagar. This platform is dedicated to connecting alumni, sharing resources, and fostering a supportive community for all members. Join us in celebrating our achievements and staying connected!

## Website

This repository publishes a website using MkDocs and GitHub Pages.

- Site content lives in [`docs/`](docs/).
- Alumni profile source files live in [`alumni-data/`](alumni-data/).
- Site configuration lives in [`mkdocs.yml`](mkdocs.yml).
- The GitHub Pages workflow lives in [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml).

## How To Update Content

For normal website changes, you usually do not need to touch the CI workflow.

- Edit Markdown files in [`docs/`](docs/) to update pages such as the home page, events, news, and resources.
- Edit files in [`alumni-data/`](alumni-data/) to add or update alumni profiles.
- Edit [`mkdocs.yml`](mkdocs.yml) only when you want to change site navigation, metadata, or MkDocs behavior.

The files in [`docs/alumni/`](docs/alumni/) are generated automatically from `alumni-data/` during the MkDocs build. Do not maintain them by hand.

## Local Preview

To preview the website locally:

```bash
mkdocs serve
```

Then open `http://127.0.0.1:8000/`.

To do a strict build check locally:

```bash
mkdocs build --strict
```

## How The Build Works

- Every branch push and pull request runs an MkDocs build in GitHub Actions.
- Only pushes to `main` deploy the live site to GitHub Pages.
- During the build, [`scripts/generate_alumni_docs.py`](scripts/generate_alumni_docs.py) regenerates alumni pages from [`alumni-data/`](alumni-data/).

## Useful MkDocs References

- MkDocs Getting Started: https://www.mkdocs.org/getting-started/
- MkDocs Configuration: https://www.mkdocs.org/user-guide/configuration/
- MkDocs Writing Documentation: https://www.mkdocs.org/user-guide/writing-your-docs/
- GitHub Pages with custom workflows: https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages
