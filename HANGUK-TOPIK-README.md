# HANGUK TOPIK

The application source is in `../app`.

## Run

1. Install Node.js 20 or newer.
2. Open a terminal in the `app` folder.
3. Run `npm start`.
4. Open `http://127.0.0.1:4173`.

No package installation or cloud credentials are required for this local build.

Initial administrator credentials:

- Access code: `herculesAI`
- Password: `hercules@2026`

Change both immediately in **Admin Security Settings**.

## Included

- Responsive black-and-gold PWA shell
- Four-language onboarding and persisted language preference
- Server-side registration, login, logout, profile, and password hashing
- HTTP-only user and admin sessions
- Admin login throttling and temporary lockout
- Published TOPIK I and TOPIK II demo tests
- Listening, reading, writing, answer autosave, resume, submission, scoring, review, and result history
- Admin statistics, test publishing/deletion, user results, writing review, and credential changes
- Local persistent data in `app/data/db.json` (created on first start)

## Deployment note

The zero-configuration build uses a server-owned JSON data store so it works immediately. For public multi-server deployment, migrate the same API models to PostgreSQL/Supabase and object storage, put the service behind HTTPS, and configure backups. Never commit hosted service-role keys to browser code.
