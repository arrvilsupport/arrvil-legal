AMP / Arrvil Music Player — legal pages
Prepared: 26 October 2026

Files to publish:
  index.html
  privacy.html
  account-deletion.html
  styles.css
  .nojekyll

Suggested GitHub Pages workflow:
1. Create a NEW public GitHub repository named arrvil-legal (do not use the AMP application repository).
2. Upload the five website files in the repository root on the main branch.
3. On GitHub, choose Settings > Pages > Build and deployment > Deploy from a branch > main > /(root) > Save.
4. Your URLs will normally have the following form (replace YOUR_GITHUB_USERNAME with the actual repository owner's username):
   https://YOUR_GITHUB_USERNAME.github.io/arrvil-legal/privacy.html
   https://YOUR_GITHUB_USERNAME.github.io/arrvil-legal/account-deletion.html
5. Open both links in an incognito browser; verify that the links work without login and the support email is correct.
6. Include URLs in release builds:
   flutter build appbundle --release --dart-define=AMP_PRIVACY_POLICY_URL=https://YOUR_GITHUB_USERNAME.github.io/arrvil-legal/privacy.html --dart-define=AMP_ACCOUNT_DELETION_URL=https://YOUR_GITHUB_USERNAME.github.io/arrvil-legal/account-deletion.html
7. Configure these same URLs in Google Play Console Privacy Policy and Data safety > Data deletion as applicable.

IMPORTANT BEFORE PUBLICATION:
- This website is a draft based on the AMP source audit, not a legal certification.
- Confirm all claims against your final app build, Firebase settings, online service terms, and your actual support/deletion practices.
- Verify that ARRVIL support mailbox is monitored and that you have an operational method to delete a Firebase Auth user after receiving a verified email request. Do not promise deletion unless you can perform it.
- If you disable online lyrics or cover art for licensing reasons, update the policy to match the published version.
- Do not publish passwords, keystores, signing configs, google-services.json, or the app's private repository in the public legal-pages repository.
- Test the account deletion request by sending a test email, and confirm you can receive and respond to it.
- No website has been deployed by ChatGPT. Creating the archive does not create public URLs.
