# 📂 FilmMarketLive Git Cheat Sheet (Backup & Version Control)

A quick and clean reference for backing up your site using Git & GitHub.

---

## 🟢 Initial Setup (Only once per project)

```bash
git init                                      # Initialize Git in the folder
git remote add origin https://github.com/jrsti06/filmmarketlive.git
git branch -M main                           # Rename default branch to 'main'
```
MY TWO GIT REMOTE OPTIONS (JR)

A -- Searching for what REMOTE URL:
git remote -v

BACKUP
git remote set-url origin https://github.com/jrsti06/jr-backups.git

ORIGINAL
git remote set-url origin https://github.com/jrsti06/filmmarketlive.git

---

## 💾 Save Your Work (Every time you make changes)

```bash
git add .                                     # Stage all changed files
git commit -m "Describe what changed"       # Commit with a message
git push origin main                         # Push to your GitHub repo
```

Examples:

```bash
git commit -m "Fixed mobile nav bug"
git commit -m "Added new article for Mooch premiere"
```

---

## 🏷 Optional: Tag a Backup Version

Use this to save specific versions of your site with easy reference tags.

```bash
git tag v1                                    # Create tag (use custom name)
git push origin v1                            # Push tag to GitHub
```

To view tags:

```bash
git tag
```

---

## 🔁 If You See Push Errors

If you get a message like `Updates were rejected...`:

```bash
git pull origin main --rebase                 # Safely update local repo first
# OR if you're confident:
git push --force origin main                  # Force push (overwrites remote)
```

---

## 🔙 Want a Version History?

Use this to view your commit history:

```bash
git log --oneline                             # Compact history log
```

---

## 🧠 Tips

* Keep this file saved as `README.md` in your main project folder.
* Commit **before** pushing changes to Netlify.
* Add clear messages so you remember what each backup was.
* You can also view Git visually in VS Code using extensions like **Git Graph**.

---

Happy backing up! ✨
