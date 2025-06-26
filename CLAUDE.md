# Project: schuler-media.com

## implicator.ai Ghost Admin API

**API Key**: `685c83699aff68000115868b:f9720fe4ff8f92f315331521eb993ca5ddb38f083ba3969a4b938a134ff0484e`

**Base URL**: `https://implicator-ai.ghost.io`

**API Version**: `v5.0`

## Project Structure

- `/maali-implicator/` - Scripts for updating implicator.ai content
  - `update-alt-tags.js` - Updates image alt tags
  - `update-meta-descriptions.js` - Updates meta descriptions
  - `test-admin-api.js` - Tests API connection
  
  ### H1 Tag Fix Scripts (Lexical Format)
  - `fix-h1-tags-lexical-proper.js` - Fixes H1 tags for a single article (test script)
  - `fix-all-h1-tags-lexical.js` - Fixes H1 tags for all articles with multiple H1s
  - `show-article-structure.js` - Shows the heading structure of an article
  - `examine-lexical-structure.js` - Examines the Lexical JSON structure
  
  ### Legacy Scripts (Don't work with Lexical)
  - `preview-h1-fixes.js` - Preview script (HTML-based, doesn't work with Lexical)
  - `update-h1-tags.js` - Update script (HTML-based, doesn't work with Lexical)

## Common Tasks

### Updating Articles
- Use Ghost Admin API to fetch and update posts
- JWT tokens need to be generated using the API key
- Always test changes with preview scripts before applying

### Fixing H1 Tags
- Articles on implicator.ai use Lexical editor format (not mobiledoc/HTML)
- To fix H1 tags, use: `node fix-all-h1-tags-lexical.js`
- This converts all H1 tags (except the first) to H2 tags
- Excludes articles with titles starting with "Morning Briefing"

## Important Notes
- Ghost Admin API requires JWT authentication
- Token expiry is set to 5 minutes by default
- **Lexical Format**: implicator.ai uses Ghost's Lexical editor
  - Direct HTML updates won't work
  - Must update via the `lexical` field in the API
  - H1 tags are stored as `extended-heading` nodes with `tag: 'h1'`
- When updating posts with Lexical content, include `updated_at` timestamp

## Maintenance Tasks
- Deleting blind text articles on schuler media