# My 2017 PHCorner Guide: SIM Unlock Huawei E5573Cs‑933 Globe Pocket WiFi (Still Relevant in 2025)
## Links

Note: PHCorner may display some aggressive ads — feel free to use an ad blocker when visiting the site or skip directly to the How-to section.

Original forum post on PHCorner: 

[Tutorial - How to openline (unlock) and debrand huawei e5573cs-933 (globe) | Pinoy Internet and Technology Forums](https://phcorner.org/threads/how-to-openline-unlock-and-debrand-huawei-e5573cs-933-globe.450070/)

Archive copy of the forum post on Archive.org (just in case it goes down):

[Tutorial - How to openline (unlock) and debrand huawei e5573cs-933 (globe) | Pinoy Internet and Technology Forums](https://web.archive.org/web/20250703063157/https://phcorner.org/threads/how-to-openline-unlock-and-debrand-huawei-e5573cs-933-globe.450070/)

Archive containing the tutorial (in PDF), and the files used in the tutorial:

[Huawei E5573CS-933 Openline And Debrand : Manley Evangelista : Free Download, Borrow, and Streaming : Internet Archive](https://archive.org/details/huawei-e-5573-cs-933-openline-and-debrand)

And of course, it's also under "Releases"

#Is it really you, yelnam2manley?

Yes, it’s really me! I’m not an imposter — I’m the same person who originally wrote and posted the tutorial. This website is mine, and I even have a screenshot as proof.

[About Page](https://phcorner.org/members/yelnam2manley.581821/#about) of my profile at PHCorner

<p align="left">
  <img src="https://github.com/manleyevangelista/HuaweiE5573CS-933_SIMUnlock_2017PHCornerGuide/blob/main/images/PHCornerLoggedIn_yelnam2manley.png" width="1000">
</p>

## Why is this still relevant in 2025?

4G (LTE) networks are still up and running in the Philippines, even though it's nowhere as quick as 4G+ (LTE-A; basically, 4G with carrier aggregation) or 5G, it should be still fast enough for many users.

## Context

In 2016, I moved back to the Philippines from California. I went from having a 90/30 Mbps cable internet connection to relying on 3G/4G (that reaches 5Mbps on a good day), as at the time, we didn’t have any option for a fiber connection. I also found myself spending more time outside the house, so I needed something portable anyway.

At the time, Globe had the strongest reception in our house, but I sometimes found myself in places where their signal was weak — or their tower was simply congested. It would’ve been nice to switch to another provider without needing to buy another pocket WiFi from Smart. So, my first step was to go online and see if there was a tutorial for unlocking the particular modem I had: a Huawei E5573CS-933.

I was able to find a tutorial for the Indian/African (E5573S-609) variant and another for the Smart one (E5573S-320). I tried following those with my Globe variant — unfortunately, they didn’t work.

My next step was to find the generic E5573CS-933 firmware online. I couldn’t find it anywhere — except on one site, and it was behind a paywall. I obliged and paid the $15 (which gave me access for three months). I downloaded the firmware and then tried adapting the tutorials from the other variants to this Globe model. The steps were mostly identical, except for the location of the pins that needed to be shorted to boot the modem into firmware-flashing mode.

After trial and error (and one scare because I shorted the wrong pins at first, saw it sparked, and thought I’d fried the pocket WiFi), I was finally able to get the generic firmware flashed successfully. Then I tried flashing it back to Globe’s firmware to reproduce the steps and verify the unlock process. Once I confirmed it worked, I proceeded to write the tutorial and posted it on PHCorner. I also gathered all the files used for the tutorial and compiled them into one archive (RAR) file.

To my surprise, the tutorial blew up — thousands of views, tons of replies, and even a job offer from someone who found it on the forum.

## How-to

I’ve copy-pasted the original guide here as is, for convenience. It was written casually back then, so please excuse any typos, grammar or punctuation issues.

>I finally unlocked my Huawei E5773CS-933 modem from Globe.
>
>I've been trying to unlock it by following a guide for the E5573-609 and E5573-322. However, those did not help as the boot pin is located differently for this variant. Once I located the boot pin (by shorting out every single pin in the board, one at a time), I tried loading the generic E5573CS firmware (after running Balong USB Downloader) and would refuse to install (I get error 12). Given those obstacles, I gave up and hunted for the Globe's 933 firmware. The 933 firmware that I downloaded turned out to be an unbranded/generic, SIM unlocked firmware. From there I faced some more obstacles, mainly the WebUI and dashboard files are nowhere to be found, except on one website where you need to pay at least $15 for a ρáíd account, to get access to the files. After pulling the trigger, I was able to unlock the device as well as remove Globe's branding in the process.
>
>I decided to put all of the files you need in a one ZIP archive. So you won't have to spend hours searching for the files. I know you got better things to do.
>
>Downloads: Links are already on top of this post.
>
>Also, I'm not respponsible if you screw/hard brick your modem. I've done this twice already (to unlock my modem (and then to replicate these step)
>
>1. Install the both the FcSerialDrv and Mobile Partner drivers on "Drivers" directory.
>
>2. Disassemble your modem using T5 torx screwdriver.
NOTE: This is the part where you'll have to break the seal and void your warranty. Sorry, there's no way to unlock without doing this. So either keep your warranty or unlock your modem.
>
>3. Take out the board and flip it over.
>
>4. Connect the board to the computer, and open Device Manager
>
>5. Grab tweezers or similar device that's conductive. Then short out one of the pin/metal part (shown in the pic) near the SIM card slot.
><p align="left">
>  <img src="https://github.com/manleyevangelista/HuaweiE5573CS-933_SIMUnlock_2017PHCornerGuide/blob/main/images/Step5.jpg"width="300">
></p>
>6. While keeping the pin/metal part shorted out. Go ahead and put the battery approximately 45-degree angle while keeping it in contacct witn the gold terminals. As shown in the pic.
><p align="left">
>  <img src="https://github.com/manleyevangelista/HuaweiE5573CS-933_SIMUnlock_2017PHCornerGuide/blob/main/images/Step6.jpg"width="500">
></p>
>7. If you did it right. You should see "HUAWEI Mobile Connect - 3G PC UI Interface", "FC - PC UI Interface" or something similar under Ports (COM & LPT) on Device Manager. You don't need the tweezers anymore but leave the battery alone.
><p align="left">
>  <img src="https://github.com/manleyevangelista/HuaweiE5573CS-933_SIMUnlock_2017PHCornerGuide/blob/main/images/Step7.jpg"width="500">
></p>
>8. Launch Balong USB Loader at "Balong USB Downloader" directory.
>
>9. Click "Detect". Then Press the three dots. Then "Load"
>
>10. It should take about 5-20 seconds for USB Downloader to do its thing. It's normal for the program to freeze, however, when its done. It should return with a full progress bar.
><p align="left">
>  <img src="https://github.com/manleyevangelista/HuaweiE5573CS-933_SIMUnlock_2017PHCornerGuide/blob/main/images/Step10.jpg"width="500">
></p>
>11. Check Device Manager and if you see both "FC - Application Interface" and "FC - PC UI Interface" or something similar, proceed to the next step.
><p align="left">
>  <img src="https://github.com/manleyevangelista/HuaweiE5573CS-933_SIMUnlock_2017PHCornerGuide/blob/main/images/Step11.jpg"width="500">
></p>
>12. Go to "Firmware (21.320.99.05.00)" directory and run "E5573Cs-933_Update_21.320.99.05.00.exe" The go through the wizard.
>
>13. Go to "WebUI (WEBUI_21.100.32.00.03_NE5)" and run "Update_WEBUI_21.100.32.00.03_NE5.exe". Same thing as last step. Go through the wizard.
>
>14. Let go of the battery, disconnect the board, and assemble the modem.
>
>15. Insert a SIM card. (I used a Globe SIM, but any SIM could work.) DON'T SKIP THIS. Doing so will give you an error on DC Unlocker when trying to repair the serial number and IMEI of your modem.
>
>16. Connect the modem to the computer. Then run "dc-unlocker2client_1277.exe" at the "DC Unlocker" directory.
>
>17. Click on the magnifying glass/search.
>
>18. When the modem is found, you'll see that it's already unlocked but we can't use it yet due to not having the correct serial and IMEI.
><p align="left">
>  <img src="https://github.com/manleyevangelista/HuaweiE5573CS-933_SIMUnlock_2017PHCornerGuide/blob/main/images/Step18.jpg"width="500">
></p>
>19. Run HxD and type out the serial number on the right side.
>
>20. Now type in this command: AT^NVWR=6,16,** ** ** ** ** ** ** ** ** ** ** ** ** ** ** **
Replace ** with the hex code you got from HxD (copy paste the values in the middle (between the zeros and the serial number you just typed. Press enter. It should say OK.
>
>21. Now type in this command: AT^CIMEI="*****". For example if your imei is 1234567890123456, then you would type: AT^CIMEI="123456789123456"
Replace * with your IMEI. Press enter. It should say OK.
><p align="left">
>  <img src="https://github.com/manleyevangelista/HuaweiE5573CS-933_SIMUnlock_2017PHCornerGuide/blob/main/images/Step21.jpg"width="700">
></p>
>22. Click on the magnifying glass (again) and see if the correct serial number and IMEI shows up. Once done, close out of DC Unlocker.
>
>23. Finally, go to "Firmware (21.326.13.00.00)" directory and run "E5573Cs-933_Update_21.326.13.00.00.exe"
>
>One done. The modem should reboot and should automatically open a web browser, which goes to the Huawei page. If not, open your web browser and go to 192.168.8.1. If it asks you for a username and password. It's "admin" for both. From here, you'll need to setup the network name, password, etc. Just like you would when you first bought the modem.
><p align="left">
>  <img src="https://github.com/manleyevangelista/HuaweiE5573CS-933_SIMUnlock_2017PHCornerGuide/blob/main/images/LastPic.jpg"width="500">
></p>
