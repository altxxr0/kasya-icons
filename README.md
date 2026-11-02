# kasya-icons

App icons used by the Kasya budgeting app for Philippine bank, e-wallet and loan apps that are not installed on the phone.

- `icons/<packageName>.png` is one 192x192 RGBA PNG per Android package name.
- `index.json` lists every icon that is present.
- Source: each app's public Google Play listing image, fetched at 192 px.
- All logos and trademarks belong to their respective owners and are used only to identify the apps.
- Raw URL pattern: `https://raw.githubusercontent.com/altxxr0/kasya-icons/main/icons/<packageName>.png`

## Interest rates

`rates.json` holds the base savings interest rate a year for each bank or savings pocket Kasya knows, by Kasya's institution key, with how often it is paid and the usual 20% Philippine final tax on deposit interest. Kasya downloads it at most once a day; a rate the user typed is never replaced.

- `ratePct`: percent a year (base rate, not a promo); `payout`: `DAILY`, `MONTHLY` or `YEARLY` (quarterly payers are listed as monthly).
- `verified`: false where no official bank page confirmed the figure; `source` and `note` say where it came from.
- Raw URL: `https://raw.githubusercontent.com/altxxr0/kasya-icons/main/rates.json`
