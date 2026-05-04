# NoNumber Chat - v9 Group Home Screen Fix

This version fixes the phone home-screen issue more reliably.

## What changed

The app no longer wipes the group invite URL after someone joins.

That means if a member opens a group invite link like:

https://nonumberchat.github.io/No-number-chat/?join=GROUP_ID&code=GROUP_CODE

then joins and adds that page to their phone home screen, the shortcut opens the same group again.

## Important for testing

Delete the old home-screen icon first.

Then:

1. Open the group/member invite link or scan the QR.
2. Enter nickname and join.
3. While still in that group/chat, add it to the phone home screen.
4. Close it.
5. Open the new home-screen icon.

It should reopen that group instead of the public page.

## Links

Public:
https://nonumberchat.github.io/No-number-chat/

Admin:
https://nonumberchat.github.io/No-number-chat/?admin=1

PIN:
0000

Group application:
https://nonumberchat.github.io/No-number-chat/?apply=1

## Upload

Upload all files to GitHub repo root and commit changes.
