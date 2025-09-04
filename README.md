# TABMON Website

The official website for the TABMON project built with Hugo static site generator featuring a custom purple-burgundy gradient design.

## 🚀 Quick Start

### Prerequisites
- **Hugo Extended** (v0.111.3 or later)
- **Git**

### Clone and Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/NINAnor/tabmon_website.git
   cd tabmon_website
   ```

2. **Install Hugo:**
   - **macOS:** `brew install hugo`
   - **Linux (Ubuntu/Debian):** 
     ```bash
     sudo apt install hugo
     # Or download from: https://github.com/gohugoio/hugo/releases
     ```
   - **Linux (using Nix):** `nix-shell -p hugo`
   - **Windows:** Download from https://gohugo.io/installation/windows/

3. **Start the development server:**
   ```bash
   hugo server
   ```
   
   Or with Nix:
   ```bash
   nix-shell -p hugo --run "hugo server"
   ```

4. **View your site:**
   Open http://localhost:1313 in your browser

### Making Changes
- Edit content in the `content/` directory
- Modify styling in `layouts/_default/baseof.html`
- Add images to `static/images/` (team photos) or `static/figures/` (project graphics)
- The site will automatically reload when you save changes

## 📁 Project Structure

```
tabmon_website/
├── content/             # Website content (Markdown files)
│   ├── _index.md       # Homepage
│   ├── about/          # About TABMON page
│   ├── data/           # Data section
│   ├── methods/        # Methods section
│   ├── news/           # News & updates
│   ├── publications/   # Publications
│   ├── resources/       # Resources & dashboard section
│   └── team/           # Team page
├── layouts/            # Custom HTML templates
│   └── _default/       # Default layouts
├── static/             # Static assets
│   ├── figures/        # Project graphics (logos, diagrams)
│   └── images/         # Team member photos
├── hugo.toml          # Hugo configuration
├── netlify.toml       # Netlify deployment config
└── README.md          # This file
```

## 🎨 Design Features

- **Custom purple-burgundy gradient theme** (#20003B to #7F2E4A)
- **Background logo watermark** with semi-transparent content areas
- **Responsive design** optimized for all devices
- **Professional typography** using Inter font family
- **Team photos** organized by institution
- **SEO optimized** with proper meta tags and social media integration

## 🚀 Deployment

This site is configured for automatic deployment on Netlify:

1. **Push to GitHub** - Any push to the `main` branch triggers a build
2. **Netlify builds automatically** using the configuration in `netlify.toml`
3. **Site goes live** at your Netlify URL

### Manual Deployment
```bash
# Build for production
hugo --gc --minify

# Output will be in the public/ directory
```

## 🛠️ Development

### Adding Content
- Create new `.md` files in the appropriate `content/` subdirectory
- Use existing files as templates for front matter and structure

### Adding Team Members
1. Add photo to `static/images/`
2. Update `content/team/_index.md` with member information

### Modifying Design
- Main styling is in `layouts/_default/baseof.html`
- Colors and gradients are defined as CSS variables
- Background logo settings can be adjusted in the CSS

## 📝 License

This project is part of the TABMON research initiative.
