# CMS-2026-1255 Regulation Comments Dashboard

Static website deployment for analyzing public comments on the CMS Interoperability and Prior Authorization for Drugs regulation (2026).

## Contents

- **index.html** - Interactive dashboard (109KB, fully self-contained)
- **analysis_results/** - AI-generated analysis files (JSON + readable TXT)
- **CMS-2026-1255-0001_comments.csv** - Metadata for all 21 comments

## Dashboard Features

- 📊 **7 Interactive Tabs**
  - Overview: Timeline, cumulative volume, attachment statistics
  - Organizations: Top commenting organizations
  - Sentiment: Distribution analysis
  - Themes: Key topics and concerns
  - Comments: Searchable list with filtering
  - Analysis: Detailed AI-generated insights
  - Geographic: State-by-state participation

- 🔍 **Search & Filter**
  - Full-text search across all comments
  - Filter by organization, sentiment, stakeholder type
  - Date range filtering

- 🌙 **Dark Mode** - Toggle for comfortable viewing

- 📤 **Data Export** - Download as JSON

## Deployment Instructions

### Option 1: Render.com (Recommended)

1. Fork or clone this repository to https://github.com/Pat-rickJoyce/PublicComments
2. Go to https://render.com
3. Create new **Static Site**
4. Connect to GitHub repository
5. Set:
   - **Branch**: main
   - **Root Directory**: `website_deploy`
   - **Build Command**: (leave empty)
   - **Publish Directory**: `.`
6. Deploy!

Your dashboard will be live at: `https://your-site-name.onrender.com`

### Option 2: GitHub Pages

1. Go to repository settings
2. Pages → Source → Deploy from branch
3. Select `main` branch
4. Set folder to `/ (root)` or create gh-pages branch with website_deploy contents
5. Access at: `https://Pat-rickJoyce.github.io/PublicComments/website_deploy/`

### Option 3: Netlify

1. Drag and drop the `website_deploy` folder to https://app.netlify.com/drop
2. Instant deployment!

## Technical Details

- **No backend required** - Pure HTML/CSS/JavaScript
- **No dependencies** - All data embedded in HTML
- **Responsive design** - Works on mobile, tablet, desktop
- **Browser compatibility** - Modern browsers (Chrome, Firefox, Safari, Edge)

## Comments Analyzed

- **Total**: 21 comments
- **With PDF attachments**: 7 (analyzed from PDF text)
- **Inline comments**: 13 (analyzed directly from submission text)
- **Analyzed**: 19 out of 21 (90% coverage)

## Data Sources

All data sourced from regulations.gov public API:
- Docket: CMS-2026-1255
- Document: CMS-2026-1255-0001
- Retrieved: June 2026

## Analysis Generated

AI-powered analysis using Claude (Anthropic) including:
- Commenter information & stakeholder classification
- Sentiment analysis
- Key themes identification
- Recommendations extraction
- Impact assessment
- Supporting evidence cataloging

## License

Public domain - These are public comments on federal regulations.
Dashboard code: MIT License

---

Generated with Claude Code - Regulation Comment Analyzer
https://github.com/anthropics/claude-code
