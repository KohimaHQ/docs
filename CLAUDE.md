# Claude AI Context - Mint Documentation

## Project Overview

This directory contains documentation files for the Mintlify documentation site hosted at `docs.kohimahq.com`, which is connected to the git repository for automatic deployment.

## File Structure & Usage

### Core Documentation Files
- **`bcp-meeting-intelligence.mdx`** - MDX documentation page for BCP meeting intelligence features
- **`regulatory-analysis.mdx`** - MDX documentation page for regulatory analysis capabilities  
- **`llm.txt`** - LLM-related content and documentation
- **`mint.json`** - Mintlify configuration file for the documentation site

### Template & Reference Files
- **`mintlify_templates.md`** - Model card/template documentation for Mintlify.com integration

## Optimal Usage of mintlify_templates.md

The `mintlify_templates.md` file serves as a **model card** and reference guide for working with Mintlify. When working on documentation:

1. **Reference First**: Always check `mintlify_templates.md` before creating new MDX files to understand:
   - Proper MDX syntax and structure
   - Mintlify-specific components and features
   - Styling conventions and best practices
   - Component examples and patterns

2. **Template Source**: Use it as a template when creating new documentation pages to ensure consistency

3. **Component Library**: Refer to it for available Mintlify components and their proper usage

4. **Style Guide**: Follow the formatting and structure patterns shown in the templates

## Mintlify Integration Notes

- Changes to MDX files automatically deploy to `docs.kohimahq.com`
- The `mint.json` file controls site configuration and navigation
- MDX files support React components and enhanced markdown features
- Always validate MDX syntax before committing changes

## Development Workflow

1. Reference `mintlify_templates.md` for structure and components
2. Edit or create MDX files following the template patterns
3. Test locally if possible before committing
4. Push changes to trigger automatic deployment to docs.kohimahq.com