GB STUDY — GitHub + Vercel deployment (static website)

FILES
- index.html: complete standalone GB STUDY website
- vercel.json: simple static hosting configuration

ADMIN
- Demo password: GBADMIN2026
- This is a front-end-only demo password embedded in the HTML source. Anyone who can inspect the source can discover it. Do not use this for private data or real security.
- Admin changes (platforms/banners/settings) are stored in that browser's localStorage only. They do not automatically sync to other devices or survive clearing browser data.

PLATFORM LIMIT
- Maximum 100 platforms. Admin refuses the 101st new platform; editing an existing one remains allowed.

FASTER PLATFORM OPENING
- Platform arrow taps now navigate directly in the current tab, which is more reliable in mobile WebViews that block new tabs/popups. Telegram links still attempt the Telegram app deep link first, with web fallback.

DEPLOY WITH PHONE
1. Extract this ZIP on your phone so index.html and vercel.json are in one folder.
2. On GitHub, create a new repository named gb-study (Public or Private).
3. Upload index.html and vercel.json to the repository root (not inside an extra nested folder); commit changes.
4. Sign in to Vercel with GitHub at https://vercel.com/ and choose Add New → Project.
5. Import the gb-study repository. Framework preset: Other. Build command: leave blank. Output directory: leave blank or use ./ .
6. Click Deploy. When deployment finishes, open the .vercel.app URL and test platform links and admin.
7. Later updates: upload/commit the changed index.html to GitHub; Vercel automatically redeploys.

IMPORTANT LIMITATION
This is a static website. Admin edits are browser-local only; to share platforms/banners across users/devices, a database and server-side admin authentication must be added. I cannot sign into your GitHub/Vercel account or publish it without your own account authorization.
