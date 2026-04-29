# Setting up the org-level README

GitHub renders a special file on your **organization homepage** (`https://github.com/TeamZoodpaz`) — but only if it lives at a very specific path inside a repo named `.github`.

## Steps

1. **Create a public repo** in the `TeamZoodpaz` org named exactly `.github`
   (URL ends up as `https://github.com/TeamZoodpaz/.github`)

2. **Add these two files** at this exact path:
   ```
   profile/README.md
   profile/zoodpaz-logomark.png
   ```

3. **Push to `main`** — GitHub automatically picks it up and renders `profile/README.md` on the org's public page.

## Files in this folder

- `profile/README.md` — the org-page content
- `profile/zoodpaz-logomark.png` — referenced by the README via raw.githubusercontent URL

## Notes

- The image URL hardcodes `main` as the branch. If you use a different default branch, update the `<img src>` in `README.md`.
- The badges at the top use [shields.io](https://shields.io). They're plain images — no JS, render everywhere.
- Replace `https://zoodpaz.xyz` placeholders if your final domain differs.
