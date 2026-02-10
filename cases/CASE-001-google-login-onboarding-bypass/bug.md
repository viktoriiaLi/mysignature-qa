## Bug Report

### Title
User can bypass mandatory onboarding when logging in via Google

### Environment
- OS: macOS
- Browser: Chrome
- Auth method: Google OAuth
- User state: New user

### Preconditions
- User is logged out
- Browser cookies cleared or Incognito mode enabled

### Steps to Reproduce
1. Open https://mysignature.io
2. Click **Sign in**
3. Choose **Sign in with Google**
4. Complete Google authentication
5. On onboarding screen, leave **Position** field empty
6. Refresh the page or open the site in a new tab

### Expected Result
User is redirected back to onboarding and cannot access dashboard until mandatory fields are completed.

### Actual Result
User is redirected to dashboard without completing mandatory onboarding step.

### Severity
High

### Priority
High

### Notes
This issue allows bypassing required onboarding logic and may lead to incomplete user profiles and inconsistent system state.
Issue also reproduces after logout and re-login via Google with partial onboarding data persisted.
