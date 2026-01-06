# 🐞 Login Page Bug Report — Misleading error message

**Bug ID:** BUG-LOGIN-001  
**Severity:** S2 — Minor  
**Priority:** P3  
**Status:** Open  
**Environment:** Safari / macOS Sequoia
**Build:** Public Heroku App (https://the-internet.herokuapp.com/login)

## Description
When logging in with invalid credentials, the message contains the text “Your username is invalid!” even if the password is wrong, which is misleading.

## Steps to Reproduce
1. Navigate to [https://the-internet.herokuapp.com/login](https://the-internet.herokuapp.com/login)  
2. Enter invalid username or password (e.g., "wronguser" / "wrongpass")  
3. Click **Login**  
4. Observe the error message

## Expected Result
It should indicates either the username or the password is wrong

## Actual Result
It implies only the username is wrong

## Impact
- Users may misunderstand that their username is wrong when their password might be the cause

## Suggested Fix
- Change the error message to communicate that either username or password is wrong  
- Add a dismiss button for user control
