VICE CITY HQ — V6.17: PRIVATE CLOUD CONNECTION

Based on the working V6.16 build.

Adds:
- A private cloud sign-in panel using the Supabase project configured by the owner.
- Secure email/password sign-in through Supabase Auth.
- First-login migration of the current phone's HQ app data, cat portraits and five station playlist URLs into public.hq_data.
- Later app saves and station changes are written to the signed-in user's own row, protected by the table's Row Level Security policies.
- Existing localStorage remains the working local copy and is not removed.
- If a cloud row already exists, the user is asked whether to load it or upload the current phone's data; no silent overwrite.

Before installing:
- Keep V6.16 ZIP as a rollback backup.
- The Supabase publishable key is embedded in the frontend by design; it is not a secret. Never put a secret/service-role key in the website.
- The hq_data table must have the RLS policies created in the Supabase SQL Editor.
- Site URL and redirect URL should include https://jakeywesley.github.io/vice-city-hq/

Install:
1. Extract this ZIP.
2. Upload index.html to the root of the GitHub Pages repository, replacing the existing index.html.
3. Commit and wait for Pages to publish.
4. Open the live site and tap HQ CLOUD.
5. Sign in using the Supabase user you created. Keep your password private.
6. On first sign-in, verify the status says the first upload completed.

Important:
- This is an initial sync connection, not a full multi-device conflict-resolution system.
- Sync occurs when the app saves changes and when station links are saved/cleared. Keep the phone's local backup.
- Do not invite Meg until her read-only access and database policies have been separately configured and tested.
