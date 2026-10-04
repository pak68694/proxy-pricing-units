# proxy plans: How to Choose Between Per-IP, Per-GB and Bundle Pricing (and What 9Proxy Actually Charges)

Search "proxy plans" and you'll get a wall of near-identical landing pages, each claiming to be the cheapest. Then you open three of them and realize the numbers aren't even measured in the same unit. One sells you bandwidth by the gigabyte. Another sells you IP addresses with "unlimited" traffic attached. A third hands you a bundle of both and calls it a plan.

That's the actual problem behind this search. It isn't finding a vendor — it's figuring out which billing model your workload belongs in, and then doing the arithmetic. Get the model right and the vendor choice becomes a short list. Get it wrong and you end up paying for gigabytes you never burn, or buying 5,000 IPs when a 100 GB pack would have done the job.

9Proxy is a useful concrete example here because it sells all three models from the same 20M+ residential pool, so you can compare the structures side by side instead of across four different vendors. Below are its current published rates, what changed in its June 2026 price adjustment, and how to work out which package is the cheaper buy for your job.

## First, stop comparing "plans" and start comparing billing units

Every residential proxy plan on the market is priced in one of three units:

**Per IP with unlimited bandwidth.** You buy a fixed number of IP addresses and push as much traffic through them as you like while they're active. Cost scales with how many separate sessions, accounts or profiles you need to keep apart — not with how much data you move.

**Per GB.** You buy a traffic allowance and rotate through the whole IP pool freely. Cost scales with data volume. Ideal when each request is small and the IP changes constantly.

**Bundles.** A fixed number of IPs plus a traffic allowance in one purchase, usually at a lower combined price than buying the two separately.

| Model | You're billed on | Best fit | Where it hurts |
| --- | --- | --- | --- |
| Per IP | Number of IPs / sessions | Long sessions, multi-accounting, bandwidth-heavy jobs | Buying more IPs than you actually run |
| Per GB | Traffic consumed | High-rotation scraping, SERP checks, ad verification | Heavy pages; monthly bills that grow with page weight |
| Bundle | IPs + GB together | Mixed workloads, client work you bill per project | Paying for the half you don't use |

If you can't say which of those three describes your workload, price tables won't help you. Most "which proxy is cheapest" arguments are really people comparing per-GB and per-IP providers as if they were the same product.

## 9Proxy's current proxy plans and prices

9Proxy runs a prepaid balance model rather than a monthly subscription. You top up, buy a package, and the balance is consumed as you use it. Its documentation describes two residential models — by IPs and by GB — plus bundle packs that combine them.

### IP-based residential: unlimited bandwidth per IP

This is the model for anything that needs a session to survive across many requests: account logins, carts, marketplaces, long-running jobs where you don't want to think about a traffic meter.

| Package | Effective rate | Total |
| --- | --- | --- |
| 100 IPs | $0.24/IP | $24 |
| 500 IPs | $0.144/IP | $72 |
| 1,000 IPs + 500 bonus IPs | $0.084/IP | $126 |
| 2,500 IPs | $0.084/IP | $210 |
| 5,000 IPs | $0.072/IP | $360 |
| 15,000 IPs | $0.048/IP | $720 |
| 25,000 IPs | $0.035/IP | $863 |
| 50,000 IPs | $0.029/IP | $1,438 |

The step from 100 IPs to 1,000 (+500 bonus) is where the per-unit price collapses, from $0.24 down to $0.084. If you're testing, 100 IPs is a reasonable entry point. If you're running anything semi-permanent, the 1,000+500 tier is the first one where the maths starts looking deliberate rather than experimental.

For teams moving industrial volume, the business tiers go further:

| Package | Effective rate | Total |
| --- | --- | --- |
| 100,000 IPs | $0.023/IP | $2,300 |
| 200,000 IPs | $0.021/IP | $4,140 |
| 500,000 IPs | $0.018/IP | $8,625 |

Two things worth knowing about this model before you buy. Each IP stays alive for a few hours up to roughly 24 hours, so you're buying *usages* rather than permanent addresses. And 9Proxy's "Today List" lets you reuse IPs pulled in the last 24 hours without spending another credit — the company's partner material puts the resulting saving at 20–30%. On top of that, the Auto-Refresh feature swaps out IPs that go offline within about 60 seconds, which matters if you're running unattended jobs.

### GB-based residential: pay for traffic, 180-day validity

Here you buy traffic and generate as many endpoints as you want. Rotation is automatic per request, or sticky for a session you define.

