# API Testing Checklist

## Request Validation
- [ ] Happy path — correct request returns expected response
- [ ] Missing required field — 400 returned with clear message
- [ ] Wrong data type (string where int expected) — handled
- [ ] Extra unexpected fields in request — ignored or rejected
- [ ] Empty string vs null — both handled correctly

## Authentication
- [ ] Valid token — request succeeds
- [ ] Expired token — 401 returned
- [ ] Invalid/tampered token — 401 returned
- [ ] No token sent — 401 returned
- [ ] Unauthorized role accessing restricted endpoint — 403

## Response Validation
- [ ] Correct HTTP status code returned
- [ ] Response schema matches documentation
- [ ] No sensitive data exposed (passwords, internal IDs)
- [ ] Consistent date/time format
- [ ] Pagination works correctly (page size, total count)

## Edge Cases
- [ ] Very large payload — handled or rejected clearly
- [ ] Special characters in string fields
- [ ] SQL injection in query params — no DB error exposed
- [ ] Rate limiting — 429 returned when exceeded
- [ ] Response time within acceptable threshold
