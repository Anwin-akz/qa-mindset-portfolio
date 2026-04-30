# Login & Signup Checklist

## Happy Path
- [ ] Valid username + valid password logs in successfully
- [ ] Redirect after login goes to correct page
- [ ] User sees their name/profile after login

## Negative Cases
- [ ] Invalid username shows correct error message
- [ ] Invalid password shows correct error message
- [ ] Empty username field — validation fires
- [ ] Empty password field — validation fires
- [ ] Both fields empty — correct error shown

## Edge Cases
- [ ] Password with special characters (@#$%!) works
- [ ] Username with spaces — handled or rejected clearly
- [ ] Very long username (200+ chars) — no crash
- [ ] SQL injection in username field — no DB error exposed
- [ ] XSS in username field — script not executed

## Security
- [ ] Password is masked by default
- [ ] Show/hide password toggle works
- [ ] Account locks after N failed attempts
- [ ] Locked account shows clear message
- [ ] Session expires after inactivity
- [ ] Logout clears session — back button doesn't return to app
- [ ] Concurrent login from 2 devices — behavior defined

## Forgot Password
- [ ] Valid email receives reset link
- [ ] Invalid email shows appropriate message
- [ ] Reset link expires after defined time
- [ ] Old password doesn't work after reset
- [ ] Reset link can only be used once

## Remember Me
- [ ] Checked — user stays logged in after browser close
- [ ] Unchecked — session ends on browser close

## Mobile Specific
- [ ] Keyboard doesn't hide the login button
- [ ] Auto-fill works correctly
- [ ] Face ID / fingerprint login works (if supported)
