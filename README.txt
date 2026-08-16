MOVE PILOT MELBOURNE CLEAN V8 — STAFF LOGIN FIX

Critical fix:
- Staff login was crashing during dashboard render because hasStaffAgreement() referenced a non-existent variable named `agreements`.
- The correct loaded agreement array is `acceptances`.
- This caused the staff account to briefly log in and immediately return to the login screen.
- Fixed to use acceptances.
- Keeps V7 Assign Staff, V6 secure offer response, V5 Driver Agreement, and V4 van workflow.

No new SQL required.

After upload, test staff login at:
https://maheshckwg.github.io/move-pilot-melbourne/?v=8
