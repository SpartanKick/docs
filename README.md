# Coplay Documentation

This repository contains the official documentation for Coplay, an AI assistant specifically designed for Unity game developers. The documentation is built using [Mintlify](https://mintlify.com/), a modern documentation platform.

## Documentation Structure

The documentation is organized into the following main sections:

- **Getting Started**: Welcome information, installation guide, and basic usage instructions
- **Essentials**: Configuration options, settings, and best practices
- **Release Notes**: Updates and new features

## Configuration (docs.json)

The `docs.json` file is the main configuration file for the documentation. It defines:

- **Theme & Branding**: Sets "mint" theme, documentation name, colors (primary: #442172, light: #B48AEB, dark: #442172), and favicon
- **Navigation Structure**:
  - Tabs: "Guides" and "Release Notes"
  - Groups: "Get Started", "Using Coplay", and "Overview"
  - Pages: Mapped to .mdx files in the repository
- **Global Navigation**: Anchors for "Community" (Discord) and "Blog" links
- **Logo**: Path to SVG file used for both light and dark themes
- **Navbar**: Contains support email link and a primary "Get Started" button
- **Footer**: Social media links for Twitter/X, GitHub, LinkedIn, and Discord

This configuration controls the entire structure, appearance, and navigation of the documentation site.

## Local Development

To preview the documentation changes locally, install the [Mintlify CLI](https://www.npmjs.com/package/mintlify):

```bash
npm i -g mintlify
```

Then run the following command at the root of this repository (where docs.json is located):

```bash
mintlify dev
```

### Troubleshooting

- If Mintlify dev isn't running - Run `mintlify install` to re-install dependencies
- If a page loads as a 404 - Make sure you are running in a folder with `docs.json`

## Publishing Changes

Changes will be deployed to production automatically after pushing to the main branch.
