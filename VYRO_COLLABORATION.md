# VYRO Collaboration Instructions

This custom Claude app is used alongside ChatGPT to work on the VYRO iOS project.

## Shared repository
https://github.com/tyrobertsonwork-pixel/VYRO-iOS3

## Read these files before starting VYRO work
- Project brief: https://github.com/tyrobertsonwork-pixel/VYRO-iOS3/blob/ai-collaboration/AI_COLLABORATION/PROJECT_BRIEF.md
- Task board: https://github.com/tyrobertsonwork-pixel/VYRO-iOS3/blob/ai-collaboration/AI_COLLABORATION/TASKS.md
- Claude work log: https://github.com/tyrobertsonwork-pixel/VYRO-iOS3/blob/ai-collaboration/AI_COLLABORATION/CLAUDE_LOG.md
- ChatGPT review log: https://github.com/tyrobertsonwork-pixel/VYRO-iOS3/blob/ai-collaboration/AI_COLLABORATION/CHATGPT_REVIEW.md

## Workflow
1. Read the project brief and task board.
2. Work only on a dedicated branch; do not commit directly to main.
3. Before editing, inspect the current code and identify dependencies.
4. Record completed work, changed paths, commit/PR link, actual tests and limitations in the Claude work log.
5. Ask ChatGPT to review the resulting branch or pull request.
6. Do not merge without Ty's approval.

## Important limitation
This file is a human-readable handoff. It does not create a live connection to ChatGPT or automatically send messages between models. Ty must share the relevant GitHub links or content between the assistants. Never claim that the other assistant has reviewed work unless a review is actually recorded.

## Using the in-app source loader
1. Open the ⌘ collaboration panel in the custom Claude app.
2. Confirm repository `tyrobertsonwork-pixel/VYRO-iOS3` and branch `ai-collaboration`.
3. Leave the default source paths or add exact repository-relative paths, one per line.
4. Tap **Connect**, then **Load source + context**.
5. Start a new Claude message after loading; the project documents and selected source snapshots are included as system context.

The default source list includes:
- `www/index.html`
- `package.json`
- `capacitor.config.ts`
- `.github/workflows/ios-unsigned-ipa.yml`
- `tests/layout-smoke.cjs`

The loader reads source files from GitHub; it does not itself edit or commit application source files. Claude must not claim to have changed the repository unless a real commit or pull request exists. The in-app **Publish handoff** action only appends notes to `AI_COLLABORATION/CLAUDE_LOG.md`.
