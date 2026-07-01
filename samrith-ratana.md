# Git CLI Exercises

## Exercise 1: The Setup

### Initialize

Create your first repository

Open your terminal, create a brand new folder, and tell Git to start tracking it.

**Step 1:**

```bash
mkdir my-first-repo
```

**Step 2:**

```bash
cd my-first-repo
```

**Step 3:**

```bash
git init
```

---

## Exercise 2: Staging Changes

### Status & Add

Prepare files for saving

Create a file, check what Git sees, and then tell Git to stage the file.

**Step 1:** Create a file named `notes.txt`

**Step 2:**

```bash
git status
```

(Notice the red text)

**Step 3:**

```bash
git add notes.txt
```

**Step 4:**

```bash
git status
```

(Notice the green text)

---

## Exercise 3: The Save Point

### Commit

Lock in your progress

Now that your file is staged (green), you must take the snapshot to save it permanently in your ledger.

**Step 1:**

```bash
git commit -m "Created initial notes file"
```

**Step 2:**

```bash
git status
```

(It should now say `nothing to commit, working tree clean`.)

---

## Exercise 4: Time Travel

### Check History

View your cryptographic ledger

Prove that your save point worked by viewing the repository's history and finding your commit message.

**Step 1:**

```bash
git log
```

Look at the output. You will see a long hash string, the author (you), the date, and your message:

`Created initial notes file`

---

## Exercise 5: Parallel Worlds

### Branching

Create a safe space to experiment

Create an isolated copy of your code so you can make changes without affecting the main file.

**Step 1:**

```bash
git branch new-idea
```

**Step 2:**

```bash
git checkout new-idea
```

**Pro Tip Shortcut:**

```bash
git checkout -b new-idea
```

(Does both at once!)
