# IWAS Public Showcase Deployment

## Files
- `index.html`
- `styles.css`

## Recommended structure
Use your main public domain for the showcase:
- `iwas.is` = public showcase
- `lab.iwas.is` or `prototype.iwas.is` = private prototype/lab

## Deploy public showcase on Vercel
1. Create a new GitHub repository, for example `iwas-showcase`.
2. Upload `index.html` and `styles.css` to the repository root.
3. Go to Vercel → Add New Project → Import the repository.
4. Framework preset: Other / Static.
5. Build command: leave empty.
6. Output directory: leave empty or use `.`.
7. Deploy.
8. In Vercel → Project → Settings → Domains, attach `iwas.is`.

## Lock the current prototype/lab
Best simple option on Vercel:
1. Move the current prototype into its own Vercel project, for example `iwas-lab`.
2. Put it on `lab.iwas.is` or `prototype.iwas.is`.
3. In Vercel, enable password protection / deployment protection if available on your plan.

## Alternative simple lock inside the page
A JavaScript PIN gate can hide content from casual visitors, but it is not secure because the code is still visible in the browser. Use only for light privacy, not real protection.

## Stronger lock
Use Vercel Deployment Protection, Vercel Authentication, Cloudflare Access, or a proper login system with Supabase Auth.
