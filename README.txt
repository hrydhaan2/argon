BIRTHDAY WEBSITE — SETUP

1. Open index.html in a browser.

2. Put the following files in the assets folder:

   bouquet.jpg
       Main background photograph:
       bouquet of red roses wrapped in parchment.

   envelope.png
       Parchment envelope with a red wax seal.
       This is the clickable envelope on the first page.

   digicam.png
       Digital camera image/icon used as the Memories button.

   gramophone.png
       Gramophone / record image used as the music button.

   memory01.jpg through memory10.jpg
       Your ten memory photographs.

   u-can-count-on-me.mp3
       Your audio file.

3. Login credentials are currently:

       Username: birthday
       Password: 2026

   Change these near the top of the JavaScript section in index.html.

4. Change the birthday letter text directly inside the
   <section id="letterPage"> section.

5. Change "Memory 01", etc. to captions for your photographs.

6. Videos:
   You can replace any memory <img> with:

       <video controls playsinline preload="metadata">
           <source src="assets/memory07.mp4" type="video/mp4">
       </video>

7. Song lyrics:
   The template does NOT include the full lyrics of
   "Count on Me" because the song lyrics are copyrighted.
   Add lyrics only if you have permission/right to reproduce them.

8. For the most reliable result, run the site through a local
   web server rather than opening the HTML directly with file://.

   For example, with Python installed:

       python -m http.server 8000

   Then visit:

       http://localhost:8000

FLOW

Login
  ↓
Bouquet + envelope
  ↓ click wax-seal envelope
Birthday letter
  ↓
Next page
  ↓
Parchment with two buttons
  ├── Digital camera → Memories → 10 media items → Go to letter
  └── Gramophone → Song + lyrics area → Go to home
