MOVE PILOT MELBOURNE - CLEAN V3

Critical fix:
- Fixed the broken JavaScript template string in the mobile job-card renderer.
- The complete inline JavaScript was checked with Node's syntax checker before packaging.
- This fixes the symptom where the dashboard displayed but every button was dead.
- Includes the correct Move Pilot Melbourne logo artwork.

No new Supabase SQL is required.

Upload ALL files to the existing GitHub repository:
move-pilot-melbourne

Replace the current files, then open:
https://maheshckwg.github.io/move-pilot-melbourne/?v=3

First tests:
1. Tap Sign out — it should show Login.
2. Sign back in.
3. Tap + New Inquiry — the inquiry form should open.
4. Tap the status filters — they should respond.
