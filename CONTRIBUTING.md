# Contributing to claude-short-stories
 
This repository holds comedy short stories co-written with Claude. Every story
keeps its full revision history, so the rules below exist to protect that history.
 
## Adding a new story
 
1. Create `stories/<story-slug>/` (lowercase, hyphens, no spaces).
2. Add one version at a time, in order. Each version is one commit containing:
   - `iterations/vN-<label>.md` (new file, never edited afterward)
   - `story.md` (overwritten with the new version)
   - `prompt-log.md` (one new row)
3. Optional: tag the commit `<story-slug>-vN`.
4. Add the story to the table in the root `README.md`.
 
For a series, each chapter gets its own `part-NN-<title-slug>/` folder with the
same three items, plus a series-level `README.md` with the reading order.
 
## Commit messages
 
Short, specific, present tense. Name the story, the version, and the change:
 
- `Porcelain Man v2: he slips a disc instead of helping her up`
- `Fred part 03 v2: Harold walks with Grady and merges too`
- `README: add Fred series to story table`
 
## Prompt logs
 
- Record every prompt verbatim, including reprint requests.
- Prompts that changed plot, character, theme, or tone get a new version file.
- Small line edits get a log row marked "(no new version)".
 
## Writing format
 
- One paragraph per line, with a blank line between paragraphs.
- Don't hard-wrap lines; it makes diffs unreadable.
 
## Branches
 
- Small changes may go straight to `main`.
- A whole new story can be drafted on `story/<story-slug>` and merged with a
  pull request. Use a merge commit, never squash: squashing erases the iterations.
 
## Never commit
 
- Drafts you don't want public (keep them in `private/`, which is ignored).
- Word source documents (keep them in `originals/`, which is ignored).
- Video or audio files; attach them to a Release instead.
 
## AI disclosure
 
Every story is written with Claude. Each `story.md` header and `prompt-log.md`
must say so.

