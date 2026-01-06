# Decentra Website

Official static website for the [Decentra](https://github.com/SluberskiHomeLab/decentra) project - a decentralized, Discord-like chat server and client that is self-hostable.

## Deployment to Cloudflare Pages

This site is designed to be deployed directly to Cloudflare Pages with zero configuration.

### Quick Deploy Steps:

1. **Connect Repository**: Link this GitHub repository to Cloudflare Pages
2. **Build Settings**: 
   - Build command: Leave empty (no build needed)
   - Build output directory: `/` (root directory)
3. **Deploy**: Click deploy and your site will be live!

> **Note**: This repository includes a `wrangler.toml` configuration file that ensures proper deployment. If you encounter issues, make sure the build command in Cloudflare Pages settings is left empty.

### Manual Testing Locally:

To test the site locally before deployment:

```bash
# Using Python
python3 -m http.server 8080

# Using Node.js
npx http-server -p 8080

# Using PHP
php -S localhost:8080
```

Then open `http://localhost:8080` in your browser.

### Troubleshooting Deployment

If you encounter a build error mentioning `wranger` (note the typo), this means the build command in Cloudflare Pages dashboard was incorrectly configured. To fix:

1. Go to your Cloudflare Pages project settings
2. Navigate to **Builds & deployments** → **Build configuration**
3. Ensure the **Build command** field is **empty** (this is a static site with no build step)
4. Save changes and retry deployment

The `wrangler.toml` file in this repository should prevent this issue for new deployments.

## Features

- 📱 Fully responsive design (mobile, tablet, desktop)
- 🎨 Modern Discord-inspired theme
- ♿ Accessibility compliant (ARIA labels, semantic HTML)
- 🔒 Security best practices (rel="noopener noreferrer")
- ⚡ Fast loading (single HTML file with embedded CSS)
- 🌐 SEO optimized with proper meta tags

## Structure

```
decentra-site/
├── index.html          # Main website file (all-in-one)
└── README.md           # This file
```

## License

This website is part of the Decentra project. See the main [Decentra repository](https://github.com/SluberskiHomeLab/decentra) for license information.