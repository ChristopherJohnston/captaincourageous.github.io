# Captain Courageous Website

Static website for the band Captain Courageous, built with Hugo and the Ananke theme.

## Website URL
https://www.captaincourageous.co.uk

## Local Development

### Prerequisites
- Hugo (installed via Homebrew)

### Running the Development Server
```bash
cd captaincourageous
hugo server -D
```

The site will be available at http://localhost:1313

### Building for Production
```bash
cd captaincourageous
hugo --cleanDestinationDir
```

The static site will be generated in the `public/` directory.

## Site Structure

- **Home** (`content/_index.md`) - Band introduction and overview
- **About** (`content/about.md`) - Band biography and influences
- **Music** (`content/music.md`) - Discography and links to streaming platforms
- **Contact** (`content/contact.md`) - Contact information and social links

## Content

The website includes:
- Band bio and description
- Discography (Astronomic, Burning Fire)
- Links to Linktree, YouTube, TikTok, X (Twitter)
- Contact information
- Band photos and logo

## Deployment Options

### Option 1: Netlify
1. Create a Netlify account
2. Connect your Git repository
3. Build command: `hugo --cleanDestinationDir`
4. Publish directory: `public`
5. Set your custom domain to `www.captaincourageous.co.uk`

### Option 2: GitHub Pages
1. Push your site to GitHub
2. Enable GitHub Pages in repository settings
3. Use GitHub Actions to build and deploy

### Option 3: Traditional Web Hosting
1. Build the site locally: `hugo --cleanDestinationDir`
2. Upload the contents of the `public/` directory to your web server
3. Configure your domain to point to the hosting

## Theme

This site uses the [Ananke theme](https://github.com/theNewDynamic/gohugo-theme-ananke) for Hugo.

## Configuration

Site configuration is in `hugo.toml`:
- Base URL: https://www.captaincourageous.co.uk/
- Language: en-gb
- Social media links
- Navigation menu

## Images

All band images are stored in `static/images/`:
- Logo variations (SVG, PNG, JPG)
- Band profile photos

## Updating Content

### Adding a New Song/Release
Edit `content/music.md` and add a new section following the existing format.

### Updating Social Links
Edit `hugo.toml` in the `[[params.ananke_socials]]` sections.

### Changing Images
Replace files in `static/images/` and update references in content front matter.

## Support

For questions or issues, contact: band@captaincourageous.co.uk
