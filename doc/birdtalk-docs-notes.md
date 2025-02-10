# Birdtalk Documentation Project Notes

## Project Goals
Create comprehensive documentation for the Birdtalk project using MkDocs, including:
- Installation requirements and setup
- Quickstart guide
- Command reference
- FAQ and tips/tricks
- Troubleshooting information
- Personal testimonial (doc/jbc_testimonial.md)

## Solution Design
- Documentation platform: MkDocs
- Structure:
  - Landing page (index.md)
  - Installation guide (installation/requirements-and-setup.md)
  - Quickstart guide (quickstart/first-session.md)
  - Command reference (commands/reference.md)
  - FAQ (faq.md, includes Tips and Tricks)
- Generated site directory for built documentation

## Implementation History

### Initial Setup (Dec 23, 2024)
- Set up MkDocs framework (b6b822f)
- Created initial landing page content (c47d57b, f3a7505)
- Added installation requirements and troubleshooting guides (0777544)

### Content Development (Dec 24-26, 2024)
- Cleaned up top-level documentation pages (9b4675a)
- Made improvements to installation documentation (919f051)

### Cline Integration (Dec 28, 2024)
- Added initial Cline and Claude integration documentation (5b867d5)
- Improved bullet formatting in documentation (a74fa8b)

### Final Review Phase (Dec 31, 2024)
- Completed version 1.0 ready for Steve review (e519150)
- Fixed typos (bdf12aa)

## Current Status
Documentation version 1.1 is in progress, incorporating Steve Colwell's feedback. Completed changes:
- Updated index.md to clarify spoken instructions focus and add acknowledgments
- Updated command reference to use "Say" prefix and clarify spoken responses
- Updated Steve's email to stevebt@membot.com throughout
- Added beta testing commitment and phone number requirement to setup guide
- Removed obsolete Personal Locations section
- Added "upload later" command and upload button documentation
- Removed Merlin section and updated compatibility info
- Updated internet requirements about hotspot caching
- Added wind muffs recommendation to hardware section
- Updated GPS tracking references to reflect current functionality
- Added Tutorial with detailed example birding session
- Replaced abstract wildcards with concrete examples in command reference
- Added more examples throughout the documentation
- Updated audio setup instructions to remove "switch" command confusion
- Improved text formatting with proper spacing around bullet lists

## Documentation Style Guide

### Text Formatting
1. Bullet Lists and Spacing
   - Always add a blank line before and after bullet lists
   - This prevents lists from running into surrounding text
   - Example:
     ```markdown
     Here is some introductory text.

     - First bullet point
     - Second bullet point
     - Third bullet point

     Here is the following text.
     ```
   - This ensures proper visual separation and readability

2. Numbered Lists with Nested Content
   - Use consistent 4-space indentation for all nested content
   - Keep numbered list items together without blank lines between them
   - Use hyphens (-) instead of asterisks (*) for bullet points
   - Add blank lines before and after nested bullet lists within a numbered item
   - Example:
     ```markdown
     1. First item
         This is explanatory text under the first item.

         - A nested bullet point
         - Another nested bullet point

     2. Second item
         More explanatory text here.

         - More nested bullets
         - And another
     ```
   - This ensures proper list numbering and nesting

3. Lists with Images
   - Place images at the same indentation level as other nested content
   - Example:
     ```markdown
     1. First item
         <figure markdown>
           ![Image description](/path/to/image.png){ .screenshot }
           <figcaption>Image caption</figcaption>
         </figure>

         - A nested bullet point
         - Another nested bullet point
     ```
   - This maintains list continuity while properly displaying images

