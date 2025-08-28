# Developer Instructions

This document contains technical setup and development information for Shane's Universe website.

## Local Development

Run the site locally on macOS using Jekyll.

### Requirements
- Ruby and Bundler

### Commands

```bash
cd /Users/shanetsui/Documents/Project/shanetsui.github.io
gem install bundler
bundle install
bundle exec jekyll serve --livereload --livereload-port 35730
```

### Open in Browser

```bash
open http://127.0.0.1:4000
```

### Notes
- For live reload (Jekyll 4+): `bundle exec jekyll serve --livereload`
- If port 4000 is busy: `bundle exec jekyll serve -P 4001`
- If livereload port 35730 is busy: use `--livereload-port 35731`

## Technical Stack

- **Jekyll**: Static site generator
- **Beautiful Jekyll Theme**: 6.0.1
- **Ruby**: 2.6.0
- **Bundler**: 1.17.2

## Customizations Made

### CSS Modifications
- Reduced title font sizes for better proportion
- Decreased spacing around bullet point lists
- Increased navbar font sizes for better readability
- Reduced footer height for compact design
- Updated navbar colors to Twitter blue (#1DA1F2)

### Configuration Changes
- Pinned Jekyll to 3.9.x to avoid protobuf dependency issues
- Added jekyll-livereload plugin for development
- Excluded vendor/ directory from site generation
- Updated site title and author information

## File Structure

- `index.md`: Homepage with personal introduction
- `aboutme.md`: Detailed about page
- `_config.yml`: Site configuration and customization
- `assets/css/beautifuljekyll.css`: Custom CSS modifications
- `DEVELOPER.md`: This file with technical instructions

## Troubleshooting

### Common Issues
1. **Port conflicts**: Change ports using `-P` and `--livereload-port` flags
2. **Gem conflicts**: Use `bundle update` and ensure Jekyll 3.x compatibility
3. **Live reload issues**: Check if ports are available and restart server

### Dependencies
- All gems are installed locally in `vendor/bundle/`
- No system-wide Ruby gem installations required
- Uses Jekyll 3.9.x for stability and compatibility
