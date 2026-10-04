# netnut alternative: what to run after the FBI seizure, what it actually costs, and how to migrate without burning a week

If you're looking up a netnut alternative, you're probably not browsing out of curiosity. Either your dashboard stopped resolving, or someone on your team noticed the scrape volume drop and asked a question you didn't enjoy answering. Both of those mean you need a working replacement, priced clearly, with the billing model that matches how you use proxies.

## What actually happened to NetNut

NetNut wasn't a small operator. It was a residential proxy service run by Alarum Technologies, an Israeli company listed on the Nasdaq (ALAR), and it was one of the largest residential proxy networks Google's threat intelligence team tracked.

On July 2, 2026, the FBI and the IRS Criminal Investigation division seized hundreds of domains tied to NetNut. The company's homepage was replaced with a federal seizure notice. Google coordinated in parallel, disabling accounts and services used for malware command and control, and pushing Play Protect updates that warn users about and disable Android apps bundling NetNut's SDK. Google said the action cut the network's usable device pool by millions.

The scale figures behind that: Google's Threat Intelligence Group attributed at least 2 million consumer devices to the operation, tracked as Popa, and observed 316 distinct threat actor clusters using suspected NetNut exit nodes in a single week in June 2026. Google also said it has high confidence that many well-known proxy brands white-label the NetNut network — a detail worth remembering later in this article.

The financial side moved fast. Alarum told Reuters it had been notified about the domain seizures and said it would cooperate with investigators. Its stock fell roughly 67 percent over the following week. By July 8, the company's own domain was also displaying a seizure notice.

Alarum disputes the framing. Through legal counsel, the company described itself as a legitimate commercial proxy network with KYC checks and misuse monitoring in place. That position is on the record and unresolved. What isn't disputed is that the service is not something you can plan a production pipeline around right now. Reporting in late August 2026 indicated the company's operational storefront domain was still returning a seizure banner rather than a working gateway.

One more piece of context: this was the second takedown in six months. Google disrupted the IPIDEA network in January 2026, and when that happened, a significant share of IPIDEA's customers migrated to NetNut. Operators whose own capacity gets weakened tend to buy from competitors and quietly become resellers, which is why Google framed the problem as structural rather than as one company.

## The part that should worry you more than the seizure

The obvious move is to sign up with the next largest provider and get back to work. Google's own write-up pushed back on that instinct: a polished dashboard can be a thin shell over someone else's IP pool, and the composition of that pool can change underneath a stable-looking logo without any announcement.

So the practical question isn't "who is biggest." It's whether the provider can tell you where its residential IPs come from and how those households ended up in the pool. If the answer is a shrug and a marketing page about "20M+ IPs," you're making the same bet twice.

Ask this of any replacement, including the one this article spends the most time on:

- Is the network operated directly or resold, and if resold, from whom?
- What happens to your prepaid balance and your live sessions if the upstream disappears?
- Can you buy a small amount without a sales call, a contract, or a monthly commitment, so you can test the answers instead of believing them?

Those three questions eliminate most of the market.

## 9Proxy, briefly

9Proxy is a residential proxy provider that sells access to a pool of 20 million-plus residential IPs across 90-plus countries, supported by 8,000-plus servers with a stated 99.95 percent uptime. It speaks HTTP, HTTPS and SOCKS5, and it targets down to country, state, city, ZIP and ISP level.

The commercially interesting part is how it bills. Rather than a monthly subscription with a data ceiling, 9Proxy runs on a prepaid balance you spend against packages. Two distinct models sit on top of that:

Residential by IP gives you a fixed number of addresses with unlimited bandwidth. Unused IPs don't expire. Individual IPs stay alive for anywhere from a few hours to about 24 hours, and there's no natural rotation, though an auto-rotation proxy feature can cycle at intervals you set on selected ports. This model requires the 9Proxy desktop app, because it works by local port forwarding.

Residential by GB charges for traffic instead of addresses. You generate as many endpoints as you want and only the data is deducted. Traffic is valid for 180 days, or indefinitely on Enterprise packages. Everything runs in the dashboard, authenticated with username/password or an IP whitelist, with rotating or sticky session modes.

That distinction matters more than it looks. If your NetNut setup was traffic-metered, the GB model is the direct analogue and you never touch a local app. If you were paying for a fixed IP inventory to hold accounts or long sessions, the IP model is the one with unlimited bandwidth and no monthly data anxiety.

One pricing note before the tables. On May 18, 2026, 9Proxy announced the first price adjustment in its history, effective June 1, 2026 at 00:00 UTC. IP-based packages and bundle packages went up. GB-based packages were left alone. Any price list you find from earlier in 2026 is probably showing the old numbers, which is why the figures below reflect the current structure.

