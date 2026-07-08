# Step 6: Commit and Push

**Previous step:** [Step 5 - Create Your File](05-create-file.md)
**Next step:** [Step 7 - Open a Pull Request](07-pull-request.md)

---

## What Is a Commit?

A **commit** is a snapshot saved in git's history — a labeled save point that you can return to at any time.

Every commit has two parts:
1. **The changes** — which files changed and exactly what changed
2. **The commit message** — a short description of *why* you made these changes

Over time, your commit history becomes a log of everything that happened to your project and why. This is incredibly useful when something breaks and you need to trace it back.

### Commit vs. Push

In your Codespace these are **two separate actions** (just like on a professional developer's machine):

- **Commit** saves the snapshot *inside your Codespace*.
- **Push** sends your commits *up to GitHub* so they are backed up and visible online.

You will do both in this step.

---

## How to Write a Good Commit Message

A commit message should describe what changed, not just say "stuff" or "changes." Here are some examples:

| Bad | Better |
|-----|--------|
| `stuff` | `Add about-me file` |
| `changes` | `Update introduction section` |
| `asdfasdf` | `Fix typo in README` |
| `final` | `Complete step 5 exercise` |

A few conventions professionals follow:
- Use the **imperative mood**: "Add" not "Added", "Fix" not "Fixed"
- Keep it **under 72 characters**
- Capitalize the first word

> **🤖 Ask Copilot:** Open Copilot Chat and ask: *"Suggest a good git commit message for adding a new file called about-me.md, and explain why it is written that way."* Notice how it uses the imperative mood.

---

## Your Task: Commit and Push in the Codespace

### Step 1: Open Source Control

Click the **Source Control icon** in the left sidebar. Your `exercises/about-me.md` should already be under **Staged Changes** from Step 5. (If it is under **Changes** instead, click the `+` to stage it first.)

### Step 2: Write your commit message

At the top of the Source Control panel, there is a text box that says **"Message"**. Type a descriptive message, for example:

```
Add about-me file
```

### Step 3: Commit

Click the blue **Commit** button (or press **Ctrl+Enter**). This saves the snapshot inside your Codespace.

### Step 4: Push

After committing, the blue button changes to **Sync Changes** (or **Publish Branch** the very first time you push a new branch). Click it to send your commit up to GitHub.

> If you see **Publish Branch**, click it — since `add-about-me` is a brand-new branch, this creates it on GitHub and pushes your commit in one click.

---

## How to Know You Did It

- The Source Control panel shows **no pending changes** (the numbered badge is gone).
- On **github.com**, go to your fork, switch the branch dropdown to `add-about-me`, and you should see `exercises/about-me.md` in the file list.

> **CLI Alternative (optional, for the curious)**
>
> In the terminal, commit and push are two commands:
> ```bash
> git commit -m "Add about-me file"
> git push -u origin add-about-me
> ```
> `git commit` saves the snapshot locally; `git push` sends it to GitHub. The `-u origin add-about-me` part is only needed the first time you push a new branch.

---

## Check the Automated Validation

1. On your fork on GitHub, click the **Actions** tab.
2. You should see a workflow run called **"Steps 5-6 Check"** triggered by your push.
3. Wait 30-60 seconds for it to finish.
4. A green checkmark means you passed. A red X means something needs fixing — click into the run to read the error message.

---

**You completed Step 6!** Head to [Step 7 - Open a Pull Request](07-pull-request.md).
