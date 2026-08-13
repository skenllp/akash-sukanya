SUKANYA & AKASH — PARINAYAVASANTHAM
=====================================

RECENT REVISIONS
-------------------
- Removed the top navigation bar and the Gallery section entirely.
- Removed the full-page ivory/gold gradient overlays site-wide (the "too
  much white" wash) — sections now show the background art at full
  richness, with text kept legible via a soft glow (text-shadow) instead
  of a panel wash.
- Removed the "Our Story" section.
- The Haldi/Wedding/Reception clips are stock template videos with their
  own baked-in text (couple initials, a heart icon, and a date/time —
  notably the wrong date, "Saturday, Nov 3", since the templates weren't
  customized). That text is part of the video's pixels, so it can't be
  edited out — instead each clip is zoomed and repositioned via CSS so the
  text-bearing top portion sits outside the visible frame, leaving just
  the clean ambient scene (sunflower field, walking couple, fairy-light
  aisle) on screen.

WHAT'S INSIDE
-------------
index.html                     The website itself (single file, no build step)
assets/images/                 Your 4 supplied backgrounds, bride & groom photos,
                                and auto-generated poster frames for the 3 videos
assets/video/                  Your Haldi, Wedding and Reception videos

HOW TO VIEW IT
---------------
Double-click index.html to open it in any browser. Keep the "assets" folder
next to it — don't separate them.

HOW TO PUT IT ONLINE
----------------------
Upload the whole folder (index.html + assets/) to any static host:
  - Netlify / Vercel: drag-and-drop the folder in their dashboard
  - GitHub Pages: push the folder to a repo and enable Pages
  - Any regular web hosting / cPanel: upload via FTP into public_html

No server, build step or database is needed.

ABOUT THE OPENING SEQUENCE
-----------------------------
The opening now plays your Firefly hand-opening video in full: the site
loads to its first frame (hands pressed together, veil closed) as a static
cover — no loader, no spinner. Tapping "Open Invitation" plays the video
from 0: the hands part the golden veil, light spills through, and the
video's own final frame reveals "A Sacred Beginning — Sukanya & Akash — 05
November 2026, Thursday." The site holds briefly on that frame, then
dissolves into the matching Hero section beneath, so the transition reads
as one continuous reveal rather than a cut.

EDITING TEXT / DETAILS
------------------------
Open index.html in any text editor. All copy — names, dates, venue, family
details — is plain, readable text inside the HTML. Search (Ctrl/Cmd+F) for
words like "Sukanya", "Star Auditorium", or "RSVP" to jump to a section.

WHAT'S STILL A PLACEHOLDER
------------------------------
- Our Story: generic, editable copy (no specific relationship history was
  supplied, per your instructions not to invent it).
- Haldi & Reception date/time: the PDF only gave the wedding day's
  Muhurtham (11:30 AM) and two other times (Reception 10:45 AM / Departure
  8:50 AM) whose exact event they belong to wasn't fully clear from the
  card, so I left them out rather than guess — search "to be announced" in
  index.html to fill them in once confirmed.
- Music: the music-toggle wiring from the reference project was left out
  since no audio track was supplied. If you add one, I can wire the same
  gold circular toggle back in.

RSVP FORM
-----------
The form shows a thank-you message on submit. To collect responses into a
spreadsheet, deploy a Google Apps Script Web App (same approach as the
reference project) and paste its /exec URL into RSVP_SHEET_ENDPOINT near
the bottom of the <script> in index.html.

A NOTE ON PRIVACY
--------------------
I left the family phone numbers off the public site (they were on the
physical card, but the brief didn't ask for them to be shown online) —
happy to add a "Call / WhatsApp" button back in if you'd like guests to be
able to reach the family directly from the site.
