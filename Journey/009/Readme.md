

# Day 9 - My First (moderately) Advanced Power Automate Flow

## Introduction

So I've been working with a friend to help automate several business processes for them and I figured it was high time I step into Power Automate and kick the tires on this bad boy to see what all the fuss was about.  Boy was I thrilled when I got something working and it was actually useful!!

It's not like I invented the next AI Jarvis or anything, it's just a simple daily email to everyone in my team to update them on the status of a project I'm working on but it's still pretty cool.  I added in a few extra flairs to see if I could stretch it as well.

## Use Case

When you are tracking a project in Excel and want to show your team or stake holders, or just want to send a regular email, you can use this flow concept to generate a link from OneDrive, customize the properties of the link, add it to an email message, and send it on a regular interval.

Like I said, it's not super flashy or amazing. And it certainly won't cure cancer or get us back to the Moon, but it was definitely a win for me because it was the first solo Automate Flow I've built. 

## Explanation

1) The first part is to create a time based trigger that will kick off the flow.  For me, I wanted it to happen every week day.  At first, I thought it couldn't happen but again, it's Microsoft and that's not likely.  A tiny bit of research and found out that the Weekly trigger will allow you to select the individual days of the week in which you want it to run. After the days, you will have to configure the time along with the first day you want it to begin in a unique format:  `2022-01-01T15:00:00Z`  The date is obvious, but the time is in 24hour standard time defaulted to UTC but you can select your local timezone in the advanced settings of the trigger box.
2) Then, after you've set the date and time, the next step is to configure the link from OneDrive/SharePoint.  This one is pretty straight forward.  Select the task to create link from file and it will give you options to select whether users who have the link can edit or view only and whether they can be 'anonymous' users or if they must be Organization Users only. (add info about 
3) Finally, this is where you create the email and add the link generated from OneDrive.  Search for Outlook email and add

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](link)
