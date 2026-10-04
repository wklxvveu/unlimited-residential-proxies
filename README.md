# Unlimited Residential Proxies: What "Unlimited" Actually Covers, Flat-Rate vs Per-GB Costs, and How to Pick the Right Plan

Search for "unlimited residential proxies" and you'll get two very different products wearing the same label.

One is a flat-rate residential plan where bandwidth is never metered — you pay for access and push as much traffic through it as the connection allows. The other is a metered GB plan that lets you generate an unlimited number of *endpoints*, which is a nice feature but has nothing to do with bandwidth being free.

Those are not the same thing, and providers rarely spell out the difference on the pricing page. This guide untangles which meaning applies where, shows the fair-use thresholds hiding behind the word "unlimited" at the major providers, and walks through 9Proxy's current plans for both models — with the actual numbers, including the price adjustment that took effect on June 1, 2026.

## Two meanings, one keyword

Ask yourself which of these you actually want before comparing anything:

**Unlimited bandwidth.** A fixed number of residential IPs, with no per-gigabyte meter. You can move 5 GB or 500 GB through the same IP and the bill doesn't change.

**Unlimited endpoints.** You buy traffic in GB and generate as many proxy endpoints as you like from the provider's pool — no per-IP activation fee, but every byte still comes out of your purchased balance.

Only the first one is genuinely "unlimited" in the sense most people mean. The second is unlimited *addresses*, metered *data*.

One more reality check: fully unlimited residential bandwidth at a fixed price is rare and expensive to provide, because residential IPs sit on real consumer devices that someone else is paying for. When a provider advertises unlimited residential traffic, there is almost always a fair-use clause with a number in it.

## How providers actually sell "unlimited"

Here's what sits behind the claim at the providers people most often compare. This is drawn from published specs and fair-use documentation:

| Provider | Proxy type | What "unlimited" covers | The catch |
| --- | --- | --- | --- |
| Bright Data | ISP (shared & dedicated) | Unlimited ISP proxy access | 100 GB/month per proxy fair use; overage billed at pay-as-you-go rates after email reminders |
| Oxylabs | ISP | No traffic restriction on ISP and dedicated datacenter proxies | Up to 100 concurrent sessions for the first 50 GB/month, then dropped to 10 for the rest of the month |
| Decodo | Static residential (ISP), datacenter | Unmetered traffic by default | Policy triggers only when a term exceeds 10 TB and a single IP exceeds 25 GB; concurrent sessions get reduced |
| Webshare | Datacenter, static residential, verified | Unlimited bandwidth on dedicated plans | Only at 1,000 premium / 100 private / 75 dedicated proxies. Free tier is 10 proxies and 1 GB |
| IPRoyal | ISP, datacenter, mobile | Unmetered ISP and datacenter usage | Mobile 4G/5G carries a 20–25 GB/day soft cap |
| ProxyScrape | Residential, shared datacenter | Unmetered traffic, no transfer-based cost growth | Connection ceiling of 60,000 per day |
| ProxyOmega | Residential | Flat rate by dedicated speed tier (200–1,000 Mbps) | You're buying throughput, not data — pick a tier that matches your pipeline |

Read that pattern carefully, because it tells you what to check in what order:

1. **Traffic cap.** Is there a GB number attached, even a soft one?
2. **Concurrency cap.** Can they throttle your session count instead of your bandwidth? That's the loophole most people miss, and it's exactly what Oxylabs and Decodo use.
3. **Minimum commitment.** Webshare's unlimited bandwidth only exists at 1,000+ proxies. Below that, you're metered.
4. **What happens on breach.** Email reminders, session reduction, or a real overage invoice — three very different outcomes.

A plan that says "unlimited" but cuts your concurrent sessions from 100 to 10 at the 50 GB mark is unlimited in name. For a scraper running parallel jobs, that's a wall.

## Where 9Proxy fits: flat-rate IPs vs metered GB

9Proxy runs two separate residential product lines, and it's worth understanding them mechanically rather than by marketing copy.

**Residential Proxies by IPs** is the flat-rate model. You buy a fixed number of residential IPs, and traffic through each active IP is unlimited. There's no per-gigabyte meter and no monthly subscription clock — this is a balance-based system, so **unused IPs never expire**. Each IP stays usable for a few hours up to roughly 24 hours, depending on the underlying device, and one IP counts as one usage when you forward through it. Rotation is handled by an auto-rotation proxy that switches at intervals you set on selected ports.

