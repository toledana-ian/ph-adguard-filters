# ph-adguard-filters

AdGuard custom filter list targeting Philippine domains. Blocks PAGCOR-licensed gambling sites and adult content.

## Filter Lists

| File | Description |
|------|-------------|
| [`gambling.txt`](./gambling.txt) | Philippine gambling sites — manually curated + all PAGCOR-accredited operators (March 2026) |
| [`porn.txt`](./porn.txt) | Philippine adult/porn sites |

## How to Use in AdGuard

1. Open **AdGuard** → **Filters** → **Custom Filters**
2. Click **Add custom filter**
3. Paste the raw URL of any filter file, e.g.:

```
https://raw.githubusercontent.com/toledana-ian/ph-adguard-filters/main/gambling.txt
https://raw.githubusercontent.com/toledana-ian/ph-adguard-filters/main/porn.txt
```

## Sources

### Gambling

- **Manually curated** — OKBet, BingoPlus, Bet88, and other known PH gambling brands
- **PAGCOR Licensed Casinos** — [List of Registered Brands and Domain Names/URLs of Licensed Casinos](https://www.pagcor.ph/regulatory/pdf/App%20Kits/List-of-Registered-Brands-and-Domain-Names-URLs-of-Licensed-Casinos.pdf) (March 30, 2026)
- **PAGCOR Accredited Operators** — [PAGCOR Guarantee Site](https://www.pagcorguarantee.ph/) — all PAGCOR-licensed e-gaming operators and their registered domains
- **PAGCOR Reported Unauthorized Websites** — [Notice to the Public](https://www.pagcor.ph/regulatory/pdf/offshore/notice-to-the-public-reported-websites.pdf) — sites using fake PAGCOR certificates or operating without license
- **PAGCOR Fake Certificate Sites** — `verification.pagcorlicense.ph`, `licensing.newwavelicensing.ph`, `validator.pagcor-licence.ph` (flagged in PAGCOR notice)

### Porn

- **Manually curated** — tracked from site sidebars, StevenBlack hosts lists, Similarweb/Semrush traffic data, and community reports

## Notes

- The gambling list covers **PAGCOR-licensed** operators (legal PH online gambling platforms). These are included because the goal is content filtering, not legality enforcement.
- Rules follow [AdGuard filtering syntax](https://adguard.com/kb/general/ad-filtering/create-own-filters/).
- Lists are updated manually. Check PAGCOR's regulatory page for the latest operator list.

