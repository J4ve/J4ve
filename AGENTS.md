# Project agent memory

This file is the project's committed home for project-intrinsic agent knowledge: build, test, release, architecture, and sharp-edge notes that should travel with the code.

- This repo is the GitHub **profile** README repo (`J4ve/J4ve`). Its `README.md` renders at
  <https://github.com/J4ve>, not as an ordinary repo page.
- **Never start `README.md` with a `---` line.** GitHub treats a leading `---` as the opening
  fence of YAML front matter, fails to parse what follows, and shows an "Error in user YAML"
  banner at the top of the profile. Start with anything else (a heading, or an HTML block such
  as `<div align="center">`). A `---` rule lower in the file is fine.
- The profile page renders Markdown, not arbitrary HTML: `style` attributes are stripped, so do
  not rely on them for layout.
- To preview a change the way GitHub will actually render it, POST the file to the markdown API
  rather than trusting a local Markdown preview:
  `curl -X POST -H "Authorization: token $(gh auth token)" --data-binary @body.json https://api.github.com/markdown`
  where `body.json` is `{"text": "<file contents>", "mode": "gfm", "context": "J4ve/J4ve"}`.
  That endpoint does not reproduce the YAML error, so check the first line separately.

## Maintaining this file

Keep this file for knowledge useful to almost every future agent session in this project.
Do not repeat what the codebase already shows; point to the authoritative file or command instead.
Prefer rewriting or pruning existing entries over appending new ones.
When updating this file, preserve this bar for all agents and keep entries concise.