## Every package currently on the 9Proxy price list

### IP-based packages (unlimited bandwidth, IPs never expire)

| Package | Price per IP | Total | Purchase |
| --- | --- | --- | --- |
| 100 IPs | $0.24 | $24 | View price & sign up |
| 500 IPs | $0.144 | $72 | View price & sign up |
| 1,000 IPs (+500 bonus) | $0.084 | $126 | Check this package |
| 2,500 IPs | $0.084 | $210 | View price & sign up |
| 5,000 IPs | $0.072 | $360 | View price & sign up |
| 15,000 IPs | $0.048 | $720 | Check this package |
| 25,000 IPs | ~$0.035 | $863 | View price & sign up |
| 50,000 IPs | $0.029 | $1,438 | View price & sign up |
| 100,000 IPs | $0.023 | $2,300 | Check bulk pricing |
| 200,000 IPs | $0.021 | $4,140 | View price & sign up |
| 500,000 IPs | $0.018 | $8,625 | Check bulk pricing |

### GB-based packages (180-day validity)

| Package | Price per GB | Total | Purchase |
| --- | --- | --- | --- |
| 5 GB | $3.00 | $15 | Start with the smallest pack |
| 50 GB (+5 GB bonus) | $2.10 | $105 | View price & sign up |
| 100 GB | $1.50 | $150 | Check this package |
| 200 GB | $1.00 | $200 | View price & sign up |
| 1,000 GB | $0.80 | $800 | View price & sign up |
| 2,000 GB | $0.75 | $1,500 | Check this package |

### Bundle packages (IPs plus bandwidth, 180-day traffic validity)

| Package | Contents | Total | Purchase |
| --- | --- | --- | --- |
| Starter Bundle | 100 IPs + 5 GB | $30 | View price & sign up |
| Mid-tier Bundle | 1,500 IPs + 50 GB | $180 | Check this package |
| Pro Bundle | 5,000 IPs + 500 GB | $720 | View price & sign up |

### Enterprise GB packages (no expiry, team seats, activity logs)

| Package | Price per GB | Total | Purchase |
| --- | --- | --- | --- |
| 3,000 GB | $0.72 | $2,160 | Ask about Enterprise |
| 6,000 GB | $0.70 | $4,200 | Ask about Enterprise |
| 10,000 GB | $0.68 | $6,800 | Ask about Enterprise |

The Enterprise tier also adds a team mode with one owner and up to five members, per-member traffic controls, full activity logs and unlimited share-code creation. If you were running NetNut across a small team with shared credentials, that's the structural equivalent.

## What you were paying, versus what you'd pay now

NetNut's last published plan structure before the seizure, as reported in third-party reviews, looked roughly like this: rotating residential starting at $99 per month for up to 28 GB and scaling to $3,750 per month for up to 2 TB; static residential (ISP) from $99 per month for 7 GB up to $4,500 per month for 1 TB. Annual billing existed but the monthly commitment was the default.

| Your old NetNut plan | Effective rate | Closest 9Proxy equivalent | Effective rate |
| --- | --- | --- | --- |
| Rotating residential, 28 GB/month | ~$3.54/GB | 50 GB + 5 GB bonus pack | $2.10/GB |
| Rotating residential, 2 TB/month | ~$1.88/GB | 2,000 GB pack | $0.75/GB |
| Static residential, 7 GB/month | ~$14/GB | Not offered (no ISP line) | — |

Read that third row carefully. 9Proxy does not sell static residential or ISP proxies as a separate product line. It also has no datacenter or mobile product. The whole catalogue is rotating residential. If your NetNut spend was concentrated on static ISP addresses for long-lived account work, 9Proxy covers the rotating side of your stack and you'll need a second vendor for the static side. That's a real gap, not a footnote.

## What independent testing shows

Published benchmarks from vendors are marketing. The useful number comes from outside testing: a Geekflare review ran 300 sequential requests through rotating 9Proxy residential IPs against a major e-commerce platform sitting behind Cloudflare's bot protection, the same class of defence that kills datacenter proxies within the first few requests. Result: 293 passes (97.7 percent), 5 CAPTCHA challenges (1.7 percent) and 2 hard blocks (0.6 percent), at an average response time of 0.63 seconds. The same pattern through a datacenter pool produced a 34 percent block rate on the first pass.

