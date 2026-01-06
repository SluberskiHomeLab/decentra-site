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