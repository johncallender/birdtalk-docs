# BirdTalk Documentation

This repository contains the official documentation for BirdTalk, using MkDocs with the Material theme. The documentation covers installation, setup, command reference, and best practices for using BirdTalk.

## Using the Documentation

### Online Access

The documentation is published at: https://johncallender.github.io/birdtalk-docs/

Key sections include:
- Requirements and Setup - Installation instructions and system requirements
- Getting Started - Tutorial and guide for using BirdTalk
- Command Reference - Detailed documentation of all BirdTalk commands
- FAQ - Common questions, tips, and best practices
- Uploading Checklists - Guide for uploading to eBird

The documentation site features:
- Tab-based navigation
- Integrated table of contents
- Full-text search with suggestions and highlighting
- Mobile-friendly responsive design

### Local Access

To preview the documentation locally:

1. Install Python and pip if not already installed
2. Install MkDocs and the Material theme:
   ```bash
   pip install mkdocs mkdocs-material
   ```
3. Clone this repository:
   ```bash
   git clone https://github.com/johncallender/birdtalk-docs.git
   cd birdtalk-docs
   ```
4. Start the local server:
   ```bash
   mkdocs serve
   ```
5. Open http://127.0.0.1:8000 in your browser

## Contributing to Documentation

### Getting Started

1. Ensure you have the required tools:
   - Python 3.x
   - pip (Python package manager)
   - Git

2. Set up your development environment:
   ```bash
   # Clone the repository
   git clone https://github.com/johncallender/birdtalk-docs.git
   cd birdtalk-docs

   # Install dependencies
   pip install -r requirements.txt
   ```

### Development Workflow

As a maintainer (John or Steve), you can:
1. Make changes directly to the main branch for straightforward updates
2. For complex changes:
   - Create a feature branch: `git checkout -b feature/your-feature-name`
   - Make and test your changes
   - Optionally create a pull request for review

### Documentation Standards

#### File Organization
```
birdtalk-docs/
├── mkdocs.yml           # MkDocs configuration
├── doc/                 # Project notes and background info
│   └── birdtalk-docs-notes.md  # Project status and history
├── docs/                # Documentation source files
│   ├── index.md        # Landing page
│   ├── getting-started.md  # Getting started guide with tutorial
│   ├── faq.md          # Frequently Asked Questions (includes Tips and Tricks)
│   ├── testimonial.md  # Personal experience testimonial
│   ├── uploading-checklists.md  # Guide for uploading to eBird
│   ├── commands/       # Command documentation
│   │   └── reference.md
│   ├── installation/   # Installation guides
│   │   └── requirements-and-setup.md
│   ├── images/         # Screenshots and images
│   │   ├── originals/  # Original high-resolution images
│   │   └── *.png      # Resized images for documentation
│   └── stylesheets/    # Custom CSS styles
│       └── extra.css
└── site/               # Generated documentation site
```

#### Adding New Content
1. Create new .md files in the appropriate directory
2. Update `mkdocs.yml` to include new pages in the navigation
3. Use Markdown for content formatting
4. Include code examples in fenced code blocks with language specification
5. Add images to the `docs/images` directory:
   - Store original high-resolution images in `docs/images/originals/`
   - Create display versions in `docs/images/` resized to 375px width
   - Use `sips` command for resizing:
     ```bash
     # For typical images where height ≤ width:
     sips -Z 375 docs/images/originals/image.png --out docs/images/image.png

     # For tall images where height > width:
     # Calculate height to maintain aspect ratio: (original_height/original_width * 375)
     sips --resampleHeightWidth [calculated_height] 375 docs/images/originals/image.png --out docs/images/image.png
     ```

#### Building and Deployment

To deploy updates to the public documentation site:
```bash
# Deploy to GitHub Pages
mkdocs gh-deploy
```

To build locally:
```bash
mkdocs build
```
The built site will be in the `site` directory.

### Troubleshooting

Common issues and solutions:
- If local preview isn't working, ensure port 8000 is available
- If changes aren't showing up, try clearing your browser cache
- For build errors, check the console output for specific error messages

## Contact and Support

- For documentation issues or suggestions:
  - Open a GitHub issue
  - Contact John Callender or Steve Colwell directly
- For BirdTalk software issues, please use the main BirdTalk repository
