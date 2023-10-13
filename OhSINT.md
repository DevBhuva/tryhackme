# OhSINT

This is the walkthrough for the [OhSINT room](https://tryhackme.com/room/ohsint) on TryHackMe.

### Task 1: OhSINT

All I have is a photo. I used exiftool to see what starting information I could get of the photo. (`exiftool WindowsXP.jpg`).
![exiftool](https://github.com/DevBhuva/tryhackme/assets/145397562/d60fdcc8-6cda-43db-980c-b812f6be678a)


Notice that the Copyright value is OWoodflint. Next, I searched good ol' google to see what I could find on OWoodflint.

I found their twitter page (answering question 1),
![twitter](https://github.com/DevBhuva/tryhackme/assets/145397562/ff85c32d-7a72-47d8-9499-9814ac2acad0)

their blog (answering questions 6 & 7, if you inspect the blog's HTML),

![blog](https://github.com/DevBhuva/tryhackme/assets/145397562/615b0e8d-6dac-47d7-95a9-72fdd2af56e8)

and their github (answering questions 2, 4 & 5).

![github](https://github.com/DevBhuva/tryhackme/assets/145397562/f8b0535d-dedb-4147-9bf6-ca2437b0b574)


1. What is this user's avatar of?

   > cat

2. What city is this person in?

   > London

3. What's the SSID of the WAP he connected to?

   The hint for question 2 mentions *BSSID + Wigle.net*. So, I accessed [Wigle.net](https://wigle.net/) and, plugging in the BSSID found OWoodflint's twitter page, I found the exact location of the WAP and its SSID. Yikes!

   ![screenshot_wigle](/room_ohsint/screenshots/wigle.png?raw=true)

   *Notice the purple circle on the map and zoom in really really close on it.*

   > UnileverWiFi

4. What is his personal email address?

   > OWoodflint@gmail.com

5. What site did you find his email address on?

   > github

6. Where has he gone on holiday?

   > New York

7. What is this persons password?

   > pennYDr0pper.!
