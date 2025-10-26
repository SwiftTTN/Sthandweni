# GitHub Explained Simply - For Beginners

## What is GitHub?

Think of GitHub as a special filing cabinet for your code and project files. It keeps track of every change you make, lets you work from different computers, and helps you not lose your work.

**Important:** GitHub is NOT like Google Drive or Dropbox. It's specifically designed for code projects, not for backing up your entire computer.

---

## GitHub's Storage Rules (The Limits)

### Individual File Sizes

Think of it like email attachments - there are size limits:

- **Files under 50 MB** → ✅ No problem, GitHub is happy
- **Files 50-100 MB** → ⚠️ GitHub warns you but allows it
- **Files over 100 MB** → ❌ GitHub blocks them (won't let you upload)
- **Uploading through website** → Max 25 MB only

**In Simple Terms:**
- Small files (documents, code, pictures) = Perfect ✅
- Medium files (small videos, large images) = Use carefully ⚠️
- Big files (movies, game files, large videos) = Not allowed ❌

### Total Repository Size

A "repository" (or "repo") is your entire project folder.

- **Under 1 GB** → ✅ Perfect size, everything runs smoothly
- **1-5 GB** → ⚠️ Still okay but getting big
- **5-10 GB** → ⚠️ GitHub complains, things slow down
- **Over 10 GB** → ❌ GitHub may block or have serious problems

**Real World Comparison:**
- 1 GB = About 500 photos or 250 songs
- 10 GB = About 2-3 movies or 1 small video game

---

## What Can You Store? (File Types)

### ✅ Great for GitHub (Recommended)

**Code Files:**
- `.js`, `.py`, `.java`, `.cpp`, `.html`, `.css` - Any programming code
- `.json`, `.xml`, `.yaml` - Configuration files
- `.md` - Documentation files (like this one!)

**Small Media:**
- `.png`, `.jpg`, `.svg` - Images under 5 MB
- `.gif` - Small animations

**Documents:**
- `.txt` - Text files
- `.csv` - Spreadsheet data
- Small `.pdf` files (under 10 MB)

### ⚠️ Use With Caution

**Larger Files:**
- Videos under 50 MB
- PDF books/documents (10-50 MB)
- Audio files
- Large datasets

### ❌ Don't Put These on GitHub

**Too Big:**
- Movies and large videos
- ISO files (disc images)
- Large zip files
- Game files
- Virtual machine images

**Security Risks:**
- Passwords
- API keys
- Private certificates
- Personal data

**Not Suitable:**
- Your entire photo collection
- Music library
- Software installers
- Complete computer backups

---

## How Much Can You Upload at Once?

- **Per upload (push):** Maximum 2 GB at a time
- **Per minute:** Don't upload more than 6 times (GitHub gets upset)

**Think of it like:**
Uploading to GitHub is like using a narrow pipe - you can't dump everything at once!

---

## Other Rules to Know

### Repository Structure Limits

- **Maximum branches:** 5,000 (branches are different versions of your project)
- **Files per folder:** 3,000 maximum
- **Nested folders:** 50 levels deep maximum

**In Simple Terms:**
Don't go crazy with organization - keep it simple!

---

## So... Can I Use GitHub as My Backup Drive?

### Short Answer: **NO** ❌

### Why Not?

| What You Want | GitHub Limit | Google Drive (Free) |
|---------------|--------------|---------------------|
| Total Storage | 10 GB max | 15 GB free |
| File Size | 100 MB max | Unlimited! |
| Big Videos | ❌ Blocked | ✅ Works great |
| Photos | ⚠️ Only small ones | ✅ No problem |
| Documents | ✅ Perfect | ✅ Perfect |

**GitHub is for:**
- 📁 Code projects (like websites, apps, scripts)
- 📝 Writing and documentation
- 🔧 Configuration files
- 🎯 Your Olympic weightlifting tracker project!

**Use these for general backup instead:**
- **Google Drive** - 15 GB free, great for photos/docs
- **Dropbox** - Easy to use, good for any files
- **OneDrive** - 5 GB free, built into Windows
- **iCloud** - If you use Apple devices
- **External hard drive** - Best for large backups

---

## GitHub's Sweet Spot

GitHub is PERFECT for projects like yours (Olympic weightlifting) where you have:
- ✅ Code files
- ✅ Small images (logos, icons)
- ✅ Documentation
- ✅ Configuration files
- ✅ Data in CSV or JSON format
- ✅ Need to work from multiple devices

---

## Quick Tips for New Users

1. **Keep files small** - If a file is over 10 MB, ask yourself if it really needs to be in GitHub
2. **Don't store secrets** - Never put passwords or API keys in your code
3. **Push often** - Save your work to GitHub frequently (we set this up in claude.md!)
4. **Use .gitignore** - Tell GitHub to ignore certain files (like huge datasets)
5. **Stay under 1 GB** - Keep your whole project under 1 GB if possible

---

## What Happens If You Break the Rules?

- **File too big (>100 MB):** GitHub rejects it with an error message
- **Repo too big (>10 GB):** Everything gets slow, cloning fails, GitHub may contact you
- **Push too big (>2 GB):** Upload fails completely
- **Too many pushes:** GitHub temporarily blocks you (rare)

**Don't Panic!** These limits are hard to hit if you're using GitHub correctly for code projects.

---

## Bottom Line

Think of GitHub as a **specialized tool for code projects**, not a general backup service.

**For your Olympic weightlifting project:**
- Store code, scripts, and data files → Perfect! ✅
- Store workout photos → Only small ones (compress them first) ⚠️
- Store training videos → Use YouTube or Google Drive instead ❌

---

---

# GitHub Gists & Personal Access Tokens - For Data Sync

## What is a GitHub Gist?

Think of a **Gist** as a special GitHub note-taking tool, like posting a single sticky note on GitHub instead of creating an entire project folder.

**Real-world analogy:**
- Regular GitHub = Your entire filing cabinet (lots of folders, documents, organization)
- Gist = A single piece of paper you stick on the wall (quick, simple, just one thing)

**Why use it for your nutrition tracker?**
- ✅ Stores your daily nutrition data (JSON format)
- ✅ Can be public or private
- ✅ Syncs across all your devices
- ✅ Free (no cost)
- ✅ Easy to update from your webpage

---

## What is a Personal Access Token (PAT)?

A **Personal Access Token** is like a special password that gives your webpage **permission** to access your GitHub Gist and save/update data.

**Analogy:**
Imagine you have a locked diary. Instead of giving someone your actual password, you write a special "permission letter" that says:
- "This person can read and write in my diary"
- "This letter expires on [date]"
- "This letter only works for [specific things]"

A PAT is exactly that - a special permission slip for your webpage.

**Why not just use your GitHub password?**
- ❌ If you put your real password in code, anyone can see it and take over your account
- ✅ PAT is limited - even if someone gets it, they can only do specific things (like update one Gist)
- ✅ You can delete it anytime without changing your password
- ✅ More secure for sharing code

---

## Step-by-Step: Create Your Personal Access Token

### Step 1: Go to GitHub Settings

1. Open GitHub: https://github.com
2. Click your **profile picture** (top right)
3. Click **Settings**

### Step 2: Find Developer Settings

1. Scroll down the left menu
2. Click **Developer settings** (near the bottom)
3. Click **Personal access tokens**
4. Click **Tokens (classic)**

### Step 3: Generate New Token

1. Click **Generate new token (classic)** button
2. You might need to confirm your password - do that

### Step 4: Configure Your Token

You'll see a form. Fill it out like this:

| Field | What to Enter |
|-------|---------------|
| **Note** | `Nutrition Tracker` (just a name so you remember what it's for) |
| **Expiration** | `No expiration` (or pick a date if you prefer) |
| **Select scopes** | Check ONLY the `gist` box (nothing else!) |

**What does "gist scope" mean?**
- It means this token can ONLY create/read/update Gists
- It CANNOT access your code, repositories, or anything else
- This keeps you safe!

### Step 5: Copy Your Token

1. Click **Generate token**
2. You'll see a long string of letters/numbers: `ghp_aBcDeFgHiJkLmNoPqRsTuVwXyZ...`
3. **Copy this immediately** and save it somewhere safe (like a notes app)
   - ⚠️ GitHub will NEVER show it again after you leave this page
   - If you lose it, you'll have to create a new one

**Important:** Keep this token private! Don't share it or put it in public code.

---

## Step-by-Step: Create Your Nutrition Gist

### Step 1: Go to Gists

1. Open: https://gist.github.com
2. Click **Create a new gist**

### Step 2: Set Up Your Gist

| Field | What to Enter |
|-------|---------------|
| **Filename** | `nutrition-tracker.json` |
| **File content** | Paste this exactly: `{"entries": []}` |
| **Description** | `My nutrition tracking data for Olympic weightlifting` |

### Step 3: Make It Public

- Look for the radio buttons at the bottom
- Select **Public** (not Secret)
  - Why public? The GitHub API is easier to use with public Gists
  - Your data is just nutrition info, nothing private

### Step 4: Create It

1. Click **Create public gist**
2. You'll see your new Gist with a URL like: `https://gist.github.com/yourusername/abc123xyz`

### Step 5: Save Your Gist ID

The Gist ID is the part after the last `/` in the URL.

**Example:**
- Full URL: `https://gist.github.com/sarah/a1b2c3d4e5f6g7h8`
- Gist ID: `a1b2c3d4e5f6g7h8`

Save this somewhere (you'll need it in the next step).

---

## What These Do (Put It All Together)

Once you have:
1. ✅ **Personal Access Token** (your permission slip)
2. ✅ **Gist ID** (where your data lives)
3. ✅ **Nutrition webpage** (your tracker interface)

Your webpage will:
- 📤 **Save** your daily nutrition entries to the Gist
- 📥 **Load** previous entries when you visit
- 🔄 **Sync** across all your devices (phone, laptop, tablet)
- 📊 **Export** everything as CSV (spreadsheet file)

---

## Ready for the Next Step?

Once you have both:
- Your **Personal Access Token** (example: `ghp_xxxx...`)
- Your **Gist ID** (example: `a1b2c3d4e5f6`)

Tell me, and I'll update your nutrition webpage to use them!

---

## Need Help?

- Check [claude.md](claude.md) for workflow guidelines
- GitHub Docs: https://docs.github.com
- Ask Claude (me!) anytime you're confused

---

*Created for absolute beginners - no technical knowledge required!*
