# Simple Nostr bot

The bot at `npub1akh4jhw580wqv60qk65cc5dzcwd5zj4g23wf3yf9eqw97y2ghxcqjh3eqr` posts "GM fiatjaf" every day and "gfy fiatjaf" every weekend using the following cronjobs:

```
15 6 * * 1-5 /home/jo/gocode/bin/noscl publish "GM fiatjaf"
15 6 * * 6,0 /home/jo/gocode/bin/noscl publish "gfy fiatjaf"
```
