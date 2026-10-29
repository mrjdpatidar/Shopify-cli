# Shopify Theme Development with Shopify CLI

A Shopify theme development demo with a practical guide to working locally using Shopify CLI.

This repository contains theme files organized into Shopify's standard directories, alongside instructions for connecting a store, previewing changes, running theme checks, and uploading an unpublished theme.

> This is a personal development repository. It is not the official Shopify CLI project.

## Project Scope

This project focuses on Liquid-based Shopify theme development.

It provides a workspace for working with:

- Liquid layouts, sections, and snippets.
- Page templates.
- CSS and JavaScript assets.
- Theme settings and translations.
- Local development previews using Shopify CLI.

Shopify app development and Hydrogen storefronts are separate workflows and are outside the scope of this guide.

## Technology Stack

| Technology | Purpose |
| --- | --- |
| Shopify Liquid | Storefront templates and dynamic content |
| HTML | Page structure |
| CSS | Styling and layout |
| JavaScript | Storefront interactions |
| Shopify CLI | Theme preview, validation, and synchronization |
| Git & GitHub | Version control |

## Repository Structure

| Directory | Purpose |
| --- | --- |
| `assets/` | Stylesheets, JavaScript, images, and other theme assets |
| `config/` | Theme settings schema and configuration |
| `layout/` | Shared layouts used by templates |
| `locales/` | Storefront and theme editor translations |
| `sections/` | Theme sections and their settings |
| `snippets/` | Reusable Liquid components |
| `templates/` | Templates for storefront page types |

## Prerequisites

Before starting, you need:

- A Node.js version supported by the current Shopify CLI.
- npm.
- Git.
- A Shopify store you are authorized to access.
- An account with the required theme permissions.

For current installation requirements, see the
[official Shopify CLI documentation](https://shopify.dev/docs/storefronts/themes/tools/cli).

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/mrjdpatidar/Shopify-cli.git
cd Shopify-cli
```

### 2. Install Shopify CLI

```bash
npm install -g @shopify/cli@latest
```

Verify the installation:

```bash
shopify version
```

### 3. Start a Development Preview

Replace the example domain with your store's `.myshopify.com` domain:

```bash
shopify theme dev --store your-store.myshopify.com
```

Follow the authentication prompts if requested.

The command starts a development preview connected to your store. Use the URLs shown in the terminal to preview the theme and access the theme editor.

Store products, collections, navigation, and other content come from the connected store. They are not included in this repository.

### 4. Make Changes

Edit the relevant theme files:

- Styling and interactions in `assets/`.
- Sections in `sections/`.
- Reusable components in `snippets/`.
- Page templates in `templates/`.
- Shared layouts in `layout/`.

While the development command is running, Shopify CLI updates the preview as supported files change.

### 5. Run Theme Check

```bash
shopify theme check
```

Review the reported issues and address applicable errors and warnings.

### 6. Upload an Unpublished Theme

To upload the local theme for review:

```bash
shopify theme push --unpublished --store your-store.myshopify.com
```

Follow the prompts to create an unpublished theme.

Review its preview in Shopify Admin before deciding whether to publish it. Uploading an unpublished theme does not automatically make it the live storefront.

## Useful Commands

| Command | Purpose |
| --- | --- |
| `shopify version` | Display the installed CLI version |
| `shopify theme dev --store your-store.myshopify.com` | Start a development preview |
| `shopify theme check` | Check theme code |
| `shopify theme list --store your-store.myshopify.com` | List store themes |
| `shopify theme info` | Inspect the current theme environment |
| `shopify theme push --unpublished --store your-store.myshopify.com` | Upload an unpublished theme |
| `shopify auth logout` | Sign out of the current account |
| `shopify theme --help` | View available theme commands |

## Suggested Review Checklist

Before sharing or uploading changes:

- Review desktop and mobile layouts.
- Check navigation and links.
- Test product variant selection and cart interactions where implemented.
- Review empty states and missing content.
- Check the browser console for JavaScript errors.
- Run Theme Check.
- Confirm the intended store and theme before uploading.

## Project Status

This repository is a development demo.

It should not be treated as a production-ready theme without reviewing its code, store configuration, and storefront behavior.

## Official References

- [Shopify CLI for Themes](https://shopify.dev/docs/storefronts/themes/tools/cli)
- [Shopify Theme Architecture](https://shopify.dev/docs/storefronts/themes/architecture)
- [Shopify Liquid Reference](https://shopify.dev/docs/api/liquid)
- [Shopify CLI Theme Commands](https://shopify.dev/docs/api/shopify-cli/theme)

## Author

**Jagdish Patidar**  
Shopify & Full-Stack Developer  
Founder & CEO — **Drunall Technologies**

I build custom Shopify experiences, business applications, and workflow automation.

- [Drunall Technologies](https://www.drunall.com)
- [Portfolio](https://jdpatidar.com)
- [LinkedIn](https://www.linkedin.com/in/jdpatidar/)

---

Independent project by Jagdish Patidar. Not affiliated with or endorsed by Shopify.
