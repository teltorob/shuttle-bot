# Shuttle Messenger Bot + Menu Messenger Bot

This is a simple Facebook Messenger bot that I built on a Thursday night in March 2017.

Credit for the code to configure the Bot goes to: https://github.com/hartleybrody/fb-messenger-bot. I also used a blog entry by the same author to help me with the configuration. Kudos to @hartleybrody.

I initially cloned the above repository to get everything up and running, and then amended it to give the desired information.

## How does it work?

~~For the shuttle schedule, it uses `binary search` to decide what is the next biggest integer after the integer representing the current time in the `list` that contains the shuttle timings.~~

~~For the Menu, it uses file handling with a `.csv` file that holds the menu for each week. The menu for each week will have to be updated manually.~~

It uses the time at which the message was _received_ by the system, and not the time at which the message was sent by the user.

**Update:**
The striked-through description above involved parsing Excel files and/or PDFs to get data. This proved to be cumbersome because of the ever-changing format in which the Ashoka University administration sent out the shuttle schedule/mess menu. Hence, I replaced that system with a user interface (UI). This UI could be used by anyone having a password (maybe someone in the Student Government) to update the database that the bot accesses. This UI can be found at: https://sheltered-woodland-59238.herokuapp.com/.

## Commands Allowed

    1. SHUTTLE HELP: Shows the list of commands that you can use for the shuttle service. It includes:
     - SHUTTLE CAMPUS: Shows timings of next 3 shuttles from Campus to Jahangirpuri.
     - SHUTTLE METRO: Shows timings of next 3 shuttles from Jahangirpuri to Ashoka.
    2. MENU BREAKFAST
    3. MENU LUNCH
    4. MENU SNACKS
    5. MENU DINNER

Example screenshot:
![Screenshot of the Messenger bot](static/screenshot.png)

## Recognition

Students loved this bot! There were regular requests for adding more and more features. This bot served the Ashoka community for about 3 years, after which no one volunteered to update data on it. In total, it served more than 800 unique users. It sent and received about 200,000 messages!

It was also recognized by the Office of Student Life (OSL) with the "Creative and Entrepreneurial Initiatives" award in the Annual Merit Awards ceremony in April 2018.
