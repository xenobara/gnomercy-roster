# GNOMERCY Roster

WoW Forever enlistment sheet for guild **GNOMERCY** (Gnome Council).

## Live data
Roster JSON is stored on [MantleDB](https://mantledb.sh) namespace `gnomercy-wow-roster` (claimed, public_read on `/roster`).

## Admin
Open the site with `?admin=gnomercy-council-reset` for Export / Reset.

Or with curl (write key is in `index.html` as `MKEY`):
```
curl https://mantledb.sh/v2/gnomercy-wow-roster/roster
curl -X POST https://mantledb.sh/v2/gnomercy-wow-roster/roster -H 'Content-Type: application/json' -H 'X-Mantle-Key: <key>' -d '{"entries":[]}'
curl https://mantledb.sh/v2/export/gnomercy-wow-roster -H 'X-Mantle-Key: <key>'
```

Claimed Mantle namespaces idle purge after ~90 days — open the page occasionally.
