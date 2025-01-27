# BirdTalk Documentation

This repository contains the official documentation for BirdTalk, using MkDocs with the Material theme. The documentation covers installation, setup, command reference, and best practices for using BirdTalk.

## Using the Documentation

### Online Access

The documentation is published at: https://johncallender.github.io/birdtalk-docs/

Key sections include:
- Requirements and Setup - Installation instructions and system requirements
- Quick Start Guide - Get up and running with BirdTalk
- Command Reference - Detailed documentation of all BirdTalk commands
- Tips and Tricks - Best practices and advanced usage patterns

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
docs/
├── index.md                    # Landing page
├── installation/               # Installation guides
│   └── requirements-and-setup.md
├── quickstart/                 # Getting started
│   └── first-session.md
├── commands/                   # Command documentation
│   └── reference.md
├── tips-and-tricks.md         # Best practices
└── faq.md                     # Common questions
```

#### Adding New Content
1. Create new .md files in the appropriate directory
2. Update `mkdocs.yml` to include new pages in the navigation
3. Use Markdown for content formatting
4. Include code examples in fenced code blocks with language specification
5. Add images to the `docs/assets` directory (create if needed)

#### Building and Deployment

The documentation is automatically built and deployed to GitHub Pages when changes are pushed to the main branch.

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
