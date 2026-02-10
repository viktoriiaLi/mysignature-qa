## Test Case

Verify that mandatory onboarding steps cannot be bypassed when logging in via Google.

### Preconditions
- User is logged out
- Browser cookies cleared or Incognito mode enabled

### Steps
1. Open https://mysignature.io
2. Click **Sign in**
3. Choose **Sign in with Google**
4. Complete Google authentication
5. On onboarding screen, leave **Position** field empty
6. Refresh the page or open the site in a new tab

### Expected Result
- User is redirected back to onboarding
- Mandatory field **Position** is required
- Access to dashboard is blocked

### Actual Result
- User is redirected to dashboard
- Mandatory onboarding step is skipped
