# OSCS 2026 Conference Website
This repository contains the temporary website for the **OSCS 2026 Conference**.

The site is built with [Quarto](https://quarto.org/) and published as a static website.

## Site structure
The main pages are:
- `index.qmd` — conference landing page, called "Home" in navbar
- `programme.qmd` — programme and schedule
- `venue.qmd` — venue information
- `contact.qmd` — contact information

Site-wide configuration and styling are handled by:
- `_quarto.yml` — Quarto website configuration and navigation
- `styles.css` — custom styling
- `images/` — images, logos, and other visual assets

The rendered website is written to:
- `docs/` — generated HTML and site assets used for publication

## Local preview
From the project directory, run:

    quarto preview

This starts a local development server and automatically refreshes the site when files are changed.

## Render the site
To generate the production version of the website, run:

    quarto render

The rendered site will be placed in the `docs/` directory.

## Updating the website
After making changes:

    quarto render
    git add .
    git commit -m "Describe your changes"
    git push

The published website is updated from the rendered files in `docs/`.

## Project file
`OSCS2026-conference-website.Rproj` can be used to open the project directly in RStudio.

## License
Website and content is published CC BY 4.0, with exception for logos in footer.
