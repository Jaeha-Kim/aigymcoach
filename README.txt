GYM SESSION COACH - YOUR OWN COPY FOR iPAD
==========================================

What this is
- The whole app, set up to install on your iPad Home Screen and run offline.
- Your log is stored on the iPad itself. Nothing depends on Claude.
- It needs a free web address (GitHub Pages) only so Safari can install it once.
  Your workout data never goes there: only these app files do.

Files in this folder (upload all of them, keep the names)
  index.html             the app
  sw.js                  makes it work offline
  manifest.webmanifest   makes it installable
  icon-180.png, icon-192.png, icon-512.png   Home Screen icon
  xlsx.full.min.js       Excel export library, so export works offline
  xlsx-LICENSE.txt       that library's license


STEP 1 - Put it online (once, about 5 minutes, on your Mac)
1. Go to github.com and create a free account (or sign in).
2. Click "+" (top right) > New repository.
   Name: gym-coach    Visibility: Public    Click "Create repository".
3. On the new repository's page, click "uploading an existing file".
4. Drag in ALL the files from this folder (not the folder itself). Click "Commit changes".
5. Go to Settings > Pages. Under "Branch", choose "main" and "/ (root)", then Save.
6. Wait 1-2 minutes and refresh. GitHub shows your address, like:
      https://YOUR-USERNAME.github.io/gym-coach/

STEP 2 - Install it on your iPad
1. Open that address in Safari on the iPad.
2. Tap Share > "Add to Home Screen" > Add.
3. From now on, ALWAYS open it from the Home Screen icon (not from Safari).
   The Home Screen app and Safari keep separate logs.
4. Optional check: turn on Airplane Mode and open it. It should still work.

STEP 3 - Bring over anything you already logged (optional)
1. In the claude.ai version: More > Back up all data > Save to Files.
2. In your Home Screen app: More > Restore from a backup > pick that file.

Keeping your log safe
- At the end of each workout, tap "Save a backup of your log" and choose
  "Save to Files" (iCloud Drive is a good place). That file restores everything.
- Don't delete the Home Screen app: deleting it deletes the log stored inside it.
  If that ever happens, reinstall (Step 2) and restore your latest backup.

Updating the app later
- Upload the new index.html to the same repository (replace the old one).
- Open sw.js on GitHub (pencil icon), change "gym-coach-v1" to "gym-coach-v2", commit.
- Open the Home Screen app twice while online; the update loads. Your log is kept.
