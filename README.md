# GNOMERCY Roster

**Live URL:** https://xenobara.github.io/

WoW Forever enlistment sheet for guild **GNOMERCY** (Gnome Council).

Source: https://github.com/xenobara/gnomercy-roster

## Persistence
Roster JSON lives on MantleDB (`https://mantledb.sh`) namespace `gnomercy-wow-roster`, entry path `roster`, with `public_read` enabled. Writes use `X-Mantle-Key` (embedded in the page for this private guild sheet). Survives redeploys of the static site.

Claimed Mantle namespaces can idle-purge after ~90 days — open the page occasionally.

## Admin
- In browser: open `https://xenobara.github.io/?admin=gnomercy-council-reset` for Export / Reset.
- Export: `curl https://mantledb.sh/v2/gnomercy-wow-roster/roster`
- Full namespace export: `curl https://mantledb.sh/v2/export/gnomercy-wow-roster -H "X-Mantle-Key: <key from index.html MKEY>"`
- Reset: `curl -X POST https://mantledb.sh/v2/gnomercy-wow-roster/roster -H "Content-Type: application/json" -H "X-Mantle-Key: <key>" -d '{"entries":[]}'`

## China / WeChat
GitHub Pages and MantleDB (Cloudflare) may be slow or blocked inside WeChat's in-app browser in mainland China. If the link warns or fails, tap **⋯ → Open in browser** (Safari/Chrome). Fallback mirror: `https://raw.githack.com/xenobara/gnomercy-roster/main/index.html`
