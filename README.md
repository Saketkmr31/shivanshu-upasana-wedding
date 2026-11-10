# Shivanshu & Upasana Wedding Website

## Enable Google Sheet RSVP
1. Open https://script.google.com and create a new Apps Script project.
2. Paste the contents of `Code.gs` into the editor.
3. Run `setup()` once and approve Google's permission prompt. This creates **Shivanshu & Upasana — Wedding RSVP**. Copy the sheet URL from the execution log.
4. Choose **Deploy → New deployment → Web app**.
5. Set **Execute as: Me** and **Who has access: Anyone**, then deploy and copy the URL ending in `/exec`.
6. In `index.html`, set `GAS_WEB_APP_URL` to that URL and commit the change.

RSVP responses are appended with timestamp, name, phone, attendance, guest count and message. The website does not collect payment or sensitive information.