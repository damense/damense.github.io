# Data Visualization Portfolio

Personal portfolio site built with [Quarto](https://quarto.org), showcasing
data visualizations in R

## Local development

```bash
# Preview the site locally
quarto preview

# Render the full site
quarto render
```

## Deployment

The site auto-deploys to GitHub Pages on push to `main` via GitHub Actions.

To enable:
1. Go to repo Settings → Pages
2. Set source to "GitHub Actions"

## Adding a new project

1. Export your visualization image to `images/`
2. Copy `projects/example-project.qmd` to a new file
3. Fill in the title, description, image path, write-up
4. Add a card to `portfolio.qmd` and optionally `index.qmd`
5. Commit and push — the site rebuilds automatically

## Structure

```
├── _quarto.yml          # Site config
├── index.qmd            # Landing page
├── portfolio.qmd        # Gallery grid
├── about.qmd            # About page
├── projects/            # Individual project write-ups
│   └── example-project.qmd
├── images/              # Viz exports and thumbnails
├── styles/
│   ├── custom.scss       # Theme overrides
│   └── extra.css         # Additional styles
└── .github/workflows/
    └── publish.yml       # Auto-deploy to GitHub Pages
```
