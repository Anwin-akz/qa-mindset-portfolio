# Mobile Testing Checklist

## Devices & OS
- [ ] Tested on Android (latest and one version below)
- [ ] Tested on iOS (latest and one version below)
- [ ] Tested on small screen (5 inch) and large screen (6.5 inch)

## UI & Layout
- [ ] No content cut off in portrait mode
- [ ] No content cut off in landscape mode
- [ ] Buttons and tap targets are minimum 44x44px
- [ ] Text is readable without zooming
- [ ] Images are not pixelated on Retina screens

## Keyboard & Input
- [ ] Keyboard does not hide active input field
- [ ] Keyboard dismiss works correctly
- [ ] Correct keyboard type shown (numeric for phone, email for email)
- [ ] Auto-correct doesn't corrupt form inputs

## Network Conditions
- [ ] App works on 4G
- [ ] App degrades gracefully on slow 3G
- [ ] Airplane mode mid-action — handled without crash
- [ ] Network loss during payment — no duplicate transaction

## App Lifecycle
- [ ] App backgrounded mid-flow — resumes correctly
- [ ] Incoming call during checkout — session preserved
- [ ] App killed and relaunched — state handled
- [ ] Phone rotated mid-form — data not lost