**Residential Proxies by GB** is the metered model. You buy a traffic balance and generate unlimited endpoints — only the data consumed is deducted, with no IP activation cost. Traffic is valid for 180 days (no expiry at all on Enterprise tiers), sessions can be sticky or rotating, and targeting goes down to country, state, city, ZIP and ISP level. This one runs entirely in the dashboard with username/password or IP whitelisting — no desktop app involved.

**Bundle packages** mix both: a block of IPs plus a GB balance, for workflows that need stable sessions on one job and wide rotation on another.

A few operational details worth knowing before you commit money:

> Two waste-reduction features are worth flagging because they're unusual. The **Today List** lets you reuse IPs that were active in the previous 24 hours at no extra cost, and there's a **replacement policy** where a proxy that fails within the first 60 seconds gets refunded. Offline IPs are also detected and replaced automatically.

And one honest caveat about the IP-based line: you'll need the desktop app for local port forwarding (optional proxy authentication on top). If you're deploying in containers or on a cloud box where you can't run a client, the GB line is the one that works out of the box, since authentication there is just credentials or a whitelisted IP.

## Every 9Proxy plan, with current pricing

9Proxy announced its first-ever price adjustment on May 18, 2026, affecting IP-based and bundle packages from June 1, 2026. GB-based prices were left untouched. Older third-party pages still list the pre-adjustment numbers — if you see 100 IPs for $20 or 1,000+500 IPs for $105, that page is stale.

