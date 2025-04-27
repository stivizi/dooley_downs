# Developer Documentation for Minimal Landing Page

This document provides an overview of the project structure and instructions for setting up and running the minimal landing page locally.

## Project Structure

- `.gitignore`: Specifies intentionally untracked files that Git should ignore.
- `hugo.toml`: The main configuration file for the Hugo site.
- `archetypes/`: Contains archetype files for creating new content.
- `assets/`: Contains asset files like images and SCSS.
  - `assets/images/`: Images used in the theme.
  - `assets/scss/`: SCSS files for styling.
- `content/`: Contains the content files for the website (e.g., Markdown files).
- `data/`: Contains data files used by the theme.
  - `data/landing_page.yaml`: YAML file containing data for the landing page sections.
- `i18n/`: Contains internationalization files for translations.
- `layouts/`: Contains the main layout templates for the site.
- `public/`: This directory is generated when the Hugo site is built and contains the static website files.
- `resources/`: Directory used by Hugo for various resources.
- `static/`: Contains static files that are copied directly to the `public` directory.
  - `static/images/`: Static images.
- `themes/`: Contains the themes for the Hugo site.
  - `themes/minimal-theme/`: The custom theme used for this landing page.
    - `themes/minimal-theme/layouts/`: Theme-specific layout templates.
    - `themes/minimal-theme/layouts/_default/`: Default layout templates.
    - `themes/minimal-theme/layouts/partials/`: Partial templates used in layouts.
    - `themes/minimal-theme/static/`: Theme-specific static files.
    - `themes/minimal-theme/static/scss/`: Theme-specific SCSS files.

## Setup and Running Locally

This project uses Hugo, a static site generator.

1.  **Install Hugo:** Follow the official Hugo installation guide for your operating system: [https://gohugo.io/getting-started/installing/](https://gohugo.io/getting-started/installing/)

2.  **Clone the repository:**
    ```bash
    git clone git@github.com:stivizi/minimal-landing-page.git
    cd minimal-landing-page
    ```

3.  **Run the Hugo development server:**
    ```bash
    hugo server
    ```
    This will start a local development server, usually at `http://localhost:1313/`. The site will automatically rebuild and the browser will refresh when you make changes to the source files.

## Relevant Files

- `data/landing_page.yaml`: Modify this file to update the content of the different sections on the landing page (hero, intro, features, quote, transform, cta).
- `themes/minimal-theme/layouts/`: Edit the HTML files in this directory and its subdirectories to change the structure and layout of the pages.
- `assets/scss/style.scss` and `themes/minimal-theme/static/scss/`: Modify these SCSS files to change the styling of the landing page.
