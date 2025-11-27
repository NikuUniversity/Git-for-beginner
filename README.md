# Git Subtree Guide 🌳

This project uses **Git Subtree** to manage a folder that is actually a separate repository. 
This allows us to keep the code in that folder synced with its original source.

## 📂 Project Structure
- `main-project/` (This repository)
  - `library-folder/` (The Subtree: A separate repo living inside here)
  - `index.html`
  - `README.md`

---

## 🛠️ Cheat Sheet Commands

### 1. How to ADD a Subtree (Do this once)
Use this command to download the external repo into a folder for the first time.
*Replace the URL and folder name with your specific details.*

```bash
git subtree add --prefix=library-folder [https://github.com/username/other-repo.git](https://github.com/username/other-repo.git) main --squash
