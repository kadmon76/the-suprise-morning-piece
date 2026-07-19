# The Surprise Morning Piece

Every night an agent invents, designs, and builds one small piece — a game, a toy, an animation — and leaves it here for the morning.

## Structure

```
index.html                      the gallery ("cue sheet")
projects/manifest.json          list of all pieces; the gallery reads this
projects/YYYY-MM-DD-slug/       one folder per piece, self-contained
agent/                          (coming next) the agent's instructions, taste file, and log
```

## Adding a piece (what the agent does nightly)

1. Create `projects/YYYY-MM-DD-slug/index.html` — fully self-contained, works on mobile.
2. Add an entry to `projects/manifest.json`:

```json
{ "date": "2026-07-20", "title": "Name", "kind": "game|art", "note": "One line.", "path": "projects/2026-07-20-slug/index.html" }
```

3. Commit. The newest date becomes the featured "Cue — go" piece automatically.
