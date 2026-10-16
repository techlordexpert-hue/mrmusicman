# Mr.Music.Man
Static frontend in `public/`, one serverless API in `api/index.js`, data in Upstash Redis.

## Deploy
1. Create an Upstash Redis database; copy its REST URL and token.
2. In Vercel, import this project and add the four variables from `.env.example`.
3. Deploy. Log in with ADMIN_USER / ADMIN_PASS on the normal login page to open the admin dashboard.

## Notes
- The admin session is not an account in the database, so it never appears in the user list.
- Admins can open chats only after a user reports them.
- Downloads render songs as WAV in the browser. For a real catalogue, connect a licensed API (e.g. Jamendo) in `songs`.
- Reels use video links. For file upload, add Vercel Blob.
