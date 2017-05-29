---
layout: article
title: Can't auto-fill in Firefox Private Browsing
categories: [Known Issues]
featured: false
popular: false
tags: [firefox, extension, private mode, private browsing]
---

## Issue
The bitwarden extension does not load when I open it in Firefox Private Browsing.

## Details
This is a known issue with Firefox.

## Workaround
1. Navigate to the website's login page
2. Right click the page
    - A context menu will appear
3. Select **bitwarden > Auto-fill > The website**
    - If **Vault is locked.** appears, unlock the browser extension from a non-private Firefox window

## References
1. bitwarden discussion - <https://github.com/bitwarden/browser/issues/136>
2. FireFox Bugzilla - <https://bugzilla.mozilla.org/show_bug.cgi?id=1329304>
