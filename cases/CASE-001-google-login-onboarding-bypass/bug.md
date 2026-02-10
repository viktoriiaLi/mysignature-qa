# Bug Report — CASE-001  
**Google Login → Onboarding Bypass**

---

## Summary
User can bypass mandatory onboarding step (**Position**)  
when logging in via Google and gain access to dashboard.

---

## Environment
- App: MySignature.io (web)
- Auth method: Google Login
- Browser: Chrome / Safari
- Account state: New user

---

## Preconditions
- User is logged out
- Browser cookies cleared or Incognito mode enabled

---

## Steps to Reproduce
1. Open https://mysignature.io  
2. Click **Sign in**
3. Choose **Sign in with Google**
4. Complete Google authentication
5. On onboarding screen, leave **Position** field empty
6. Refresh the page **or**
7. Log out and log in again via Google

---

## Expected Result
- User cannot access dashboard
- Mandatory onboarding fields are enforced
- User remains on onboarding screen

---

## Actual Result
- User is redirected to dashboard
- Mandatory onboarding step is skipped
- Previously entered data may be auto-applied

---

## Severity
**High**

---

## Impact
- Incomplete user profiles
- Broken onboarding flow
- Invalid user data in system
- Potential analytics and billing issues

---

## Evidence
See `/evidence/video.md`