| Package | Effective rate | Total | Validity |
| --- | --- | --- | --- |
| 5 GB | $3.00/GB | $15 | 180 days |
| 50 GB + 5 GB bonus | $2.10/GB | $105 | 180 days |
| 100 GB | $1.50/GB | $150 | 180 days |
| 200 GB | $1.00/GB | $200 | 180 days |
| 1,000 GB | $0.80/GB | $800 | 180 days |
| 2,000 GB | $0.75/GB | $1,500 | 180 days |

The 180-day window is the detail that trips people up. Buy 1,000 GB at $800 and you need to consume it within six months. That works out to roughly 167 GB a month. If your actual burn rate is 40 GB a month, you've just paid for a third of a package you'll never touch — buy the 200 GB pack twice instead.

### Enterprise GB packages: validity removed

For always-on infrastructure, the same GB model without the clock:

| Package | Effective rate | Total | Validity |
| --- | --- | --- | --- |
| 3,000 GB | $0.72/GB | $2,160 | No expiry |
| 6,000 GB | $0.70/GB | $4,200 | No expiry |
| 10,000 GB | $0.68/GB | $6,800 | No expiry |

These are also the tiers where the headline "from $0.68/GB" figure on 9Proxy's marketing comes from.

### Bundle plans: IPs plus traffic in one purchase

| Bundle | What's inside | Price |
| --- | --- | --- |
| Starter | 100 IPs + 5 GB | $30 |
| Popular | 1,500 IPs + 50 GB | $180 |
| Pro | 5,000 IPs + 500 GB | $720 |

Bundle traffic carries the same 180-day validity. These exist for the fairly common situation where 80% of a project needs stable IPs and 20% needs throwaway rotation, and you'd rather make one purchase than two.

