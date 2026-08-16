MOVE PILOT MELBOURNE CLEAN V9 — SIGNATURE FIX

Critical fix:
- Staff Driver & Van Responsibility Agreement used the wrong JavaScript helper name.
- It called signatureData(...), but the app defines getSignatureData(...).
- This caused Sign & Accept Agreement to fail even when the staff member drew a signature.
- Fixed all signature call sites to use getSignatureData(...).

No new SQL required.

Test:
1. Staff logs in.
2. Open Driver Agreement.
3. Enter licence details.
4. Draw signature.
5. Tick agreement checkbox.
6. Tap Sign & Accept Agreement.
7. Agreement should save and the staff member can continue to the job offer / van workflow.
