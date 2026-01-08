# Coplay Documentation & Release Notes Update Guide

**Last Updated:** August 15, 2025

This guide captures the process followed when updating Coplay documentation and release notes based on Discord messages from Marcus (`msanatan`) and Jos (`josvdw`). It summarizes what worked, what didn't, and suggests improvements for future iterations.

## 📋 Overview

**Last Documentation Update Completed:** August 15, 2025
- ✅ Successfully updated: `configuration.mdx`, `settings.mdx`, `blender-mcp.mdx`
- ❌ Failed to update: Release notes (pending)

---

## 1. 📚 Gathering Requirements from Discord

### Initial Setup
1. **Login to Discord:**
   - Use the browser tool to navigate to [discord.com](https://discord.com)
   - Log in using your credentials
   - Navigate to the Coplay public server

2. **Search for Relevant Messages:**
   - Use Discord's search (or channel-specific search) to filter messages from `msanatan` and `josvdw`
   - Search for keywords: `docs`, `mode`, `release`, etc.

### Collecting Information

**Marcus' Key Updates (Version 2.0.0):**
- Easier MCP usage
- Ability to create/paste MCP JSON
- Additional MCP servers (Blender MCP & Supabase)

**Jos' Key Updates (Version 4.3.0):**
- Detailed descriptions of modes
- Instructions for using external docs/web search
- Orchestrator mode
- Web search functionality
- Kimi K2 model support
- Domain-reload improvements
- Pipeline recording improvements
- Various bug fixes

### Documentation Planning
- Compile information into concise bullet points
- Identify which existing docs need updates:
  - `configuration.mdx`
  - `settings.mdx` 
  - `blender-mcp.mdx`
- Plan new release notes entries

---

## 2. 📝 Updating Documentation

### Repository Access
1. **Navigate to GitHub:**
   - Go to [github.com/CoplayDev/coplay](https://github.com/CoplayDev/coplay)
   - Ensure you are logged in to GitHub
   - *Note: GitHub API connector only provides read operations*

2. **Create a New Branch:**
   - Use GitHub's UI to edit a file
   - When committing, select "Create a new branch and start a pull request"
   - Use descriptive branch names (e.g., `update-docs-mode-section`)

### File Updates

#### `Docs/essentials/configuration.mdx`
- Replace the "Mode" placeholder with detailed list of modes:
  - Normal
  - PipelineRecording
  - Orchestrator


#### `Docs/essentials/settings.mdx`
- Add section on external documentation and web search
- Include information about:
  - Downloading docs
  - `.coplayrules.md` file usage
  - New web search feature

#### `Docs/tutorials/blender-mcp.mdx`
- Note the ability to create/paste MCP JSON
- Mention additional MCP servers (Supabase)

### Pull Request Process
1. Commit each change directly to your branch
2. Create a PR summarizing the changes
3. Wait for user or reviewer approval before merging

---

## 3. ⚠️ Updating Release Notes (Lessons Learned)

### Location
- File path: `Docs/api-reference/release-notes/index.mdx`
- Use GitHub's search to locate the file

### Challenges Encountered

**GitHub Monaco Editor Issues:**
- ❌ Click placement: Must click to the right of line numbers, otherwise clicks are ignored
- ❌ Scroll behavior: Typing causes unpredictable scrolling
- ❌ Text persistence: Newly typed text often doesn't persist
- ❌ Verification: Search (`Ctrl+F`) confirmed inserted strings weren't saved

### Outcome
- ❌ **Release notes were NOT successfully updated**
- 📋 **Status:** Pending task
- 📝 **Prepared content:** Available for versions 4.3.0 and revised 2.0.0 entry

---

## 4. 💡 Recommendations for Next Time

### Alternative Editing Approaches
1. **Local Development:**
   - Clone repo locally (if authentication permits)
   - Use GitHub Desktop for editing and pushing changes
   
2. **File Replacement Method:**
   - Copy file's raw content to clipboard
   - Modify locally
   - Delete old file and upload new version via GitHub UI

### File Management
- **Break release notes into smaller files:**
  - Consider splitting by year or quarter
  - Smaller files are easier to edit through web interface

### Editor Best Practices
- **Confirm editing mode:**
  - Ensure caret is visible (vertical bar `|` indicates active caret)
  - If typing scrolls unexpectedly, immediately search for inserted text
  - Undo and retry if text doesn't persist

### Documentation Tracking
- **Record update dates:**
  - Always note when documentation was last updated
  - Track which files were successfully updated vs. pending

### Backup Strategy
- **Maintain prepared content offline:**
  - Keep summarized release notes in local files
  - If editing fails, attach content to PR for manual application by reviewers

---

## 5. ✅ Conclusion

### Success Summary
- ✅ Documentation successfully updated in separate files via new branch and PR
- ✅ Process worked well for: `configuration.mdx`, `settings.mdx`, `blender-mcp.mdx`

### Outstanding Issues
- ❌ Release notes update failed due to GitHub Monaco editor reliability issues
- 🔄 **Recommendation:** Use local editing or file upload method for future release notes updates

### Next Steps
- Consider implementing local development workflow for large file edits
- Maintain backup content for failed updates
- Document successful patterns for future reference