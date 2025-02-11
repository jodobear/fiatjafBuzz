# Simple Nostr bot

The bot `npub1akh4jhw580wqv60qk65cc5dzcwd5zj4g23wf3yf9eqw97y2ghxcqjh3eqr` runs every alternate days and posts "GM fiatjaf" on week days and "gfy fiatjaf" on weekends using the following cronjob:

```
20 4 */2 * * [ $(date +\%u) -ge 6 ] && /home/jo/gocode/bin/noscl publish "gfy fiatjaf" || /home/jo/gocode/bin/noscl publish "GM fiatjaf"
```
