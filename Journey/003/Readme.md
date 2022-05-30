

# Day 3 - Exchange Online Configuration 

## Introduction

I'm doing this one today because email is very useful and a key component to Microsoft 365 infrastructure. Also, I'm pretty sure that most things going forward will need some kind of email verification or email connector, so yea, having a functioning mail system is necessary. 

## Prerequisite

A firm grasp on how mail flow and MS Exchange in general works, 365 Admin Roles, and Outlook endpoint connector configuration.  



## Cloud Research

- My first research was on how to configure MX records when there aren't any already setup in your Domain Registrar.  I thought it was something that would be added when you connect your domain to 365 automatically, which ironically, I was right.  I just wasn't patient enough to figure that out.  So my research was to discover that I needed to be patient. 


### Step 1 — Configuring DNS Records in Domain Registrar

After you've setup your users in Azure AD or MS 365 Admin Portal and assigned them a license that includes Exchange/Mail, after Microsoft processes the request, they will have an Exchange Mailbox automatically created for them.  So that part is fairly automated.  

- However, it does appear that even though I connected the domain to 365 as a custom domain on Day One, the Mail Exchanger (MX) records were not created.  So that is what I need to do first.  

- (Correction) I only partially connected the domain to 365, although not sure why.  It didn't add all of the DNS records it was supposed to.  Perhaps there is a delay in the registration or setup and now that it's uploaded into 365, I am able to add in the DNS records properly.  Either way, I've got the records entered.  And not just MX and SPF, but the Skype/Lync connectivity and even the Intune Mobile Device Enrollment DNS records as well! So those will come in handy in a few weeks when I start on the Intune MDM topics. 

### Step 2 - Testing the Email in Outlook

Fairly straight forward:  Send myself an email from another account and see what happens.  

Spoiler Alert!

I received the email after getting the DNS records sorted out.  Woohoo! 

<p align="left">
  <img src="Templates/homer-woohoo.jpg">
</p>

### Step 3 — Summary of Step

![Screenshot](https://via.placeholder.com/500x300)

## ☁️ Cloud Outcome

✍️ (Result) Describe your personal outcome, and lessons learned.

## Next Steps

✍️ Describe what you think you think you want to do next.

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](link)
