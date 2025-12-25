# Shopify CLI Setup Guide

This repository is dedicated to **Shopify CLI setup and usage** for Shopify theme, app, and Hydrogen development.  
It explains installation, authentication, development store connection, and commonly used Shopify CLI commands.

---

## 🚀 What is Shopify CLI?

Shopify CLI is an official command-line tool that helps developers:
- Create and manage Shopify themes and apps
- Build and run Hydrogen storefronts
- Connect to Shopify Partner accounts and development stores
- Run Shopify projects locally

---

## 🧰 Prerequisites

Before starting, ensure you have:
- Node.js (v18 or later)
- Git installed
- Shopify Partner account
- Shopify development store

---

## 📦 Install Shopify CLI

Install Shopify CLI globally using npm:
```bash
npm install -g @shopify/cli
```

Verify installation:
```bash
shopify version
```

---

## 🔐 Login to Shopify

Authenticate your Shopify account:
```bash
shopify login
```

Login and connect to a specific store:
```bash
shopify login --store your-store-name.myshopify.com
```

---

## 🏪 Create or Connect a Development Store

Create or select a development store from your Shopify Partner account:
```bash
shopify dev
```

---

## 🛠 Common Shopify CLI Commands

List all available commands:
```bash
shopify help
```

Create a Shopify app:
```bash
shopify app create
```

Create a Shopify Hydrogen storefront:
```bash
shopify hydrogen init
```

Run a Shopify project locally:
```bash
shopify dev
```

---

## 📁 Use Cases

This repository is useful for:
- Learning Shopify CLI workflows
- Practicing store authentication and setup
- Preparing the environment for Hydrogen development
- Understanding Shopify's modern development tooling

---

## 📌 Notes

- Always use Node.js v18 or later
- Run Shopify CLI commands inside the project directory
- Ensure correct store permissions are enabled
- Clear CLI cache if login issues occur

---

## 🧑‍💻 Tech Stack

- Shopify CLI
- Node.js
- Git
- Shopify Partner Dashboard

---

## 📎 Author

**Jagdish Patidar**  
Shopify Developer
