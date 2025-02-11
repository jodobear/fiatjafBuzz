# Simple Nostr bot

The bot `npub1akh4jhw580wqv60qk65cc5dzcwd5zj4g23wf3yf9eqw97y2ghxcqjh3eqr` posts "GM fiatjaf" every day and "gfy fiatjaf" every weekend using the following cronjobs:

```
20 4 */2 * * [ $(date +\%u) -ge 6 ] && /home/jo/gocode/bin/noscl publish "gfy fiatjaf" || /home/jo/gocode/bin/noscl publish "GM fiatjaf"
```
