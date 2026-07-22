![KB logo](./assets/images/KB.png)

# Kailyn Brown Portfolio

![Jekyll](https://img.shields.io/badge/Jekyll-Static%20Site-CC0000?logo=jekyll&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-121013?logo=github&logoColor=white)
![Themes](https://img.shields.io/badge/Themes-Aero%20%2B%20Chrome-4FC3F7)
[![Live Site](https://img.shields.io/badge/Live%20Site-Visit%20Portfolio-7C4DFF?logo=googlechrome&logoColor=white)](https://kailyn0215.github.io/portfolio/)

A personal portfolio website built with Jekyll, featuring a playful Frutiger Aero-inspired visual system, animated backgrounds, project case studies, and data-driven content sections.

[**Live site**](https://kailyn0215.github.io/portfolio/)

## Banner

![Portfolio banner graphic](./assets/images/kailynbrown.png)

Branding artwork used by the homepage in the current portfolio build.

## Overview

This site is a custom portfolio for showcasing Kailyn Brown's background, technical skills, featured work, and contact information. It uses Jekyll collections and YAML data files to keep content easy to update while preserving a fully custom visual design.

The homepage includes:

- a hero section with theme-aware branding
- an about summary pulled from structured data
- a skills preview driven by YAML content
- selected project cards generated from the `projects` Jekyll collection
- a contact form powered by Formspree

Additional pages provide a deeper look at background, skills, and project case studies.

## Features

- **Jekyll-powered static site** with collection-based project pages
- **Two visual themes** with saved preference via `localStorage`
- **Animated Frutiger Aero-inspired background system** with clouds, drifting orbs, and glass UI accents
- **Data-driven content** via `_data/*.yml`
- **Project gallery and case study pages** generated from `_projects/*.md`
- **Responsive layout** with reduced-motion and performance-minded interaction patterns
- **SEO and feed support** via `jekyll-seo-tag` and `jekyll-feed`

## Tech Stack

- **Static site generator:** Jekyll
- **Language/runtime:** Ruby
- **Templating:** Liquid
- **Content formats:** HTML, Markdown, YAML
- **Styling:** Custom CSS
- **Client-side behavior:** Vanilla JavaScript
- **Plugins:** `jekyll-feed`, `jekyll-seo-tag`

> [!NOTE]
> This project uses Jekyll from the main branch in `Gemfile`, which helps compatibility with newer Ruby versions.

## Project Structure

```text
portfolio/
├── _config.yml           # Jekyll site config, plugins, base URL, collections
├── _data/                # Structured content for about, skills, orbs, pills, etc.
├── _includes/            # Reusable navigation partials
├── _layouts/             # Page, homepage, and project layouts
├── _projects/            # Project case studies as collection items
├── assets/
│   ├── css/              # Main stylesheet
│   └── images/           # Logos, profile image, skies, orb textures, artwork
├── projects/             # Projects index page
├── about.html            # About detail page
├── index.html            # Homepage
├── skills.html           # Skills detail page
├── run.sh                # Convenience script for local development
└── README.md
```

## Getting Started

### Prerequisites

- Ruby installed locally
- Bundler available in your shell

### Install dependencies

```sh
cd /Users/kb83635/sideproj/website2/portfolio
bundle install
```

### Run the site locally

```sh
cd /Users/kb83635/sideproj/website2/portfolio
bundle exec jekyll serve --livereload
```

Or use the included helper script:

```sh
cd /Users/kb83635/sideproj/website2/portfolio
./run.sh
```

The site builds into `_site/` and, with the current configuration, is available locally at:

```text
http://127.0.0.1:4000/portfolio/
```

### Production build

```sh
cd /Users/kb83635/sideproj/website2/portfolio
bundle exec jekyll build
```

## Content Editing Guide

### Update personal information

Edit `_data/about.yml` to change:

- bio and background copy
- journey timeline
- interests and values
- experience and education
- resume download link
- contact details

### Update skills

Edit `_data/skills.yml` to manage:

- homepage skill categories
- detailed skill breakdowns
- proficiency labels and descriptions

### Add or edit projects

Each project lives in `_projects/` as a Markdown file with front matter.

Useful fields include:

- `name`
- `tagline`
- `description`
- `category`
- `status`
- `stack`
- `github`
- `live`
- `cover_image`
- `hero_image`
- `gallery`
- `overview`
- `problem`
- `solution`
- `features`
- `challenges`
- `outcomes`

Project pages are published using the permalink pattern defined in `_config.yml`:

```text
/projects/:name/
```

### Update visuals

- Replace or add assets in `assets/images/`
- Update theme styling in `assets/css/style.css`
- Adjust decorative content in `_data/orbs.yml` and `_data/pills.yml`

## Pages

Routes below are shown relative to the site base URL. In production, that base URL is `/portfolio`.

- `/` — homepage
- `/about.html` — extended about page
- `/skills.html` — technical skills breakdown
- `/projects/` — project gallery
- `/projects/:name/` — individual project case studies

## Deployment Notes

The site is configured for GitHub Pages-style hosting with:

- `url: "https://kailyn0215.github.io"`
- `baseurl: "/portfolio"`

If you deploy this site somewhere else, update `_config.yml` so asset paths and generated links stay correct.

## Verified Commands

The following build command was successfully run in this project:

```sh
bundle exec jekyll build
```

## Screenshot and Asset Notes

The repository already includes branding and decorative assets such as:

- `assets/images/KB.png`
- `assets/images/kailynbrown.png`
- `assets/images/meowl.jpg`
- `assets/images/sky1.jpg` through `assets/images/sky6.jpg`

These support the current identity and animated background system used across the site.
