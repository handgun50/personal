---
layout: page
title: BCA Transaction Notifier
---

This idea behind this project is because I have an account with 2 owners. When there is a transaction in or out, everyone should know to avoid abusement. I use python to solve this case. I got the main code from GitHub so I didn't need to write the code from scratch. After learn the code, then I modify the code to have an ability for continuous checking and notify when there is an incoming or outgoing transaction. The code is deployed to my private VPS because I need to save the ID and password for login. The code itself is quite ugly because the main code from GitHub is using class statements and I haven't learn many about using class. At least, it works :)

The core of the code is the script will check if there is new transaction every 4 minutes from 08:00 until 20:00. 4 minutes is selected because there is a rate-limit from the bank side so I can't check like every 5 seconds. And the delay also shouldn't more than 4 minutes to avoid session getting timed out from the bank side.

I have run the script for months and so far I have fixed all important bugs. At the moment, I didn't have plan to improve the script beacause it already covers all my needs.

Below is screenshot when there is new transaction, the script will send notification to my discord
![bca-discord](https://res.cloudinary.com/handgun50/image/upload/q_auto:eco/v1676733948/personal/Screenshot_2023-02-18-22-24-28-283_com.discord_gwvrmb.jpg)

**Update 1 :**

After some months, the code breaks because the bank side has implement things to prevent bot getting the bank data. After thinking and getting ideas from Internet, so I build a new code. 

The code will simulate user input. Because of this, the VPS is fully used for simulating the browser. At the moment, the check occurs every ~30 minutes because if too fast, the bank side will mark it as a bot so I couldn't get the bank data.. The code itself still has some bugs because sometimes the missclick happens. But thankfully it didn't create a big mess so I can live with the bugs. 

