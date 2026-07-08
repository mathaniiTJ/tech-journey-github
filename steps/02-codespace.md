# Step 2: Launch a Codespace

**Previous step:** [Step 1 - Fork the Repo](01-fork.md)
**Next step:** [Step 3 - Set Up GitHub Copilot](03-copilot.md)

---

## You Have a Copy — Now You Need a Workshop

In Step 1 you forked the repo, so you own a copy of the files. Now you need a place to actually *work* on them. That place is a **Codespace**: a full development environment that GitHub runs for you in the cloud and opens right in your browser.

No installing anything. No setup on your own computer. You click a button and a real developer machine appears in a browser tab.

---

## What Is a Codespace?

A Codespace is **Visual Studio Code** — the editor millions of professional developers use — running on a real computer in the cloud. Because it is a real computer, it can:

- Edit and create files
- Run a real **terminal** (command line)
- Run code (Python, JavaScript, and more)
- Install extensions — including **GitHub Copilot**, the AI assistant you will set up in Step 3

> GitHub also has a lighter-weight editor called **github.dev** (you open it by pressing `.` on a repo). It is handy for quick edits, but it *cannot run code or use Copilot*. This course uses a Codespace so you get the full experience.

---

## Is It Free?

Yes. Personal GitHub accounts get a **generous free monthly allowance** for Codespaces (at the time of writing, 120 core-hours and 15 GB of storage per month — far more than this course needs). You will not be charged as long as you stay within it.

Two habits keep you safely inside the free allowance:
- **Stop your Codespace when you finish** (see the bottom of this page).
- **Do not leave many Codespaces running** at once.

---

## Your Task: Create a Codespace

1. Go to your forked repository on **github.com** (the page with *your* username in the address bar).
2. Click the green **`< > Code`** button near the top-right.
3. In the dropdown, click the **Codespaces** tab.
4. Click **Create codespace on main**.

GitHub now builds your cloud computer. The first time takes a minute or two — you will see a screen with build logs. When it finishes, a full VS Code editor opens in your browser.

> You are creating this Codespace on the `main` branch for now. That is fine — in Step 4 you will create your own branch from right inside the Codespace.

---

## Getting to Know Your Codespace

Once it loads, you will see:

- **Left sidebar** — the file explorer. Click any file to open it.
- **Main area** — the editor where you read and write files.
- **A terminal at the bottom** — this is a real command line. If you do not see it, open it from the menu: **Terminal → New Terminal** (or press `` Ctrl+` ``).
- **Bottom-left corner** — shows your current branch name (`main` for now).

Try the terminal out. Click into it, type the command below, and press Enter:

```bash
git status
```

You just ran a real git command on a real machine in the cloud. This is the exact workflow professional developers use every day.

---

## How to Know You Did It

- The browser tab shows your repo name and the word **Codespaces**.
- There is a working **terminal** at the bottom that responds to commands.
- The file explorer on the left shows the repo files, including the `exercises` and `steps` folders.

---

## Important: Stop Your Codespace When You Are Done

Your Codespace uses your free hours while it is running. When you finish a work session, **stop it** so you do not waste your allowance:

1. Go to **[github.com/codespaces](https://github.com/codespaces)**.
2. Find your Codespace in the list.
3. Click the **`...`** menu next to it and choose **Stop codespace**.

A stopped Codespace keeps all your files and picks up right where you left off next time — it just stops the clock. Codespaces also stop themselves automatically after about 30 minutes of inactivity, so you are protected even if you forget.

> **Do not delete your Codespace until your work is committed and pushed** (Step 6). Stopping is safe; deleting an uncommitted Codespace loses your work.

---

**You completed Step 2!** Head to [Step 3 - Set Up GitHub Copilot](03-copilot.md).
