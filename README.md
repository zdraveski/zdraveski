### Hi, I'm zdraveski

I build free, open-source plugins for [Claude Code](https://claude.com/claude-code), Anthropic's coding assistant for the terminal. Each one fixes something that bothered me in daily use: Claude forgetting yesterday's work, or hitting a usage limit without warning.

They share a few rules:

- **Your data stays on your computer.** No account, no API key, no server of mine.
- **Works on Windows, macOS and Linux.** Every change is tested automatically on all three.
- **Easy to undo.** Each plugin can be paused or removed, and puts back what it changed.
- **Plain-language docs.** Written for people who use Claude Code, not only for developers.

---

#### 🧠 [project-memory](https://github.com/zdraveski/project-memory) · [project page](https://zdraveski.github.io/project-memory/)

**Claude remembers your work: where you left off, and anything you did before.**

Claude Code starts each conversation from zero. project-memory gives it a memory that carries over:

- **A journal of every exchange**, kept on your computer. Ask about earlier work in your own words and Claude finds it, with the date.
- **Picks up where you stopped.** A new conversation starts already knowing what the last one was doing.
- **Nothing is lost.** Every version of Claude's notes is kept, so a deleted or overwritten note can come back.
- **Long tasks stay on track** when a conversation is cut down to a summary.
- **Lessons shared across projects**, and two Claude windows on one project without overwriting each other.

```
/plugin marketplace add zdraveski/project-memory
/plugin install project-memory@project-memory
```

[![release](https://img.shields.io/github/v/release/zdraveski/project-memory?label=release)](https://github.com/zdraveski/project-memory/releases/latest) [![tests](https://img.shields.io/github/actions/workflow/status/zdraveski/project-memory/test.yml?branch=master&label=tests)](https://github.com/zdraveski/project-memory/actions/workflows/test.yml) [![OpenSSF Best Practices](https://www.bestpractices.dev/projects/16158/badge)](https://www.bestpractices.dev/projects/16158)

---

#### 🔋 [claude-juice](https://github.com/zdraveski/claude-juice) · [live customizer](https://zdraveski.github.io/claude-juice/web/)

**Your Claude Code usage limits as little batteries under your prompt.**

- **Four batteries:** the 5-hour session, the weekly limit, the Fable limit, and how full the current chat is.
- **Counts like Anthropic's usage page** and shows when each limit resets.
- **Warns you before you run out**, with `!` and `!!`.
- **12 ready-made looks and 13 colour sets.** Try them all in the browser before installing.
- **One-step undo:** `/juice restore` brings back your old status line.

```
/plugin marketplace add zdraveski/claude-juice
/plugin install juice@juice
```

[![release](https://img.shields.io/github/v/release/zdraveski/claude-juice?label=release)](https://github.com/zdraveski/claude-juice/releases/latest) [![tests](https://github.com/zdraveski/claude-juice/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/zdraveski/claude-juice/actions/workflows/test.yml)

---

#### How I work

- **Tested on three systems.** Every change runs the full test suite on Windows, macOS and Linux.
- **Mutation testing.** project-memory deliberately breaks its own code, about 1,170 ways, to check the tests notice every one. A change can't merge while a break in the code it touches goes unnoticed.
- **Security checks.** Both projects are scanned by CodeQL. project-memory also runs dependency review and [zizmor](https://github.com/zizmorcore/zizmor) on its GitHub workflows, with every action pinned to an exact version.
- **Small releases with changelogs**, so you can see what changed and why.

#### Get in touch

Found a bug or have an idea? Open an issue in the project's repository; bug reports, questions and pull requests are all welcome. Both projects are MIT-licensed.

<sub>These are independent projects, not made by or affiliated with Anthropic. "Claude" and "Claude Code" are Anthropic's names.</sub>
