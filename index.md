# ConsentZap — say no to cookie banners, automatically

ConsentZap answers “Reject all” for you through each site’s own consent tool, checks that the refusal was actually saved, and blocks the trackers that load anyway.

- For Safari on Mac, iPhone and iPad, and Firefox on desktop and Android.
- Status: coming soon (not yet in the App Store or on addons.mozilla.org).
- Website: https://consentzap.app/ · Privacy policy: https://consentzap.app/privacy.html

## Not just hidden. Refused.

Most banner tools click whatever button they find, or simply hide the banner and hope. ConsentZap says no the way the site expects, then checks the answer stuck.

- **Rejects through the site’s own consent tool.** Works with the consent platforms most sites use — OneTrust, Cookiebot, Didomi, Usercentrics, Google’s consent dialog, CookieYes and about 1,200 more. It walks through “Manage options” screens and switches off every optional purpose, including “legitimate interest”.
- **Checks the refusal was saved.** After saying no, it reads the site’s own consent record. You see “rejected — verified” only when the record proves it.
- **Handles every banner on the page.** Some sites stack two or three consent tools. ConsentZap deals with each one in turn, even when they appear only after you start scrolling.
- **Blocks trackers that ignore your answer.** Plenty of sites load analytics and ad trackers no matter what you choose. ConsentZap blocks over 3,500 known tracking domains — but never a company’s own resources on its own site.
- **One tap when a site misbehaves.** If a page breaks, pause blocking for that site until you close the browser. Your “no” to cookies stays in place.

## What makes it different

| | Typical banner tools | ConsentZap |
|---|---|---|
| Refuses through the consent tool | Sometimes — often just hides the banner | Yes |
| Checks the refusal was saved | No | Yes, for the main consent platforms |
| Several banners on one page | Usually the first one only | Yes |
| Blocks trackers that load anyway | No | Yes |
| Tells you when it couldn’t refuse | Rarely | Yes — “dismissed, not verified” or “failed” |
| Ever clicks “Accept” | Some do | Never |

## Where it works

- Safari on Mac — macOS 12 or later — coming soon
- Safari on iPhone & iPad — iOS 17 or later — coming soon
- Firefox — Windows, Mac, Linux — coming soon
- Firefox for Android — coming soon

## Private by design

- **No data collected.** No accounts, no analytics, no telemetry. Everything ConsentZap does happens on your device.
- **No calls home.** The extension makes no network requests of its own. Its tracker list ships with it and updates with the app.
- **No cookies here either.** This website uses no cookies, no analytics and no external fonts — so it has no banner to reject.

## Questions

**Does ConsentZap ever accept cookies for me?**
No. It only ever chooses “reject” or the most restrictive option a site offers. If a site leaves no way to refuse, ConsentZap tells you instead of clicking “Accept”.

**What does “rejected — verified” mean?**
After refusing, ConsentZap reads the consent record the site itself stores (for example its consent cookie or the industry-standard TCF data) and confirms every optional purpose is off. If it can only hide a banner, it says “dismissed — rejection not verified”.

**Will blocking break sites?**
Rarely. Video embeds, fonts, login buttons and anti-bot checks are never blocked, and a company’s own resources load on its own site. If a page still misbehaves, pause blocking for that site with one tap.

**Why are there two switches in Safari?**
Safari runs tracker blocking as a separate “content blocker”. Turn on both *ConsentZap* and *ConsentZap Blocker* in Safari’s Extensions settings.

**Ads or trackers still show on one site in Safari?**
Safari can switch content blockers off for a single site. Open the page menu in the address bar (the “AA” or page-settings button) and choose *Turn On Content Blockers*. To check every site: Settings → Apps → Safari → Content Blockers, and make sure *Other Websites* is on.

**How much will it cost?**
Pricing will be announced at launch.

---

Consent rules: [DuckDuckGo autoconsent](https://github.com/duckduckgo/autoconsent) (MPL-2.0) · Tracker list: [Disconnect](https://disconnect.me/trackerprotection) (CC BY-NC-SA 4.0) · © 2026 ConsentZap
