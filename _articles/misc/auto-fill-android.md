---
layout: article
title: Auto-fill Android
categories: [Misc]
featured: false
popular: false
tags: [android, auto fill]
---

## Enable the service
1. Open the bitwarden app
2. Tap **Tools > bitwarden Auto-fill Service**
    - *Status Disabled* will appear
3. Tap **OPEN ACCESSIBILITY SETTINGS**
4. Locate **bitwarden** from the list and enable it

Auto-fill is context-sensitive. This means that the bitwarden auto-fill icon, and notification will only appear when it detects a login form or when the password field is selected. It should be noted that the auto-fill service does not currently work when logging into a website from your mobile web browser.

## Test auto-fill
1. Open an app that has not been signed in to
2. Tap the password box
    - The bitwarden icon will appear in the notification bar
3. Open the notification drawer and tap **bitwarden Auto-fill Service**
    - Your vault will display all matching logins otherwise you may need to manually search for it
4. Tap the appropriate login
    - Your username and password will be auto-filled
