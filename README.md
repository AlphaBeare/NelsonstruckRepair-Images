# NelsonstruckRepair-Images
How to Replace Photos in GitHub (Browser Only)

1. Sign in and open the repository

Go to https://github.com/AlphaBeare/NelsonstruckRepair-Images
Make sure you are signed in with the GitHub account that was added as a collaborator (look at the top-right of the page; it should show your profile picture).


2. Locate the existing photo

In the repository file list, navigate through the folders until you find the photo you want to replace.
Example: if the photo is stored in work/truck.jpg, click on the work folder, then click truck.jpg.


3. Upload the replacement file

There are two methods for replacing:

Method A: Overwrite by uploading into the same folder

Navigate to the folder that contains the file (not the file itself, but the folder view).
Example: if replacing work/truck.jpg, open the work folder.
In the top right of the file list, click Add file → Upload files.
Drag-and-drop your replacement image into the upload area, or click choose your files and select it from your computer.
⚠️ Important: Make sure the filename is exactly the same as the one you’re replacing (1.jpg).
If the name matches, GitHub will record this as a replacement (old file removed, new file added in the same commit).

Method B: Delete first, then upload

Open the file you want to replace (e.g., 1.jpg).
In the file preview page, click the trash can icon (Delete this file) in the upper right.
Scroll down and Commit changes to remove it.
Now go back to the folder, click Add file → Upload files, and upload the new version with the same name.

👉 Both methods end up with the same result; Method A is faster.

4. Update .txt file
 the .txt file will need updated to match the photo numbers.
 this way the correct captions go with the correct photos.
 the photo wont be picked up if its not present in the.txt file although a caption is not 100% required as there is a default.
 the format is as follows: 1.jpg|Caption
  
5. Commit your changes

Scroll down to the Commit changes section (it appears below the upload box or after clicking delete).
Fill out the commit message. A good format is:
Replace 1.jpg with updated photo
Select Commit directly to the main branch (since you’re a collaborator, you’re allowed).
If you want to stage changes for review, you can instead select Create a new branch and make a pull request. But for direct replacements, main branch is fine.
Click the Commit changes button.

6. Verify the replacement

Back in the repository, navigate to the file again and click it.
The preview will show the new image.
If it still shows the old one, refresh the page with Ctrl+Shift+R (hard reload) to clear your browser cache.
To double-check, click on the History button (clock icon in the file’s top right). You should see your commit listed as the most recent change.
Example: “Replace 1.jpg with updated photo — committed by [your username]”.

7. Handle caching (important if the file is used on a live site)

GitHub’s raw file URLs (raw.githubusercontent.com/...) and GitHub Pages may cache old versions.
If your live website or embed still shows the old photo:
Append a query string to the image URL (e.g., 1.jpg?v=20250913).
This ensures browsers and CDNs fetch the new file immediately.

✅ Quick Checklist

Sign in and open the repo.

Go to the folder containing the image.

Add file → Upload files → upload new image with the same filename.

Write a clear commit message and commit directly to main.

Verify by viewing the image and checking commit history.

Clear cache or rename file if the old version is still showing.
