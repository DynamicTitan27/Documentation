This document contains every terminal command, Git workflow, VS Code shortcut, and official documentation link needed to build, debug, and submit the full-stack lab exam.

---

## 1. NPM & Project Setup Commands
Run these in your terminal to initialize the project and install dependencies.

* **Initialize project (creates package.json):**
  `npm init -y`
* **Install core backend packages:**
  `npm install express mongoose`
* **Install auto-restarting developer tool:**
  `npm install -D nodemon`
* **Start the server normally:**
  `node server.js`
* **Start the server with auto-restart (Recommended):**
  `npx nodemon server.js`
* **The Panic Button (Clean Reinstall):**
  If packages break, delete the folder and reinstall:
  1. `rm -rf node_modules package-lock.json`
  2. `npm install`

---

## 2. Git & GitHub Commands
Use these commands to back up your code and upload it to your repository.

* **Clone an existing repository to your computer:**
  `git clone <insert-github-repo-url-here>`
* **Initialize a new local repository (if starting from scratch):**
  `git init`
* **Check the status of your files (Red = unsaved, Green = ready to save):**
  `git status`
* **Stage all changes:**
  `git add .`
* **Commit (Save) your changes with a message:**
  `git commit -m "Finished the Express routes"`
* **Push (Upload) your code to GitHub:**
  `git push origin main` 
  *(Note: If it's your first time pushing a new repo, use: `git push -u origin main`)*

---

## 3. Using GitHub Directly in VS Code (UI Method)
If you forget terminal commands, you can use Visual Studio Code's built-in tools.

1. **Sign In:** Click the Accounts Icon (bottom-left gear area) > Turn on Settings Sync > Sign in with your GitHub account.
2. **Source Control Tab:** Press `Ctrl + Shift + G` (or `Cmd + Shift + G` on Mac) to open the Source Control panel on the left.
3. **Stage Changes:** Click the `+` icon next to the files you changed.
4. **Commit:** Type your save message in the text box and click the Commit button.
5. **Push:** Click the Sync Changes button (or "Push" in the three-dot menu) to upload to GitHub.

---

## 4. VS Code Terminal Management
Keep your workspace clean and kill frozen servers.

* **Stop a running server:**
  `Ctrl + C` (Press inside the terminal).
* **Clear the terminal screen:**
  * Mac/Linux: Type `clear` and press Enter (or press `Cmd + K`).
  * Windows: Type `cls` and press Enter.
* **Limit Command History to 5 (Windows PowerShell in VS Code):**
  `$MaximumHistoryCount = 5`
  *(Run this to restrict your up-arrow command history to only the last 5 entries for the current session.)*
* **Limit Command History to 5 (Windows CMD in VS Code):**
  `doskey /listsize=5`
* **Delete VS Code Terminal History completely:**
  To completely wipe the terminal instance, click the Trash Can Icon (Kill Terminal) on the top right of the terminal panel, then open a fresh one with ` Ctrl + ` ` (backtick).
* **Toggle Terminal Window:**
  ` Ctrl + ` ` (The key above Tab).

---

## 5. General File & Folder Commands
Navigate your computer without leaving the keyboard.

* **List all files in the current folder:**
  `ls` (Mac/Linux) or `dir` (Windows)
* **Move into a folder:**
  `cd folder_name`
* **Go back one folder:**
  `cd ..`
* **Create a new folder:**
  `mkdir folder_name`
* **Create new files:**
  * Mac/Linux: `touch server.js index.html`
  * Windows: `echo. > server.js`

---

## 6. Official Documentation Links (For Code Snippets)
Keep these tabs open during the exam to quickly copy and paste boilerplate code.

* **Express.js (Backend Setup & Routing)**
  * Hello World / Server Setup: `https://expressjs.com/en/starter/hello-world.html`
  * Serving Static Files (HTML/CSS): `https://expressjs.com/en/starter/static-files.html`
  * Routing (GET/POST logic): `https://expressjs.com/en/guide/routing.html`

* **Mongoose (Database Connection & Models)**
  * Quick Start (Connection string & basic schema): `https://mongoosejs.com/docs/index.html`
  * Defining Schemas: `https://mongoosejs.com/docs/guide.html`

* **MDN Web Docs (Frontend JavaScript & Validation)**
  * Fetch API (Sending data to server): `https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch`
  * DOM Manipulation: `https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Manipulating_documents`

* **Bootstrap (Frontend Styling & Forms)**
  * Quick Start Template: `https://getbootstrap.com/docs/5.3/getting-started/introduction/`
  * Form Components: `https://getbootstrap.com/docs/5.3/forms/overview/`

  Open MongoDB Compass from your Windows Start Menu.

In the URI connection box, paste:
mongodb://localhost:27017
(Alternatively: mongodb://127.0.0.1:27017)

Click Connect.

Click your database name (e.g., SmartLibrarySystem1DB) on the left to view your collections and JSON documents.
