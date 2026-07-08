# Step 4: Create a Branch

**Previous step:** [Step 3 - Set Up GitHub Copilot](03-copilot.md)
**Next step:** [Step 5 - Create Your File](05-create-file.md)

---

## What Is a Branch?

A **branch** is a parallel timeline of your code.

Imagine you are writing a paper and you want to try a completely different introduction. Instead of deleting your current one and hoping you remember it, you make a photocopy. You write on the copy, and if you like it, you swap it in. If you hate it, throw away the copy — your original is untouched.

Branches work like that. You can have many branches at once and switch between them instantly.

### The `main` Branch

Every repository has a default branch called `main`. Think of it as the "official" version — the one that is always stable. You never work directly on `main`. Instead, you create a new branch for each piece of work, do your work there, and then merge it back into `main` when it is ready.

This is how professional developers work every day.

> **🤖 Ask Copilot:** Open Copilot Chat and ask: *"Why do developers create a new branch instead of working directly on main?"* Compare its answer to what you just read.

---

## Your Task: Create a Branch

You need to create a branch called exactly **`add-about-me`**. This name is important — the automated check looks for it.

### Option 1: In the Codespace editor (recommended)

1. Look at the **bottom-left corner** of the editor. You will see the current branch name — it says `main`.
2. Click on `main`.
3. A menu appears at the top of the screen. Click **"Create new branch..."**.
4. Type `add-about-me` and press Enter.
5. If asked, confirm switching to the new branch.

The bottom-left corner now shows `add-about-me`. You are on your new branch.

### Option 2: In the terminal

Because a Codespace has a real terminal, you can also do it the way professionals often do — with a single command. Open the terminal (**Terminal → New Terminal**) and run:

```bash
git checkout -b add-about-me
```

This creates the branch and switches to it in one step. Verify it worked with:

```bash
git branch
```

The branch with a `*` next to it is the one you are on — it should be `add-about-me`.

---

## Branch Naming Tips

Good branch names are:
- **Lowercase** with hyphens between words (`add-about-me`, not `Add About Me`)
- **Short and descriptive** — someone should be able to guess what the branch is for
- **Action-oriented** — start with a verb like `add-`, `fix-`, `update-`

Avoid generic names like `my-branch`, `test`, or `stuff`.

---

## How to Know You Did It

The **bottom-left corner** of the editor shows `add-about-me` instead of `main`. If you used the terminal, `git branch` shows a `*` next to `add-about-me`.

---

**You completed Step 4!** Head to [Step 5 - Create Your File](05-create-file.md).
