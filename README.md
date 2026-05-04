# NoNumber Chat - Private Pilot

A private pilot for a phone-number-free group chat tool.

## Current working structure

### Public/member link

https://nonumberchat.github.io/No-number-chat/

This page does not show the admin buttons. It tells people this is a private pilot and asks them to join by QR/invite link.

### Creator Admin link

https://nonumberchat.github.io/No-number-chat/?admin=1

Creator Admin PIN for this pilot:

0000

### Member join links

Creator Admin creates a group and uses the QR button. Members scan the QR code or open the invite link.

They then:

1. Choose a first name or nickname.
2. Agree to the rules.
3. Join the group chat.
4. Chat without sharing phone numbers.

## What is included

- index.html
- manifest.json
- sw.js
- assets/icon-192.png
- assets/icon-512.png
- firestore-rules-private-pilot.txt
- README.md
- QUICK_START.txt

## Important Firebase note

The included Firestore rules are still pilot rules. They are better than the fully open test rules because they require anonymous Firebase sign-in:

allow read, write: if request.auth != null;

Before any public launch, Creator Admin and Group Admin permissions should be properly locked down server-side.

## GitHub upload

Upload all these files to the root of the GitHub repo:

- index.html
- manifest.json
- sw.js
- assets folder
- README.md
- QUICK_START.txt
- firestore-rules-private-pilot.txt

Then commit changes.

## GitHub Pages

Settings → Pages → Deploy from branch → main → /root

## Firebase rules

Open Firebase:

Firestore Database → Rules

Paste the contents of:

firestore-rules-private-pilot.txt

Then Publish.
