# Step 5: Create Your File

**Previous step:** [Step 4 - Create a Branch](04-branch.md)
**Next step:** [Step 6 - Commit and Push](06-commit.md)

---

## The Staging Area

Git does not automatically save every change you make. Before you can save a snapshot (a "commit"), you have to tell git which changes to include. This is called **staging**.

Think of it like packing a box to ship:
- Staging puts items in the box.
- Committing (next step) seals the box and writes a label on it.
- You can add and remove items from the box before you seal it.

This two-step process lets you make multiple changes and choose exactly which ones to save together — keeping your history clean and organized.

### The Three States of a File

| State | Meaning |
|-------|---------|
| **Untracked** | Git sees the file exists but is not watching it |
| **Modified** | A tracked file has changed but is not staged yet |
| **Staged** | The file is in the "box" ready to be committed |

---

## Your Task: Create Your About Me File

### Step 1: Open the exercises folder

In the file explorer on the left sidebar, click the `exercises` folder to expand it. You will see `README.md` and `about-me-template.md` inside. Open `about-me-template.md` to use as a reference.

### Step 2: Create a new file

1. Hover over the `exercises` folder in the sidebar.
2. Click the **New File** icon (a page with a `+` sign).
3. Type `about-me.md` and press Enter.

The new file opens in the editor. Make sure the path shown at the top says `exercises/about-me.md`.

### Step 3: Add your content

Your file must contain:
1. A line that says `## About Me` (exactly this heading)
2. At least a few lines about yourself

Here is a starter template — paste this in and fill it out:

```markdown
## About Me

**Name:** [Your name or a nickname]

**Why I joined Tech Journey:**
[Write 1-2 sentences]

**Something I am interested in:**
[A hobby, subject, game, sport — anything]

**One thing I hope to learn:**
[What do you want to be able to do after this program?]
```

> **🤖 Ask Copilot:** This is a great place to try Copilot's **inline suggestions**. Type a line like `**Something I am interested in:**` and then press Enter — watch for the grey ghost text. Or open Copilot Chat and ask: *"Help me write a friendly one-sentence intro for a student who likes robotics and basketball."* Then edit the result to make it truly *yours* — Copilot gives you a starting point, not the final word.

### Step 4: Save the file

Press **Ctrl+S** (Windows/Linux) or **Cmd+S** (Mac) to save.

---

## Step 5: Stage the File

Unlike a quick browser editor, a real Codespace does **not** automatically stage your changes when you save — you do it yourself. This is the real staging step.

1. Click the **Source Control icon** in the left sidebar (a branching icon with a numbered badge).
2. You will see `about-me.md` listed under **Changes**.
3. Hover over `about-me.md` and click the **`+`** (plus) icon to stage it.
4. The file moves up into a **Staged Changes** section. It is now in the "box," ready to commit.

> **CLI Alternative (optional, for the curious)**
>
> In the terminal you can stage the file with one command:
> ```bash
> git add exercises/about-me.md
> ```
> Then check what is staged with `git status` — your file appears under "Changes to be committed."

---

## How to Know You Did It

In the Source Control panel, `exercises/about-me.md` appears under **Staged Changes**. If you see it there, you are ready to commit.

---

## Automated Check

When you commit and push (Step 6), the **Steps 5-6 Check** workflow runs and verifies:
- `exercises/about-me.md` exists
- It contains the `## About Me` heading
- It has at least 3 lines of content

If something is wrong, the error message in the Actions tab will tell you exactly what to fix.

---

**You completed Step 5!** Head to [Step 6 - Commit and Push](06-commit.md).
