# 두둥실 (Dudungsil)

A Korean survey game: type the answer most people would give, and your krill floats higher on its balloons.

- `index.html`: the whole game (single-player Daily / Classic / Endless, plus multiplayer)
- `config.js`: multiplayer settings (Supabase project URL + public key)
- `vendor/supabase.js`: Supabase browser library v2.118.0 (MIT)
- `fonts/`: Galmuri pixel font by Minseo Lee (SIL Open Font License, see `fonts/LICENSE-Galmuri.md`)

## Multiplayer setup (Supabase, free)

1. Create a project at https://supabase.com.
2. In the project, open **Project Settings → API** (or **Data API**), and copy the **Project URL** and the **anon / publishable** key.
3. Paste them into `config.js`.

Multiplayer only uses Supabase Realtime presence (no database tables). The anon key is meant to be public.

## Hosting on GitHub Pages

Push these files to a public repository, then go to **Settings → Pages**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`. The game appears at `https://<username>.github.io/<repo>/`.

Invite links look like `https://<username>.github.io/<repo>/#r123456`.