4. Image Layout
   - Screenshots float right with text wrapping
   - Current width: 375px
   - Consistent margins and spacing
   - Clear separation between sections (4em margin)
   - Image resizing guidelines:
     * Store original high-resolution images in docs/images/originals/
     * Use macOS sips command to create display-sized versions:
       ```bash
       # For typical images where height ≤ width:
       sips -Z 375 docs/images/originals/image.png --out docs/images/image.png

       # For tall images where height > width:
       # Calculate height to maintain aspect ratio: (original_height/original_width * 375)
       sips --resampleHeightWidth [calculated_height] 375 docs/images/originals/image.png --out docs/images/image.png
       ```
     * Always ensure width is exactly 375px to match documentation layout
     * Use -Z for typical images, --resampleHeightWidth for tall images to guarantee 375px width
   - Best practices for image positioning:
     * Place image-container divs before the content they illustrate
     * Allow h3 headings to wrap next to images by removing clear:both
     * Use clear-floats div to force specific sections below images
     * For extended content wrapping (including headings), use content-wrap:
       ```markdown
       <div class="image-container" markdown>
       <figure markdown>
         ![Alt text](/path/to/image.png){ .screenshot }
         <figcaption>Caption text</figcaption>
       </figure>
       </div>

       <div class="content-wrap" markdown="1">
       Content that should wrap, including headings...

       ## This Heading Will Wrap

       More content that wraps...
       </div>

       <div class="clear-floats"></div>

       ## This Heading Appears Below
       ```
     * The content-wrap class:
       - Allows h2 headings to wrap next to images
       - Maintains proper markdown formatting
       - Use when you want multiple sections to flow around an image
       - Always close with clear-floats before content that should appear below

     * For side-by-side images:
       ```markdown
       <div style="text-align: center" markdown>
       <div style="display: inline-block; margin-right: 1em" markdown>
       <figure markdown>
         ![First image](/path/to/image1.png){ .screenshot }
         <figcaption>First caption</figcaption>
       </figure>
       </div>
       <div style="display: inline-block" markdown>
       <figure markdown>
         ![Second image](/path/to/image2.png){ .screenshot }
         <figcaption>Second caption</figcaption>
       </figure>
       </div>
       </div>
       ```
       - Centers the container and displays images side by side
       - Uses inline-block to prevent floating behavior
       - Maintains proper markdown image processing
       - Adds margin between images for spacing

## Current Status (Feb 10, 2025)

Recent Updates:
1. Documentation Structure:
   - Combined Tips and Tricks into FAQ section
   - Simplified testimonial link text and description
   - Improved dialogue formatting in testimonial
   - Consolidated quickstart and tutorial content into getting-started.md
   - Removed redundant directories (quickstart/, tutorial/)
   - Updated navigation structure in mkdocs.yml
   - Cleaned up unused CSS styles in extra.css

2. Navigation and Mobile Improvements:
   - Fixed nav bar for mobile viewing
   - Adjusted nav bar padding for smaller screens
   - Updated navigation menu labels to be more descriptive
   - Removed unnecessary header button SVG styling

3. Content Updates:
   - Getting Started:
     * Added "BirdTalk is Listening" section explaining voice recognition
     * Added "Checklist Concepts" section explaining timer mode and entry behavior
     * Improved command examples and formatting
     * Clarified shorthand naming conventions
     * Reorganized sections for better flow

   - Command Reference:
     * Added detailed explanations for Starting/Stopping commands
     * Clarified checklist behavior and entry ordering
     * Added more context about the `Resume` and `Upload later` commands
     * Updated hotspot selection commands with better descriptions

   - Installation Guide:
     * Renamed sections to be more action-oriented
     * Improved section organization
     * Updated navigation links

   - Testimonial:
     * Improved dialogue flow and readability
     * Refined wording for better clarity
     * Updated formatting for consistency

4. Image Standards:
   - All BirdTalk UI screenshots standardized to 375px width
   - Images stored in two locations:
     * docs/images/originals/ - Full resolution originals
     * docs/images/ - 375px width versions for display
   - Special cases:
     * Steve's photo on index.md uses custom sizing
     * Sort view screenshots (04, 06) positioned side-by-side in command reference

Note: All planned tasks have been completed. Documentation is now in a polished state with consistent formatting, clear navigation, and standardized image handling.

## Project Structure
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
