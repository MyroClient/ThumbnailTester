YT Thumbnail Tester (Dark Mode)
================================

Open index.html in any browser — no server or build step needed.

REPLACING THE PLACEHOLDER THUMBNAILS
-------------------------------------
Each competitor card loads its image from a numbered file in /assets:

  assets/thumbnail1.jpg
  assets/thumbnail2.jpg
  assets/thumbnail3.jpg
  ...through...
  assets/thumbnail8.jpg

To swap in real thumbnails, just overwrite these files with your own
images using the SAME filenames (keep the .jpg extension, or update the
"assetPath" value for that card in the <script> block near the top of
index.html if you want to use .png/.webp instead).

If a file is ever missing or fails to load, the card automatically falls
back to a styled gradient placeholder — so the page never breaks.

YOUR OWN VIDEO CARD
--------------------
Your own thumbnail slot is handled separately: click the hamburger menu
(or the ✎ icon on your card) to upload an image directly in the browser.
That image is stored in your browser's localStorage as a data URL, so it
never touches the assets/ folder and stays local to your machine.

FILES
-----
index.html      - the full app (structure, styles, and logic)
assets/         - placeholder thumbnail1.jpg ... thumbnail8.jpg
README.txt      - this file
