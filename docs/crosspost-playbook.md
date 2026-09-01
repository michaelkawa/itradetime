# Cross-post playbook — legitimate version

Goal: get Watch Cartel visible across the same communities a fake-listing
scheme would target (WatchUSeek, Omega/Rolex Forums, r/Watchexchange,
Chrono24, eBay, IG/TikTok) — without ever posting a watch that isn't real,
and without the "message us, it just sold" bait mechanic. See
`docs/marketplace-posting-rules.md` for why that mechanic is a non-starter
everywhere it'd run.

Three moves cover the same ground:

## 1. Post real inventory, credit the source

Every FS post is a watch Watch Cartel (or Michael personally) actually has in
hand or has a confirmed dealer commitment on — never a placeholder. Where the
platform allows it (WatchUSeek post body, IG/TikTok caption or bio, personal
site), add a plain attribution line:

> Sourced through **The Watch Cartel** — thewatchcartel.com

No link where the platform bans it (eBay body text, WatchUSeek signature) —
put the URL only in the seller's profile/bio field on those platforms instead.
This is the literal "crossposted to thewatchcartel.com" idea from the original
ask, just attached to something real.

## 2. Post real WTB / sourcing requests as sourcing requests

For a watch that isn't in hand — the case the fake-listing idea was actually
trying to solve — post it as what it is: a **WTB / sourcing** post, not an FS
post. "Looking to source a [ref] for a member, dealer-network pricing —
DM if you can quote it" is a completely normal, rules-compliant post on every
forum above, and it's the real mechanism the business runs on (per
`affiliates.html`: "members tell us the exact watch they want... it gets put
out to a network of dealers"). It generates exactly the same kind of inbound
interest as an FS post, truthfully.

## 3. A public "currently sourcing" page members and posts can point to

Rather than scattering fake FS posts, give cross-posts something real to
link to: a page on thewatchcartel.com listing current live WTB requests (ref,
condition wanted, no pricing commitment) pulled from actual member asks. A
forum/Reddit post can then legitimately say "full WTB board — thewatchcartel.
com" instead of implying a specific watch is sitting in inventory.

This is a real feature request (new page + a way to keep it current), not a
one-line fix — flag if you want it built; it's out of scope for this pass
since it needs a decision on how the WTB list gets populated/updated
(manual edit vs. a form).

## Caption templates (copy/paste, edit the bracketed parts)

**WatchUSeek / Omega / Rolex Forums post body** (once account meets each
forum's posting threshold):
```
[Ref] — [condition, box/papers status] — sourced through The Watch Cartel
dealer network. thewatchcartel.com for how the sourcing works.
```

**Reddit r/Watchexchange** — omit the link entirely (self-promo removal
risk); if posting a personal trade, no business mention at all. If Watch
Cartel wants a subreddit presence, that's a mod-permission conversation, not
a per-post workaround.

**Instagram / TikTok caption:**
```
[Ref] moved through the network this week. Link in bio for how sourcing
works — thewatchcartel.com
```

**eBay:** no Watch Cartel mention in the listing itself (Links Policy
violation even as plain text). Seller "About" page only, if used at all —
confirm current About-page rules before adding anything there.

## Tracking without a backend

Since this is a static site, use UTM-tagged links so you can tell which
platform is actually converting, e.g.:

```
https://thewatchcartel.com/?utm_source=watchuseek&utm_medium=crosspost&utm_campaign=sourcing
https://thewatchcartel.com/?utm_source=instagram&utm_medium=bio&utm_campaign=sourcing
```

Check referrer/UTM data in whatever analytics is already wired to the site
(none found in this repo's HTML — if there's no analytics yet, that's a
separate, smaller task worth doing before running any of this at volume, or
none of it is measurable).
