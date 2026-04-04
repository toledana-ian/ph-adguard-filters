# ph-adguard-filters

AdGuard custom filter list targeting Philippine domains. Blocks PAGCOR-licensed gambling sites, adult content, and DNS-over-HTTPS providers.

## Filter Lists

| File | Description |
|------|-------------|
| [`gambling.txt`](./gambling.txt) | Philippine gambling sites — manually curated + all PAGCOR-accredited operators (March 2026) |
| [`porn.txt`](./porn.txt) | Philippine adult/porn sites |
| [`dns.txt`](./dns.txt) | DNS-over-HTTPS providers (prevents DNS bypass) |

## How to Use in AdGuard

1. Open **AdGuard** → **Filters** → **Custom Filters**
2. Click **Add custom filter**
3. Paste the raw URL of any filter file, e.g.:

```
https://raw.githubusercontent.com/toledana-ian/ph-adguard-filters/main/gambling.txt
https://raw.githubusercontent.com/toledana-ian/ph-adguard-filters/main/porn.txt
https://raw.githubusercontent.com/toledana-ian/ph-adguard-filters/main/dns.txt
```

## Sources

- **Gambling:** Manually curated list + [PAGCOR List of Accredited Gaming System Administrators and Registered Brands/Domain Names](https://www.pagcor.ph/regulatory/pdf/App%20Kits/List-of-PAGCOR-Accredited-Gaming-System-Administrators-and-Registered-Brands-and-Domain-Names-URLs.pdf) (as of March 30, 2026)
- **Porn:** Manually curated
- **DNS:** Common DNS-over-HTTPS providers

## Notes

- The gambling list covers **PAGCOR-licensed** operators (legal PH online gambling platforms). These are included because the goal is content filtering, not legality enforcement.
- Rules follow [AdGuard filtering syntax](https://adguard.com/kb/general/ad-filtering/create-own-filters/).
- Lists are updated manually. Check PAGCOR's regulatory page for the latest operator list.

## License

MIT
