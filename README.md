# ArvinSu Blog

This is a Hexo blog using the [NexT](https://theme-next.js.org/) theme, configured for automatic deployment to GitHub Pages.

## 🚀 Features
- **Hexo** Static Site Generator
- **NexT** Theme (Gemini scheme default)
- **GitHub Actions** for CI/CD
- **Strapi Integration Ready** (Configuration placeholders included)

## 🛠️ Development Workflow

We use a source-branch workflow:
1.  **`dev` Branch**: Active development (writing posts, changing themes).
2.  **`main` Branch**: Stable source code.
3.  **`gh-pages` Branch**: Generated static site (Auto-deployed).

### Daily Routine
1.  Checkout `dev`: `git checkout dev`
2.  Write/Edit: `hexo new "My Post"` or locally edit files.
3.  Preview: `hexo server` (Visit http://localhost:4000)
4.  Push: `git add .`, `git commit -m "..."`, `git push origin dev`
5.  **Release**: Merge `dev` to `main`.
    ```bash
    git checkout main
    git merge dev
    git push origin main
    ```
    (This triggers GitHub Actions to deploy to `gh-pages` automatically)

## 📦 Setup

```bash
# Install dependencies
npm install
```

## 🔌 Strapi Integration (Future)

This project consists of configuration placeholders for Strapi integration.
- **Config**: See `_config.yml` under `strapi:` section.
- **Script**: Logic location `scripts/strapi-placeholder.js`.
- **CI/CD**: `deploy.yml` has comments for enabling Strapi data fetching.

To enable:
1.  Set up Strapi server.
2.  Update `_config.yml` with API URL and Token.
3.  Implement fetching logic in `scripts/strapi-placeholder.js`.
4.  Uncomment relevant sections in `.github/workflows/deploy.yml`.
