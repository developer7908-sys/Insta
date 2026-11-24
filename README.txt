HEMANTABARMAN INSTAGRAM BIO TRACKER
====================================

FILES
- index.html: Welcome page shown from your Instagram bio link.
- profile-photo.webp: Your supplied profile photo used on the welcome page.
- admin.html: Private dashboard.
- firebase-config.js: Firebase web app configuration and Instagram destination URL.
- firestore.rules: Firestore access rules.
- README.txt: Setup notes.

IMPORTANT NEXT STEPS
1. Keep all files in the same folder when uploading to GitHub Pages.
2. In firebase-config.js, set DESTINATION_URL to your exact Instagram profile URL, for example:
   https://www.instagram.com/YOUR_USERNAME/
3. Check Firestore Rules are published. The rules currently allow anonymous consented click records
   with device and timestamp, and reads only for the authenticated admin email configured in the rules.
4. In Firebase Authentication, ensure Email/Password is enabled and the admin user exists.
5. In GitHub Pages, publish from the repository root. Open the public site URL to test.
6. Open /admin.html and sign in with your Firebase admin email/password.

PRIVACY
This page records only the consented link click, device category (Mobile/Desktop), and timestamp.
It cannot identify who viewed your Instagram profile, reveal a visitor's Instagram username,
or show individual Instagram profile visits. Visitors can continue only after checking consent.

SECURITY
Never publish admin passwords or service-account private keys. Firebase web config is browser-visible;
Firestore Security Rules are what restrict database access. Consider Firebase App Check and abuse
protection before relying on public analytics.