| Plan | What you get | Effective rate | Price (USD) | Validity | Purchase |
| --- | --- | --- | --- | --- | --- |
| IP-Based — 100 IPs | 100 residential IPs, unlimited traffic | $0.24/IP | $24 | IPs never expire | [Get the 100 IP starter pack](https://bit.ly/9-Proxy) |
| IP-Based — 500 IPs | 500 residential IPs | $0.144/IP | $72 | IPs never expire | [Get 500 residential IPs](https://bit.ly/9-Proxy) |
| IP-Based — 1,000 IPs + 500 bonus | 1,500 IPs total | $0.084/IP | $126 | IPs never expire | [Get 1,000 IPs plus 500 free](https://bit.ly/9-Proxy) |
| IP-Based — 2,500 IPs | 2,500 residential IPs | $0.084/IP | $210 | IPs never expire | [Get the 2,500 IP package](https://bit.ly/9-Proxy) |
| IP-Based — 5,000 IPs | 5,000 residential IPs | $0.072/IP | $360 | IPs never expire | [Get the 5,000 IP package](https://bit.ly/9-Proxy) |
| IP-Based — 15,000 IPs | 15,000 residential IPs | $0.048/IP | $720 | IPs never expire | [Get the 15,000 IP package](https://bit.ly/9-Proxy) |
| IP-Based — 25,000 IPs | 25,000 residential IPs | $0.035/IP | $863 | IPs never expire | [Get the 25,000 IP package](https://bit.ly/9-Proxy) |
| IP-Based — 50,000 IPs | 50,000 residential IPs | $0.029/IP | $1,438 | IPs never expire | [Get the 50,000 IP package](https://bit.ly/9-Proxy) |
| Business — 100,000 IPs | 100,000 residential IPs | $0.023/IP | $2,300 | IPs never expire | [Get the 100,000 IP business pack](https://bit.ly/9-Proxy) |
| Business — 200,000 IPs | 200,000 residential IPs | $0.021/IP | $4,140 | IPs never expire | [Get the 200,000 IP business pack](https://bit.ly/9-Proxy) |
| Business — 500,000 IPs | 500,000 residential IPs | $0.018/IP | $8,625 | IPs never expire | [Get the 500,000 IP business pack](https://bit.ly/9-Proxy) |
| GB-Based — 5 GB | Unlimited endpoints, metered traffic | $3.00/GB | $15 | 180 days | [Get the 5 GB traffic pack](https://bit.ly/9-Proxy) |
| GB-Based — 50 GB + 5 GB bonus | 55 GB total | $2.10/GB | $105 | 180 days | [Get 50 GB plus 5 GB free](https://bit.ly/9-Proxy) |
| GB-Based — 100 GB | 100 GB traffic | $1.50/GB | $150 | 180 days | [Get the 100 GB pack](https://bit.ly/9-Proxy) |
| GB-Based — 200 GB | 200 GB traffic | $1.00/GB | $200 | 180 days | [Get the 200 GB pack](https://bit.ly/9-Proxy) |
| GB-Based — 1,000 GB | 1,000 GB traffic | $0.80/GB | $800 | 180 days | [Get the 1,000 GB pack](https://bit.ly/9-Proxy) |
| GB-Based — 2,000 GB | 2,000 GB traffic | $0.75/GB | $1,500 | 180 days | [Get the 2,000 GB pack](https://bit.ly/9-Proxy) |
| Enterprise GB — 3,000 GB | Unlimited validity, team mode, VIP pricing | $0.72/GB | $2,160 | No expiry | [Get the 3,000 GB Enterprise plan](https://bit.ly/9-Proxy) |
| Enterprise GB — 6,000 GB | Unlimited validity, team mode, VIP pricing | $0.70/GB | $4,200 | No expiry | [Get the 6,000 GB Enterprise plan](https://bit.ly/9-Proxy) |
| Enterprise GB — 10,000 GB | Unlimited validity, team mode, VIP pricing | $0.68/GB | $6,800 | No expiry | [Get the 10,000 GB Enterprise plan](https://bit.ly/9-Proxy) |
| Bundle — Starter | 100 IPs + 5 GB | — | $30 | 5 GB within 180 days; IPs never expire | [Get the Starter bundle](https://bit.ly/9-Proxy) |
| Bundle — Popular | 1,500 IPs + 50 GB | — | $180 | 50 GB within 180 days; IPs never expire | [Get the Popular bundle](https://bit.ly/9-Proxy) |
| Bundle — Pro | 5,000 IPs + 500 GB | — | $720 | 500 GB within 180 days; IPs never expire | [Get the Pro bundle](https://bit.ly/9-Proxy) |

Two things stand out in that table. The 1,000+500 tier is the obvious sweet spot on the IP side — the per-IP cost drops from $0.144 to $0.084 with a $126 spend, while the truly cheap rates require buying tens of thousands of IPs. And on the GB side, the price curve is steep: a 25 GB jump from 5 GB to 55 GB cuts the rate by 30%, while going from 100 GB to 1,000 GB only cuts it about 47%.

Enterprise tiers are the only place you get traffic that never expires, plus team mode for one owner and up to five members, per-member traffic controls, and no-expiry bandwidth sharing inside the team.

## Which model is cheaper for your workload

The decision comes down to one asymmetry:

- **IP-based charges per IP consumed and gives bandwidth away free.**
- **GB-based charges per byte and gives IP count away free.**

So the question isn't which is cheaper in general. It's whether your job burns more bandwidth per IP, or more IPs per gigabyte.

**Bandwidth-heavy, small IP set → IP-based.** Say you're pulling 30,000 pages a month at roughly 3 MB each. That's about 90 GB. On the GB side you're looking at the 100 GB pack for $150, or $200 to get headroom. On the IP side, if the workflow only needs a rotation pool of around 100 addresses — account sessions, logged-in workflows, price monitoring on a handful of regional sites — that's the $24 tier with zero traffic metering. Same job, meaningfully different bill.

**Rotation-heavy, small payloads → GB-based.** Now flip it: 50,000 distinct addresses, each used once for a lightweight JSON or geo-check request that costs a few kilobytes. On the IP side, every one of those IPs is a consumed unit — roughly $1,438 at the 50,000 tier. On the GB side, that whole run might not even consume 5 GB, which is $15. Buying IPs here is paying for something you throw away after a single request.

If you genuinely need both — stable sessions for one pipeline and wide rotation for another — the bundles do the arithmetic for you. Starter (100 IPs + 5 GB) is $30 versus about $39 bought separately. Popular (1,500 IPs + 50 GB) is $180 versus roughly $231 separately, a $51 saving. Pro (5,000 IPs + 500 GB) is $720 versus around $760 separately. The saving shrinks as you scale up, so buy the bundle for convenience at the top end, not for the discount.

## Discounts, trials and the invite code

There is no standing public coupon for 9Proxy, and the promotions that have run were time-boxed — the 2026 Lunar New Year event, for instance, applied a code-based discount to regular IP and GB packages between January 23 and February 23 of that year and is long over. Don't plan a purchase around a promo that may not exist next week.

What is reliably available is the referral discount. 9Proxy's affiliate program ties referrals to a code system, and the referred user gets **5% off their purchases** when signing up through a referral link or code. That applies to the purchase itself, so it's worth entering before you check out rather than after.

New-user trials also exist, but they're issued in limited batches depending on availability — the team has run a free-proxy trial campaign for new customers rather than a permanent free tier, so treat any free allocation as a bonus, not a right.

On payment: cards, crypto (USDT, BTC, ETH, LTC, DOGE and others), Alipay, Apple Pay and Google Pay are all accepted. Support runs 24/7 via Telegram, email and a ticket system.

👉 [Create a 9Proxy account with the invitation code applied](https://bit.ly/9-Proxy)

## What third parties say — including the criticism

Independent reviews of 9Proxy land mostly positive on price and pool size, with a consistent footnote about IP lifespans.

Geekflare's 2026 review is broadly favorable and spends a lot of space on setup paths — desktop app, browser-based access, mobile tooling, SOCKS5 for anti-detect browsers and custom scripts. ProxyLook's directory puts the provider at 3.9 stars and notes the pay-per-IP model with unlimited bandwidth as the differentiator. Caproxy's profile highlights the 60-second refund policy and the Today List reuse feature, and makes the fair point that this isn't a beginner-oriented product — the tooling assumes you know what you're doing with proxy rotation.

The criticism is worth reading rather than skipping. On Trustpilot the profile sits in the low range, and the recurring complaint in negative reviews is IPs dropping out mid-session — one reviewer described addresses failing after roughly an hour, causing security blocks on their accounts. 9Proxy's public reply is actually instructive: the company explained that this is inherent to dynamic residential proxies, since the underlying IP belongs to a real household, and that users who need long-lived fixed sessions should be looking at static ISP proxies instead of shared residential pools.

Read that as product-class information rather than a brand defect. If your workflow needs an IP that lives for days, no residential rotation pool from any provider will give you that reliably. The dashboard docs put natural residential uptime in the range of a few hours to about 24 hours, with roughly 3 hours as a typical lifespan. Plan for re-authentication, or plan for a static product.

There's also a positive user note in the alternative-software directories: stable connections that work well with anti-detect browsers like Dolphin Anty and AdsPower, at pricing that compares well to alternatives.

## Setup details that affect the bill

A few operational points that decide whether a plan works out:

**IP whitelisting needs a stable egress IP.** It's the cleanest authentication method until your own environment changes addresses — dynamic office connections and auto-scaling cloud instances will break it. Username/password with sub-users is safer in those setups.

**Sticky versus rotating is a workflow decision, not a preference.** Sticky sessions hold one IP across multiple requests, which you need for login state and multi-step forms. Rotating gives a fresh IP per request and is right for broad collection. Mixing both in one project is normal, and GB-based plans let you configure each endpoint differently.

**Geo-targeting granularity is country → state → city → ZIP → ISP.** ISP-level targeting is what makes a profile look like a genuine local user rather than "someone in California."

**Team and permission structure only comes with Enterprise.** If more than one person needs access with activity logs and per-member traffic controls, that's the tier, not the regular bundles.

## Quick answers

**Are there truly unlimited residential proxies anywhere?** Almost never in the absolute sense. The realistic version is a flat-rate plan with unlimited bandwidth per IP and a fair-use clause. If a provider promises unlimited everything with no threshold, the threshold is in the terms of service.

**Does 9Proxy's IP-based plan really have no traffic limit?** Per the official docs, traffic is unlimited during an IP's active time. You're limited by how many IPs you buy and how long each one stays usable, not by gigabytes.

**What happens when an IP fails?** Offline IPs are detected and replaced automatically, and a proxy that fails within the first 60 seconds is refunded. IPs already used in the last 24 hours can be reused free through the Today List.

**Do unused IPs expire?** No. The system is balance-based with no monthly subscription cycle, so leftover IPs stay in your account.

**Can I really generate unlimited endpoints?** On GB-based plans, yes — you generate as many proxy endpoints as you want and only data is deducted.

**Do I need to install anything?** For GB-based plans, no; it all runs in the dashboard. For IP-based plans, the desktop app handles local port forwarding.

## The bottom line

"Unlimited residential proxies" gets used for two products, and the one worth paying for depends entirely on where your costs actually come from. If huge traffic through a modest set of IPs is your pattern, the flat-rate IP model is the only structure that removes bandwidth from your budget — 9Proxy's entry point there is $24 for 100 IPs with no meter, and the 1,000+500 tier at $126 is where the per-IP economics start making sense. If your pattern is thousands of short-lived addresses making tiny requests, the GB plans will cost a fraction of what buying those IPs would.

Go in knowing two things: the IP-based line requires the desktop app and IP lifespans are measured in hours, not weeks, and the invite code is worth entering before checkout because it takes 5% off.

👉 [Start with a 9Proxy account and the invitation discount](https://bit.ly/9-Proxy)
