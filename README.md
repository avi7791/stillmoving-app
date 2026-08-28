# Still Moving — The Jaipur Challenge Web App

## What this is
A mobile-first web app for the Still Moving virtual fitness challenge platform.
Participants track their progress on the Jaipur Challenge (50km in 30 days).

## Features
- Participant login with registration code
- Activity logging (distance, type, RPE, notes)
- Visual progress bar along the Jaipur route
- Milestone unlocks at 10/20/30/40/50km with articles
- Leaderboard showing all participants
- Admin panel with CSV export
- Works on any phone browser (Android + iPhone)
- installable as home screen app (PWA)

## How to deploy FREE on Vercel

### Step 1 — Create GitHub account
Go to github.com and create a free account

### Step 2 — Create a new repository
- Click "New repository"
- Name it "stillmoving-app"
- Set to Public
- Click "Create repository"

### Step 3 — Upload files
- Click "uploading an existing file"
- Upload all files from this folder:
  - index.html
  - manifest.json
  - logo.png
  - README.md
- Commit changes

### Step 4 — Deploy on Vercel
- Go to vercel.com
- Sign up with your GitHub account
- Click "New Project"
- Import your "stillmoving-app" repository
- Click Deploy
- Done! Your app is live at yourname.vercel.app

### Step 5 — Share with beta testers
Send them:
- Your Vercel URL
- Their registration code (SM1001, SM1002 etc)
- Their name to use on login

## Registration Codes
Current valid codes: SM1001 through SM1015
Admin code: ADMIN1
Admin password: stillmoving2026

TO ADD MORE CODES:
Open index.html, find the VALID_CODES array and add more codes.

## Admin Panel
- Open the app
- Click "Admin Login"
- Password: stillmoving2026
- See all participants, their progress, export CSV

## Customising for future challenges
To change the challenge (e.g. Manali to Leh):
1. Update CHALLENGE object (name, totalKm, days)
2. Update MILESTONES array (km, landmark, emoji, text)
3. Update LOCATION_NAMES array
4. Update total km references (currently 50)

## Tech stack
- Pure HTML/CSS/JavaScript (no framework needed)
- Data stored in browser localStorage
- No backend needed for beta
- PWA manifest for home screen install

## Next steps after beta
- Move to Supabase backend (free tier) for shared data
- Add Razorpay payment integration
- Add email notifications for milestones
- Build Manali-Leh challenge as second event
