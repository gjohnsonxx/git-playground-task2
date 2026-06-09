# Unit 4 Git playground — Lesson 2

A tiny command-line notes tool, used as the practice repo for Unit 4, Lesson 2 (committing well). The app is a safe sandbox; the task is to make one small change and have Claude commit it with a clear message.

### The app
- `node notes.js add <text>` — add a note
- `node notes.js list` — list all notes
- `node notes.js search <term>` — list notes containing a term
- `node notes.js delete <id>` — delete a note

Layout: `notes.js` is the entry point, `lib/store.js` loads, saves, and searches notes (in `notes.json`), and `lib/config.js` holds app settings.

### Set up
1. Make sure you have your own copy of this repo (created from the lesson on the platform).
2. Clone it locally and open Claude Code in the folder.

### Lesson 2 task — let Claude write the commit message
Goal: make one focused change, then have Claude commit it with a message a reviewer could understand without opening the diff.

1. Make one small, focused change. For example: the `search` command has a bug — it should list notes that *contain* your term, but right now it only matches the whole note exactly. Fix that, or add a short function of your own.
2. Before committing, jot down — in `notes.md` or a scratch note — the quick commit message you'd dash off yourself in five seconds.
3. Ask Claude: *"Stage my changes and commit them on a new branch with a good message."*
4. Open that commit on GitHub and read Claude's message. Does it explain the change — the *why*, not just the *what* — better than your five-second version?
5. Submit the link to the commit.
