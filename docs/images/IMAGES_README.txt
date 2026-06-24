IMAGES THE SITE EXPECTS
=======================

Included already
----------------
  images/blink-logo.gif            Animated BLiNK lab logo (navbar/home)
  images/rutgers-sas-black.png     Rutgers SAS lockup (navbar, on white)
  images/rutgers-sas-white.png     Rutgers SAS lockup (footer, on dark)
  images/placeholder.svg           Fallback avatar for people without a photo

You add these
-------------
PEOPLE  ->  images/people/   ALL HEADSHOTS ARE NOW INCLUDED:
  nuria.jpeg, kaylee.jpg, eva.jpg, hector.jpg, krupa.jpg, anushka.jpg,
  anthony.JPG, adarsh.png, ibrahim.jpeg, ezequiel.png, cristina.jpeg, daniel.JPG
  (Replace any of these files in-place if you want a different photo; keep the
   same filename, or update the <img src> in people.Rmd.)

HOME HERO TILES  ->  images/lab/   (landscape)
  hero1.jpg  hero2.jpg  hero3.jpg  hero4.jpg

GALLERY  ->  images/lab/   (landscape; see gallery.Rmd for the exact list)
  eeg1.jpeg ... eeg7.jpeg, eeg8.jpg ... eeg16.jpg,
  eyetracking.png, hls2023.jpg

Notes
-----
- Filenames are case-sensitive on most web servers. Match them exactly,
  or edit the <img src="..."> path in the matching .Rmd file.
- If a referenced image is missing, the browser shows a broken-image icon
  (people fall back to placeholder.svg).
