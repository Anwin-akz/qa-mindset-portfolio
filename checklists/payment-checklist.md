# Payment & Checkout Checklist

## Cart Behavior
- [ ] Correct items and quantities shown
- [ ] Price updates when quantity changes
- [ ] Out-of-stock item added mid-session — handled gracefully
- [ ] Cart persists after browser refresh
- [ ] Cart persists after logout/login

## Coupon / Promo Codes
- [ ] Valid coupon applies correct discount
- [ ] Expired coupon shows clear error
- [ ] Invalid coupon shows clear error
- [ ] Same coupon can't be applied twice
- [ ] Coupon + gift card combination — price never goes negative
- [ ] Coupon removed — original price restored correctly

## Payment Flow
- [ ] Successful payment — confirmation shown + email received
- [ ] Card decline — clear error, no money deducted
- [ ] Network timeout during payment — no duplicate charge
- [ ] Double-clicking Pay button — only one transaction fires
- [ ] Back button after payment initiated — what happens?
- [ ] Payment page auto-refreshed — session handled

## Post Payment
- [ ] Order confirmation page loads
- [ ] Confirmation email received within expected time
- [ ] Order appears in order history
- [ ] Invoice/receipt is accurate

## Edge Cases
- [ ] Price changes between adding to cart and checkout
- [ ] Last item in stock bought by someone else mid-checkout
- [ ] Zero value order (100% coupon) — handled
- [ ] Refund flow — partial and full refund
