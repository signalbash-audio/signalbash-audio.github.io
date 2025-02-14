---
title: Website Help
layout: home
nav_order: 1
---

# The Signalbash Website

The Signalbash Website ([signalbash.com](https://signalbash.com)) is where you
can create an account, review your activity, view the leaderboard, manage your 
signalbash profile, and download the signalbash plugin.


## Features

### Leaderboard

The Signalbash leaderboard is a ranked list of everyone who has used Signalbash
to track their activity in the past 24 hours. It will show how long each artist
has been working, as reported by the Signalbash Plugin, along with the DAW(s) or software they used. It will also show personalizable information about each artist, including a profile image, a display or user name, and country.

### Plugin Download

For more information about how to Install & Use the Signalbash plugin,
see its dedicated manual here: [Signalbash Plugin](/plugin/signalbash-plugin-manual)

### Profile Features

Your signalbash profile features stats related to your activity, as well as
standard profile information fields which you can customize.

#### Activity Stats

- Activity Chart (All Time)
    - This chart is private and viewable only by you. It contains a chart
      of your active DAW usage over the past 24 hours.
- Activity Summary (All Time)
    - This is a daily heatmap of all your DAW activity since you've had
      a Signalbash account.
- Streaks (Current & All Time)
    - Streaks show how many days in a row you've actively been working in 
      your DAW with the Signalbash plugin.
      - The *Current* Streak is the length in days of your most recent streak
      - The *All-Time* Stream is the length in days of your longest streak
        since you've been using the Signalbash plugin
- DAW Activity Stats
    
    These stats give at-a-glance stats for the following time spans:

    - Time Today: How long you've been working since 12AM in your local time
    - Last 24 Hours: How long you've been working in the last 24 hours
    - Last 30 Days: How long you've been working in the last 30 days
    - This Year: How long you've spent working since Midnight on January 1st
        of the current year (in your local time)
    - All Time: All your activity combined


## How to Create An Account

Signalbash accounts are free to make and do not require an email address.
In fact, Signalbash doesn't ask you for an email address at
any point.

To create an account, visit the [create account](https://signalbash.com/create-account) page on signalbash.com.

You will have to create a user name and enter a password.

## Verifying Your Account

In order to verify your account to start tracking activity, you must
first verify the session key assigned to you after you create your account.

To do this:

- Download & Install the Signalbash Plugin
- Open the Plugin in your DAW
- Copy the Session Key from your Signalbash Account
- Paste the Session Key into the plugin and hit submit.

Once you do this, the Plugin will verify the key, and you'll be able to
start tracking your activity. 

Learn More: [Signalbash Session Key](/website/session-key)

After creating an account, you will have 24 hours to verify your session
key. Once verified, your account will exist as long as you'd like. However,
if you don't verify your session key within the 24 window, that account
will be automatically deleted, and the associated username will become available
for others to use.


### Signalbash User Names

Signalbash user names must be unique. The account creation page will inform
you if the name you want to use is already taken.

Additionally, there is a limited character set that you can use to create
accounts.

The username is what you use to log in in the future, and will be present
in your Signalbash profile URL. Your Username cannot be changed.

If you want to customize how you appear in your profile and on the leaderboard,
you can edit your display name. You can change this as often as you'd like.

#### TIP
It is highly recommend to use a password manager to save your username & password when creating an account.


## Resetting Your Password

You can reset your password in two ways.

1. While logged in:
    - Click Your Profile Icon in the top right corner of the website
    - Click "Manage Account"
    - Navigate to "Reset Password" and fill in the form

2. While logged out:

    If you can't remember your password, you can use your session key to
    log you back in.

    - Go to the login page on signalbash.com
    - Click Forgot Password
    - Enter Your Session Key & The New Password
    - After you click submit, log back into your account with the new password.

    It's very important you keep your session key safe & private because it can
    be used to login.


## Customizing Your Profile

You can customize your profile on Signalbash like any other website. Editing
several of your profile attributes require that you have verified your session
key, so be sure to do that before proceeding.

### Set Profile Image

To set your profile image:
- Go to your Profile Page
- Under the circular image, click "Edit Profile Image"
- On the next page, drag or select an image, and click "use selected image"

For best results, use a high quality square image. Images that aren't
square will be cropped to square from the center.

Transparency/alpha channels are supported.

### Update Profile Attributes

Your Profile Attributes include:

- Your Display Name
- Currently Working On
- Your Country
- Bio

These are all optional fields, which can be used to populate more information
about you. Several have character limits which appear in the input text boxes.

Currently, only the Display Name & Country fields will display on the
signalbash leaderboard.

### Add Your Links

You can add links which will appear on your profile. To do so, click
"Add Link". Add the URL, and the optional "link title" field.


## Deleting Your Signalbash Account

You can easily delete your account at any time. When deleting your account,
all your activity and associated account data will be permanently deleted. 

To delete your account:
- Click Your Profile Icon in the top right corner of the website
- Click "Manage Account"
- Scroll to "Delete Account"
- Follow the instructions to confirm

Once deleted, your account can't be recovered.


## Activity Stats

### Streaks

Streaks denote how many consecutive days you've been working in your DAW.
Signalbash reports both your Current Streak, and your All Time Streak.

Activity is grouped by days based on your current timezone, which is handled
automatically by your browser.

Your Current Streak will display your most recent activity streak. If
you haven't been active on the current date, but have activity on the previous
date, the streak will still show the most recent streak count. Once two
consecutive days without activity have been detected (today & yesterday), the
current streak will reset to 0.


## Images

Signalbash.com use the modern webp codec to display and encode images in order to
feature high quality
images with smaller file sizes, and also support alpha channels/transparency.

However, legacy browsers on older machines and phones may not be able to
display or use these formats.

At the moment, we do not have any fallback support for legacy browsers.

If you are having issues seeing images appear on the leaderboard or your
profile, you may be on an outdated browser. For example, this is likely to
happen if you're
using the Safari browser on a computer or iphone with an old operating system 
version.

To fix the issue, visit the site on a more modern browser. Chromium based
browsers such as Edge or Chrome should work well, even on older operating
systems.

This may be a requirement to upload profile images in some cases, as images
are resized by your browser before being stored in your account.

When changing your profile image, if you already had a previous
profile image set, the old profile image will be permanently deleted once
the new profile image is finalized and uploaded.

The source image file used to create your profile image will
not be stored. Only the derived, resized variants are stored.
To ensure the highest quality across the site, we suggest using a lossless
image format such as PNG, with dimensions of at least 1000x1000.

You must have the necessary permissions to upload images to your account, and
its contents must abide by the Signalbash Terms of Service.
If you upload images with content that violates the terms of service or
that you do not have permission to use, they may be removed. Repeat or egregious
violations may result in bans.
If someone is using an image which you hold the
copyright for, visit the Copyright Page, accessible from the signalbash.com site
footer, for instructions to issue a takedown request.

