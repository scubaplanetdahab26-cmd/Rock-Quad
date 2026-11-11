# Rock Quad Ledger (v1.0.0)

Offline cash ledger for the quad bike trips. Arabic and English. It runs on one iPhone (Abram's) and sends the daily report to Emad on WhatsApp.

## What is in the folder
| File | What it is |
|---|---|
| index.html | The app |
| report-template.html | Layout of the monthly report file |
| sw.js | Makes the app work with no signal |
| manifest.webmanifest, icon-*.png | Home Screen icon and name |

## Put it online once (free)
The iPhone can only install an offline app from an https website. Pick one:

**A. GitHub Pages (recommended, free, permanent)**
1. On github.com create a new public repository, e.g. `rock-quad`.
2. Upload all files in this folder (Add file › Upload files), then Commit.
3. Settings › Pages › Source: "Deploy from a branch", branch `main`, folder `/ (root)` › Save.
4. After a minute the app is at `https://<your-user>.github.io/rock-quad/`.

**B. Netlify Drop**
Go to app.netlify.com/drop, sign in for free, and drag this folder onto the page. You get an https link.

Your data never goes to that website. The site only delivers the app files. Everything you type stays on the phone.

## Install on the iPhone
1. Open the link in **Safari**.
2. Tap Share › **Add to Home Screen** › Add.
3. Always open the app from the new **Rock Quad** icon. A Safari tab keeps separate data.
4. First start: choose the language, name of who closes the day (Abram), Emad's WhatsApp number, and the cash in the box now.

## Daily use
- **+ Trip** › time, route, guide. Then **+ Add guests**: people, bikes, the price you agreed (prices are not fixed, type it), currency (EGP, USD, EUR), paid by cash / InstaPay / e-wallet / pays later, who referred them and their commission (typed, paid now or owed).
- **Cash** tab › **+ In / Out** for fuel, spare parts (write the part and bike number), repairs, fees, commission, camp & tea, water, etc. Add a receipt photo if you like.
- Only **cash** counts in the box. InstaPay and e-wallet are shown separately.
- **Close** tab at the end of the day: count the cash, close, then **Send to Emad on WhatsApp** (WhatsApp opens with the report, tap Send).

## Backups (important)
- **More › Save backup file** after closing: save to Files / iCloud Drive or send it to yourself on WhatsApp.
- **More › Monthly report file** on the 1st of each month: one file with every detail of the month that opens in any browser. It is also a backup of that month. Send it to Emad.
- **More › Restore from file** reads a backup or a monthly file back in, for example on a new phone.
- Deleting the app icon deletes its data. Keep backups.

## Updating the app later
Replace the files on the website. In sw.js change the version in `CACHE` (e.g. `rockquad-v1.0.1`) so phones pick up the new version the next time they open the app with internet.