👉 [Check the full 9Proxy plan list and current balance pricing](https://bit.ly/9-Proxy)

## What changed in June 2026 — and what didn't

9Proxy announced its first-ever price adjustment on 18 May 2026, effective 1 June 2026. Two categories moved: IP-based packages and bundle packages. GB-based packages were left alone.

That explains why so many reviews still quote numbers that don't match. The 100-IP tier used to be $20; it's now $24. The 500-IP tier used to be $60; it's now $72. Older write-ups still show $25/$150/$600 for the bundles, where the current figures are $30/$180/$720.

The practical consequence, according to 9Proxy's own announcement, is that GB-based buyers saw no change at all, while IP-based buyers are now paying roughly 15–20% more per IP than they were in May. If a comparison article tells you 9Proxy's IP pricing starts at $0.20/IP, you're reading a pre-June-2026 snapshot.

## Working out which plan is cheaper for your job

Price tables tell you what things cost. They don't tell you which one you need. Here's the arithmetic that actually decides it.

**Case 1: 500 browser profiles for account management.** You need each profile pinned to its own IP for weeks. Traffic is modest but unpredictable. The 500-IP package at $72 gives you unlimited bandwidth across those IPs with no expiry on unused ones. A GB plan would charge you per gigabyte and rotate your IPs underneath you, which breaks the whole point. Per-IP wins, and it isn't close.

**Case 2: daily SERP checks and ad verification across 30 cities.** Requests are small — a few hundred KB each — but you want a different IP every time. Volume might land around 20–30 GB a month. Over six months that's 120–180 GB, so the 200 GB pack at $200 covers it with room to spare. Going per-IP here means buying hundreds of IP usages you don't need, since you never want the same IP twice.

**Case 3: scraping JavaScript-heavy product pages.** Page weight of 2–5 MB changes everything. A job hitting 100,000 pages a month is moving hundreds of gigabytes, and per-GB pricing turns into your largest line item. This is where the IP model's unlimited bandwidth stops being a footnote and starts being the reason to choose it.

The general rule: **if bandwidth is your variable, buy GB. If session count is your variable, buy IPs.** When both are variable, the bundles exist precisely for that.

## The fine print that quietly changes the maths

A few details from 9Proxy's documentation that belong in your decision, not in a features list:

- **Unused IP-based credits never expire.** Unused GB does, after 180 days (unless you're on an enterprise GB tier).
- **The IP-based model requires the desktop app.** It works through local port forwarding, with optional proxy authentication — so it routes traffic at the OS level and works with software that has no native proxy settings. The GB model works straight from the dashboard with username/password or IP whitelisting, no app needed. That's a real difference if you're deploying on a headless server.
- **IPs are not static.** Natural lifetime runs from a few hours to about 24 hours. Fixed rotation is available through the Auto Rotation Proxy, which rotates on selected ports at intervals you set.
- **Auto-refresh replaces dead IPs in about 60 seconds.** Useful; also means your effective IP count fluctuates.
- **No monthly commitment.** This is a balance system. There's no subscription to cancel, which is either liberating or a budgeting problem depending on how you work.

## Targeting, protocols and how you plug it in

The network advertises 20M+ residential IPs across 90+ countries, with targeting down to country, city, ZIP code and ISP, over HTTP/HTTPS and SOCKS5. The SOCKS5 support is why anti-detect browsers and automation stacks generally work without extra plumbing.

Access options, drawn from the vendor's own write-ups and reviews:

- **Proxy Program** — a desktop client that routes traffic at the OS layer, so any application inherits the proxy.
- **Proxy2Web** — browser-based access with standard username/password credentials, for quick manual checks.
- **ProxyHub / ProxyHub Lite / ProxyHub Pro** — mobile device management, with Lite on individual devices and Pro for centralised control across devices.
- **Public API** — programmatic session control and usage stats for pipelines.
- **Direct SOCKS5** — for anti-detect browsers, proxychains and custom scripts.

Support runs 24/7 via Telegram, email and a ticket system, according to the company's partner documentation. Uptime is claimed at 99.95%.

## Where 9Proxy sits against other budget proxy plans

Third-party numbers on 9Proxy diverge, and it's worth seeing the spread rather than one figure.

ProxyLook's directory entry gives it a 3.9-star rating, a 7.8/10 trust score, a 97% success rate and ~1,300 ms average response time, positioning it as a budget residential provider starting around $0.018–$0.02 per GB equivalent. A long-form case study on ProxyBros reports ~99.5% success rate and ~0.6 s average response across a month of testing with roughly 12M requests — a much rosier picture, and one produced on a different target mix. Traffic-Creator's June 2026 price survey places 9Proxy at roughly $1.30–$2/GB at standard volumes, second cheapest behind DataImpulse, while noting a 90–95% success rate on moderately protected targets versus 97–99% for Bright Data.

Read those together and the honest summary is: 9Proxy is a genuinely cheap residential option whose performance varies by target. The cheapness is consistent across sources; the success rate is not. Lab numbers don't transfer cleanly to your target list, which is why the smallest package exists.

## Who probably shouldn't buy these plans

Being fair about the boundaries:

- **Enterprise teams needing contractual SLAs, dedicated account management and compliance paperwork** are better served by the likes of Bright Data or Oxylabs. 9Proxy's top tiers reach those price points without the enterprise scaffolding.
- **Anyone whose targets are heavily protected.** If you're scraping sites with aggressive bot management, the 90–95% end of the third-party range is the relevant number, and a premium per-GB provider may pay for itself.
- **People who want one flat monthly invoice.** The balance model rewards planning and punishes drift. If you'd rather pay a predictable subscription, this isn't that.
- **Static datacenter or ISP proxies.** 9Proxy's documented lineup is two residential models. If you need fixed datacenter IPs, look elsewhere.

## Questions that come up before buying

**Are these subscriptions?** No. You buy packages against a balance. IP-based credits don't expire; GB credits expire after 180 days except on enterprise GB tiers.

**What's the cheapest way to start?** The 100-IP package at $24 if you need sessions, or the 5 GB pack at $15 if you just want to test the network against your targets. Given the third-party variance in success rates, starting small on your own target list is the sensible move.

**Can I reuse an IP I already used today?** Yes, within 24 hours, via the Today List, without spending another credit.

**Does it work with anti-detect browsers?** Yes — SOCKS5 and HTTP/HTTPS are both supported, which covers Dolphin Anty, AdsPower and similar tools. User reviews on software directories specifically call out compatibility with those two.

**How do I sign up?** Through an invite-code link. The code carries over into the account on registration.

👉 [Create your 9Proxy account and pick a plan](https://bit.ly/9-Proxy)

## The short version

Proxy plans are priced in three units, and picking the wrong unit costs more than picking the wrong vendor. Buy per IP when you need sessions to survive; buy per GB when you need rotation and your data volume is the variable; buy a bundle when a project genuinely needs both. On 9Proxy's current rates, the per-IP cliff is at the 1,000+500 tier ($126, $0.084/IP), the per-GB cliff is at 200 GB ($200, $1.00/GB), and the enterprise GB tier at 10,000 GB is where the advertised $0.68/GB actually applies. GB prices held steady in the June 2026 adjustment; IP and bundle prices did not.
