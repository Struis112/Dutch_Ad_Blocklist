# Dutch Ad Blocklist

A DNS-level ad and tracker blocklist focused on the Dutch advertising ecosystem. Compatible with AdGuard, AdGuard Home, Pi-hole, and any blocker that supports the AdGuard/AdBlock filter format.

## Subscribe

Add this URL directly to your blocker:

```
https://raw.githubusercontent.com/Struis112/Dutch_Ad_Blocklist/main/filter.txt
```

## What it blocks

- Dutch ad networks and affiliate platforms (Daisycon, TradeTracker, Awin, etc.)
- Dutch publisher ad servers (STER, DPG Media, Telegraaf, RTL, etc.)
- Dutch tracking and affiliate redirects
- General ad infrastructure (Google Ads, Amazon Ads, DoubleVerify, etc.)

## Sources

The list is compiled from the following sources, each clearly marked with a comment section inside `filter.txt`:

| Source | Description |
|---|---|
| **My custom entries** | Manually curated Dutch ad/tracker domains |
| [EasyList Dutch](https://easylist-downloads.adblockplus.org/easylistdutch.txt) | Classic Dutch ad filter, maintained by the EasyList team |
| [EasyDutch (uBO)](https://github.com/EasyDutch-uBO/EasyDutch) | Modern Dutch filter for uBlock Origin |
| [JohnyP36 Personal List](https://github.com/JohnyP36/Personal-List) | Personal Dutch blocklist targeting ads and anti-adblock |

## Recommended companion lists

These lists are too large to embed but pair well with this one. Add them as separate subscriptions:

| List | URL |
|---|---|
| Hagezi Light | `https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/light.txt` |
| OISD Basic | `https://dbl.oisd.nl/basic` |
| ph00lt0 Blocklist | `https://raw.githubusercontent.com/ph00lt0/blocklist/master/blocklist.txt` |

## How to add in AdGuard Home

1. Go to **Filters → DNS blocklists → Add blocklist → Add a custom list**
2. Paste the raw URL above and save

## How to add in Pi-hole

1. Go to **Group Management → Adlists**
2. Paste the raw URL and click **Add**
3. Run `pihole -g` to update gravity

## Contributing

Found a Dutch ad domain that should be blocked? Open an issue or pull request.
