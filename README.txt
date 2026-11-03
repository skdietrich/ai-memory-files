THE AI MEMORY FILES: GITHUB PAGES DEPLOYMENT
============================================

CONTENTS
- index.html       Main website with a GitHub Pages-compatible contact form
- thanks.html      Branded success page for completed submissions
- .nojekyll        Ensures GitHub serves the files directly without Jekyll processing

Keep your existing video file, videos/ai-mem.mp4, in the same relative location.
The MP4 is not included in this archive.

HOW TO PUBLISH
1. Open the GitHub repository already hosting this site.
2. In the folder GitHub Pages publishes (usually the root of the main branch,
   or /docs if configured that way), replace the existing index.html and add
   thanks.html and .nojekyll. Do not replace or remove your videos folder.
3. Commit the files. When the GitHub Pages deployment completes, visit the site.
4. Fill out the form and send one real test inquiry. FormSubmit will email an
   activation request to stephen@wolframtek.de. Open that email and approve
   the form. Check the spam folder if it does not arrive.
5. After activation, send a second test inquiry and verify the message reaches
   stephen@wolframtek.de and that the visitor is redirected to thanks.html.

WHY THIS VERSION IS DIFFERENT
- GitHub Pages does not run PHP. Do not upload contact.php; it cannot work there.
- The HTML form sends data to FormSubmit (https://formsubmit.co), which then
  delivers an email to stephen@wolframtek.de. No PHP backend is needed.
- The form has native required-field checks, a consent checkbox, honeypot, and
  FormSubmit's default CAPTCHA protection. The action and destination email
  appear in the public HTML. FormSubmit processes messages as a third party.
- Because the form intentionally accepts inquiries only, ask visitors not to
  send medical records, intimate conversation logs, financial or credential data.
- FormSubmit must be activated by the recipient email address; this build
  cannot verify inbox delivery before the live tests.

EXISTING FEATURES KEPT
- The Private Lives video is the only embedded video.
- The top-left title returns to the beginning of the page.
- Public examples remain fictionalized rather than copied from a private file.
- Mobile layout and the original investigation/review sections are preserved.

Troubleshooting:
- A blank video frame means videos/ai-mem.mp4 is missing, inaccessible, or
  encoded in a browser-incompatible format. Match exact capitalization.
- If you do not receive mail, verify FormSubmit activation and check spam.
- If the custom success page is not displayed, ensure thanks.html is in the
  same published directory as index.html.
