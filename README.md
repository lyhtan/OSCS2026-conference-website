# Quarto conference website starter

This is a minimal four-page Quarto website for a temporary research conference.

## Pages

- `index.qmd` — landing page
- `signup.qmd` — registration
- `submit.qmd` — abstract submission
- `schedule.qmd` — programme
- `_quarto.yml` — site-wide navigation and configuration
- `styles.css` — fonts, colours, widths, footer logos, and responsive styling

## 1. Add your images

Put your existing header image here:

    images/header.png

Put collaborator logos here:

    images/logos/

The starter configuration currently expects:

    logo-1.png
    logo-2.png
    logo-3.png

Either rename your actual PNGs to those names or edit `_quarto.yml` to match their filenames.

## 2. Open in RStudio

Open this folder as a project/folder in RStudio.

If Quarto is installed, either use RStudio's Preview/Render controls or run:

    quarto preview

from the Terminal.

Quarto will open a local version of the website in your browser and refresh it when files change.

## 3. Edit the visual design

Start in `styles.css`.

The variables near the top control:

- page background
- text colour
- accent colour
- navigation/footer backgrounds
- maximum content width
- body font
- heading font

## 4. Edit conference information

Replace the placeholder conference name, dates, city, text, email address, and external form links in the `.qmd` files.

Also replace `Conference Name` in `_quarto.yml`.

## 5. Render the production site

Run:

    quarto render

The generated site will appear in the `docs/` folder. This is convenient for GitHub Pages publishing from the repository's `/docs` directory.

## 6. Next steps

Once the local version looks right, the usual next steps are:

1. create a GitHub repository;
2. push this folder to GitHub;
3. enable GitHub Pages using the `/docs` folder;
4. test the temporary `github.io` address;
5. connect the conference subdomain after the site is working.

## Notes

The footer uses root-relative image paths (`/images/...`) because Quarto recommends root-relative paths for shared website footer/header content. If you later deploy under a GitHub Pages project subpath rather than a custom domain, we can adjust this if necessary.
