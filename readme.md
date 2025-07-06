
# Hugo Blog Extended - Example Site

This repository contains a complete example site demonstrating the [hugo-blog-extended](https://github.com/BiosPlus/hugo-blog-extended) theme. The site is optimized for deployment on Cloudflare Pages.

## Features

- **Multilingual Support**: Content available in English, German, French, Italian, Portuguese, Russian, Japanese, and Chinese
- **Modern Design**: Clean, responsive layout with dark/light mode toggle
- **Rich Content**: Examples of markdown features, math typesetting, emoji support, and more
- **Optimized for Cloudflare Pages**: Pre-configured with proper build settings and Hugo version pinning

## Quick Start

### Deploy to Cloudflare Pages

1. **Fork this repository** to your GitHub account
2. **Connect to Cloudflare Pages**:
   - Go to your [Cloudflare Dashboard](https://dash.cloudflare.com/)
   - Navigate to **Computer (Workers)** → **Workers & Pages** → **Create** → **Pages** → **Import an existing Git repository**
   - Connect your GitHub account and select your forked repository
3. **Configure build settings**:
   - **Build command**: `hugo --minify`
   - **Build output directory**: `public`
   - **Root directory**: `/` (leave empty)
   - **Build system version**: Version 3 (Latest)
4. **Deploy**: Click "Save and Deploy"

Note: A `wrangler.toml` file is included for defining most of these settings and is read on build via the Cloudflare Pages runners.

### Theme Customization

For detailed customization options, refer to the [hugo-blog-extended documentation](https://github.com/BiosPlus/hugo-blog-extended).

## Cloudflare Pages Configuration

### Build Settings

| Setting | Value |
|---------|-------|
| Build command | `hugo --minify` |
| Build output directory | `public` |
| Root directory | `/` |
| Build cache | Disabled |
| Hugo version | 0.147.8 (defined in `wrangler.toml`) |

### Branch Control

- **Production branch**: `main`
- **Automatic deployments**: Enabled

### Environment Variables

The Hugo version is automatically set via the `wrangler.toml` file. You can modify it by updating the `HUGO_VERSION` variable.

## License

This example site is provided as-is for demonstration purposes. The hugo-blog-extended theme has its own [license](https://github.com/BiosPlus/hugo-blog-extended/blob/main/LICENSE).

## Support

- **Theme Issues**: Report issues with the theme at [hugo-blog-extended repository](https://github.com/BiosPlus/hugo-blog-extended/issues)
- **Cloudflare Pages Documentation**: [Cloudflare Pages Docs](https://developers.cloudflare.com/pages/)
