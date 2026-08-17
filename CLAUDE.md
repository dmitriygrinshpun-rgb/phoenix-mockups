# Phoenix Mockups — Claude Instructions

## What this repo is

Standalone, self-contained HTML/CSS/JS prototypes for Doodle's Phoenix product — used for fast design exploration outside the main app codebase (`poc-phoenix-post-mvp`). Each file is a single `.html` document with inline `<style>` and `<script>`, no build step, no dependencies. Open it directly in a browser or serve the folder with:

```bash
python3 -m http.server 8931
```

## Conventions

- One prototype per file, named for the flow it covers (e.g. `meeting-creation-v3_4.html`). Version bumps in the filename (`_v2`, `_v3_4`, ...) are fine when a prototype meaningfully diverges from the previous version rather than just fixing it — prefer editing the existing file in place for bug fixes and small iterations.
- Keep everything in one file: inline styles, inline `<script>`, no external assets or CDN links, so any file can be opened straight from disk or shared as a single attachment.
- Match the visual language already established (CSS variables like `--primary`, `--text-muted`, etc. at the top of each file) rather than introducing a new palette per prototype, unless the task is explicitly to explore a different visual direction.
- No frameworks, no bundler. Plain DOM APIs only.
- Update `README.md` with a one-line description whenever a new prototype file is added.

## Git Commits

Write commit messages that clearly explain **what the prototype does and why**, not which files were touched.

- Lead with a conventional prefix: `feat`, `fix`, `refactor`, `chore`
- The summary line should describe the user-facing change or behaviour
- The body should explain the feature/fix clearly in plain terms — what it does, how it works, edge cases covered
- No need to list individual files

### Format

```
<type>(<scope>): <short summary of the change>

<Clear description of what was added or fixed and why. Focus on
the feature behaviour, not the implementation details.>

Co-Authored-By: Claude Sonnet 5 <noreply@anthropic.com>
```