Average latency around 0.63 seconds is honest rather than impressive. Residential routing adds hops. For scraping and verification work, a clean IP that completes the request beats a fast one that gets blocked on request three, which is the tradeoff you're accepting either way in this category. The same review flagged that 5 CAPTCHAs came from a single IP range and disappeared after rotation, and that the low hard-block rate suggests the pool is being actively cycled rather than left to rot.

## Where 9Proxy falls short

Worth knowing before you spend, because none of these are hidden:

- No self-serve free trial on the website. Trial access exists but you have to ask for it through the vendor's community threads, and availability varies. The 60-second refund window, which credits you back automatically if an IP fails within a minute of activation, is not the same thing as an evaluation period.
- Coverage is 90-plus countries. Solid for the US, UK, Western Europe and much of Southeast Asia. If your targets sit in niche geographies, verify before committing.
- Trustpilot complaints centre on the refund terms rather than the IP quality. Users who picked a plan that didn't fit their workload couldn't get their money back. The lesson is unglamorous: test on your own targets before buying a large tier.
- Speed is consistent rather than exceptional, with some slowdown in Southeast Asian locations during peak hours.
- IPs that fail later, not within the first 60 seconds, need manual replacement requests.

A caveat on the wider picture, since this article is about provider reliability: at least two third-party proxy comparison sites published claims of service interruptions at 9Proxy during mid-2026, one describing a blackout in late June and another a second gap in August. None of those claims are corroborated by 9Proxy's own channels, and both sites sell competing products, which is not a neutral position. Treat them as unconfirmed, and treat the checkpoint below as the thing that actually protects you.

## Migrating off NetNut in an afternoon

Most NetNut integrations pointed at a single gateway host with country and session behaviour encoded as suffixes in the proxy username. That means migration is usually a host change rather than a rewrite: swap the endpoint and translate your country and session flags into 9Proxy's format. The parts that need actual thought are these:

1. **Rotate credentials first.** Your NetNut username and password, your IP allowlists and any webhook endpoints you shared with the platform should all be treated as compromised after a federal seizure. That's ordinary hygiene after any vendor incident, and it's cheaper than finding out the hard way.
2. **Audit what you were actually doing.** High-volume scraping cares about pool size and rotation logic. Account workflows care about session stickiness. Geo-targeted collection cares about how deep the location coverage goes. Buy against the thing you actually do, not the thing that sounds most impressive.
3. **Pick the billing unit deliberately.** Traffic-heavy work with light per-request data belongs on a GB pack. Long sticky sessions with unpredictable data volume belong on IP packages with unlimited bandwidth. Buying the wrong unit is the single fastest way to conclude that a provider is overpriced.
4. **Test the failure paths, not just the happy path.** Run the same batch on your real targets for a week before you commit serious money. Then test what happens when a session expires, when a target flags an IP, and when you open a support ticket. Those tests surface the failure modes that matter, and they cost far less than a production outage.
5. **Split the dependency.** Routing most of your traffic through one provider and the rest through a second means a single vendor going dark degrades your operation instead of ending it. Managing two integrations is real overhead. So is a full stop.

## Questions people ask before buying

**Is NetNut gone for good?**

As of early July 2026, the main domain carried an FBI seizure notice, and late-August reporting indicated the operational storefront was also returning a seizure banner rather than a service. Nobody outside the investigation can predict the legal outcome. What's already true is that any balance you held sits with a seized operator, and your shared credentials and allowlists need rotating.

**What's the closest cheap replacement for NetNut's rotating residential plans?**

If you were buying traffic by the gigabyte, 9Proxy's GB packs are the direct functional equivalent with no desktop app required. Pricing is per gigabyte with prepaid balance and 180-day validity, which means irregular project schedules don't punish you with an expiry date.

**Does 9Proxy sell static ISP proxies?**

No. The product line is rotating residential only, in either IP-based or GB-based form. Long-lived static addresses need a separate provider.

**Does 9Proxy have a free trial?**

Not self-serve on the site. Trial access is occasionally offered to new users through the vendor's community threads, conditional on availability. 👉 9Proxy accounts start with an invite code, and the smallest GB pack costs $15, which is a cheaper way to evaluate the pool on your own targets than waiting for a trial slot.

**How much does 9Proxy discount referred sign-ups?**

9Proxy runs a lifetime affiliate program that pays up to 15 percent commission and advertises a 5 percent discount for users who sign up through a referral. Sign-up on the platform runs through an invite code, so the parameter travels with the link.

**Can I keep 9Proxy and a second provider running at the same time?**

Yes, and after the last six months, you probably should. Nothing about the platform requires exclusive use, and the balance-based model means you're not paying a monthly subscription penalty for keeping volume low on the backup.
