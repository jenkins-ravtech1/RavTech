# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a static HTML documentation repository focused on development methodologies and training materials. The repository contains:

- **BMAD Workflow Guide**: Comprehensive guide for AI-driven agile development methodology
- **Developer Onboarding**: RavTech's junior developer training program documentation  
- Static HTML files with embedded Tailwind CSS and Mermaid.js for diagrams

## Development Commands

Since this is a static HTML repository, there are no build, lint, or test commands. Development is straightforward:

### Viewing Files
```bash
# Open files directly in browser
open bmad-workflow-guide.html
open onboarding.html
```

### Local Development Server (if needed)
```bash
# Simple Python server for local testing
python3 -m http.server 8000
# Then visit http://localhost:8000
```

## Architecture & Code Structure

### HTML Structure
- **Self-contained HTML files**: Each file includes all CSS, JavaScript, and content inline
- **Tailwind CSS**: Loaded via CDN for styling
- **Mermaid.js**: Used for workflow diagrams and flowcharts
- **Vanilla JavaScript**: Tab navigation and diagram rendering

### Key Components
- **Tab-based navigation**: Interactive section switching within single HTML files
- **Responsive design**: Mobile-first approach using Tailwind utilities
- **Accessibility features**: ARIA attributes, semantic HTML, keyboard navigation
- **Mermaid diagrams**: Auto-rendering flowcharts for process visualization

### File Organization
```
├── bmad-workflow-guide.html    # Main BMAD methodology documentation
├── onboarding.html            # RavTech developer onboarding (274KB)
├── test.html                  # Copy of BMAD guide for testing
└── .claude/                   # Claude Code settings
    └── settings.local.json    # Bash permissions configuration
```

## Content Architecture

### BMAD Workflow Guide Structure
The guide follows a structured approach with these main sections:

1. **Introduction**: Core concepts and AI agent roles
2. **Greenfield Workflow**: New project development process
3. **Brownfield Workflow**: Existing project enhancement process  
4. **Development Cycle**: Iterative implementation methodology
5. **Commands Reference**: Agent commands for different platforms
6. **Workflows**: Visual Mermaid diagrams showing process flows
7. **Documents**: Expected outputs and file structure

### Development Methodology Context
The documentation describes a two-phase approach:
- **Phase 1 (Planning)**: Web UI for document creation using AI agents
- **Phase 2 (Development)**: IDE-based implementation with file operations

## Working with This Repository

### Making Changes
- Edit HTML files directly - no build process required
- Test changes by opening files in browser
- Mermaid diagrams auto-render when sections become active

### Content Updates
- Follow existing HTML structure and Tailwind classes
- Maintain accessibility attributes (ARIA roles, semantic elements)
- Test tab navigation and responsive behavior

### Adding New Content
- Use consistent styling patterns from existing files
- Include proper meta tags for SEO
- Ensure Mermaid diagrams are properly wrapped in `.mermaid` divs

## Technical Considerations

- Files are self-contained for easy distribution
- Large file sizes (onboarding.html is 274KB) due to inline content
- CDN dependencies for Tailwind and Mermaid.js
- No version control for external dependencies