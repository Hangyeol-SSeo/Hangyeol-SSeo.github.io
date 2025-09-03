# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based resume website using the modern-resume-theme. It's designed to be hosted on GitHub Pages and serves as a personal portfolio/resume site.

## Architecture

- **Jekyll Static Site Generator**: Built with Jekyll, configured in `_config.yml`
- **Theme Structure**: Uses modern-resume-theme (v2.0.10) with modular components
- **Content Configuration**: Uses version 2 content system with flexible sections (Projects, Experience, Education, etc.)
- **Layout System**: 
  - Main layout: `_layouts/default.html`
  - Includes: `_includes/` (header, footer, about, section components)
  - Sass styles: `_sass/` (base, dark mode, icons, buttons, typography)
- **Data-driven Content**: All resume content configured in `_config.yml` using YAML structure

## Development Commands

### Local Development
```bash
bundle install          # Install dependencies
bundle exec jekyll serve # Start local server at http://localhost:4000
```

### Docker Development (Alternative)
```bash
docker-compose up        # Start Jekyll in container at http://localhost:4000
```

### Common Issues
- **Bundler version conflicts**: Use `gem install bundler:2.1.4` or `bundle update --bundler`
- **ffi gem compilation errors**: Install Xcode Command Line Tools with `xcode-select --install`
- **Permission errors**: Use `sudo` for gem installation or prefer rbenv/rvm

## Content Management

### Main Configuration
- **`_config.yml`**: Contains all personal info, social links, and resume content
- **Content sections**: Defined in `content:` array with `layout: list` or `layout: text`
- **Dark mode**: Controlled via `darkmode:` setting (true/false/never)

### Styling
- **Custom styles**: Add to `assets/main.scss` after the import line
- **Sass organization**: Modular stylesheets in `_sass/` directory
- **Theme components**: Base styles, dark mode, icons, buttons, typography

### Layout Options
- **List layouts**: left, right, top, top-right, top-middle (for Experience, Education, Projects)
- **Text layouts**: For free-form content sections
- **Responsive design**: Built-in mobile responsiveness

## File Structure
- **`_includes/`**: Reusable HTML components and sections
- **`_layouts/`**: Page templates
- **`_sass/`**: Stylesheet partials
- **`_site/`**: Generated site (excluded from git)
- **`assets/`**: Static assets (favicon, custom JS/CSS)
- **`images/`**: Image assets for content

## Deployment
- **GitHub Pages**: Automatically deploys from master branch
- **Local testing**: Always test changes locally before pushing
- **Config changes**: Require server restart to see changes