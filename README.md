# World Robots - Digital Chairside Solutions

A modern, responsive landing page for World Robots dental technology solutions. This website showcases the complete digital chairside ecosystem for dental clinics.

## Features

- **Responsive Design**: Optimized for all devices (desktop, tablet, mobile)
- **Smooth Animations**: Scroll-based animations and smooth scrolling navigation
- **Clean Structure**: Separated HTML, CSS, and JavaScript for maintainability
- **Modern UI**: Gradient backgrounds, card-based layouts, and professional styling

## Project Structure

```
chike/
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # All styles
├── js/
│   └── main.js         # JavaScript functionality
└── README.md           # This file
```

## Sections

1. **Navigation**: Fixed top navigation with smooth scrolling
2. **Hero Section**: Eye-catching introduction with CTA buttons
3. **Value Proposition**: Key benefits and features
4. **Products**: Complete equipment showcase with specifications
5. **Materials**: Medical-grade dental consumables catalog
6. **Workflow**: Step-by-step digital workflow process
7. **Service & Support**: Training and support offerings
8. **Comparison**: Feature comparison with traditional labs
9. **Footer**: Contact information and site navigation

## Deploying to GitHub Pages

### Option 1: Using GitHub Web Interface

1. **Create a new repository** on GitHub
   - Go to https://github.com/new
   - Name your repository (e.g., `world-robots-website`)
   - Choose "Public" visibility
   - Click "Create repository"

2. **Upload files**
   - Click "uploading an existing file"
   - Drag and drop all files from this project
   - Commit the changes

3. **Enable GitHub Pages**
   - Go to repository Settings
   - Scroll to "Pages" section in the left sidebar
   - Under "Source", select "main" branch
   - Click "Save"
   - Your site will be published at `https://[username].github.io/[repository-name]/`

### Option 2: Using Git Command Line

1. **Initialize Git repository** (if not already initialized)
   ```bash
   git init
   ```

2. **Add all files**
   ```bash
   git add .
   ```

3. **Commit changes**
   ```bash
   git commit -m "Initial commit: World Robots landing page"
   ```

4. **Create repository on GitHub** (via web interface)
   - Go to https://github.com/new
   - Create new repository (don't initialize with README)

5. **Push to GitHub**
   ```bash
   git remote add origin https://github.com/[username]/[repository-name].git
   git branch -M main
   git push -u origin main
   ```

6. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Select "main" branch as source
   - Save

### Option 3: Using GitHub Actions (Automatic Deployment)

Create `.github/workflows/deploy.yml`:

```yaml
name: Deploy to GitHub Pages

on:
  push:
    branches: [ main ]

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./
```

## Local Development

To test the site locally:

1. **Simple HTTP Server (Python)**
   ```bash
   # Python 3
   python -m http.server 8000

   # Python 2
   python -m SimpleHTTPServer 8000
   ```

2. **Node.js HTTP Server**
   ```bash
   npx http-server
   ```

3. **VS Code Live Server**
   - Install "Live Server" extension
   - Right-click on `index.html`
   - Select "Open with Live Server"

Then open your browser to `http://localhost:8000` (or the port shown)

## Customization

### Changing Colors

Edit css/styles.css and modify the color variables:

```css
/* Primary blue gradient */
#00b4d8, #0096c7, #0077b6

/* Success green */
#28a745

/* Error red */
#dc3545
```

### Adding Content

1. **Products**: Add new product cards in the #products section of index.html
2. **Materials**: Add new material cards in the #materials section
3. **Features**: Add new feature cards in the #uvp section

### Modifying Animations

Edit js/main.js to adjust:
- Scroll animation timing
- Intersection observer thresholds
- Smooth scroll behavior

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- No external dependencies
- Optimized CSS with efficient selectors
- Minimal JavaScript
- Fast loading times

## License

Copyright © 2024 World Robots. All rights reserved.

## Contact

- Website: www.worldrobots.cn
- Email: worldrobots@qq.com
- Phone: 021-80370633
- Mobile: 18018526313

## Credits

Built with:
- Vanilla JavaScript
- CSS3 with Grid and Flexbox
- HTML5 semantic elements
- No frameworks or libraries required
