# best private proxies: how to pick clean residential IPs, and what 9Proxy charges for the first 100

Most people searching for private proxies are not confused about the concept. They know a proxy hides their IP. What they're actually trying to figure out is why two providers quoting "residential proxies" can differ by a factor of ten on price, and which of those numbers will still look reasonable once the first month's invoice lands.

There's a shorter version of that problem. Private proxy shopping comes down to three choices: what kind of IP you need, whether you pay per IP or per gigabyte, and how long the thing you bought stays usable. Brands matter less than people expect. Get those three wrong and even a well-reviewed provider will feel broken.

## What "private" is actually buying you

The word gets used loosely. In practice there are three tiers:

- **Public proxies** are free, shared with strangers, and already burned. Nothing serious should run through one.
- **Shared proxies** are paid but split across customers. Cheaper, and the IP reputation is whatever the worst user on the range made it.
- **Private proxies** are allocated to you alone, at least for the duration of your session. Cleaner reputation, predictable speed, no neighbour torching your IP at 3am.

One caveat worth saying out loud, because it catches people out: in the residential world, "private" rarely means an IP registered in your name forever. Real home connections in 9Proxy's pool have a natural uptime measured in hours up to roughly a day. Private means nobody else is on that address while you're using it, not that you own it for the year.

The other shift is that datacenter IPs have largely stopped being viable for anything defended. Cloud ASN ranges are public knowledge, and modern anti-bot systems flag them within dozens of requests. If your target is a search engine, a social platform, or a retail site with real bot protection, you need residential or ISP IPs whether you like the price or not.

## The decision that decides your bill: per IP or per GB

This is where most comparisons get vague, so here's the arithmetic.

**Per-GB pricing** charges for traffic. You can generate as many different endpoints as you want, and you're billed for what flows through them. It suits high-rotation work: lightweight scans, ad verification, geo-checking, API polling, anything where each request pulls a small page and you want a different IP each time.

**Per-IP pricing** charges for addresses, with bandwidth unmetered. You buy 100 IPs, you can push 10 GB or 400 GB through them and the cost doesn't move. It suits sustained sessions and heavy pages — JavaScript-heavy sites, image and video assets, long authenticated sessions.

The break-even is stark. Take 9Proxy's entry IP package at $24 for 100 IPs, which works out to $0.24 per IP with unlimited traffic. A per-GB provider charging $3/GB would bill you $0.24 after roughly 80 MB of traffic. Most real scraping workflows blow past 80 MB per IP without trying. On heavy pages, per-IP wins before you finish your first coffee.

The catch on the other side: per-IP means each address has a limited natural lifespan, and you can't manufacture more of them for free. If your job needs thousands of distinct exits in an hour, per-GB is the model that gives you that.

## Residential, ISP, mobile, datacenter: pick by target, not by budget

| IP type | Trust level | Rotation vs stability | Where it works |
| --- | --- | --- | --- |
| Datacenter | Low | Fast, cheap, rotating or dedicated | Sites with no meaningful bot defence |
| Residential (rotating) | High | New IP per request or per session | Scraping, SERP tracking, price monitoring, geo checks |
| Residential (sticky) | High | Holds one IP through a session | Logged-in workflows, carts, forms |
| ISP / static residential | High | Fixed address on a carrier subnet | Long-lived accounts that need one identity |
| Mobile | Very high | Static per session, carrier ASN | Warmed-up accounts, mobile app testing |

If you're buying one thing and want it to cover the most ground, rotating residential with a sticky option is the default. Everything else is a specialisation.

## Where 9Proxy fits

9Proxy sells residential IPs — the company advertises a pool of more than 20 million across 90-plus countries, with targeting down to country, state, city, ZIP and ISP. HTTP/HTTPS and SOCKS5 are both supported, which matters if you're pointing an anti-detect browser or a scraping framework at it. Directory listings put claimed uptime at 99.95%.

What's more interesting than the headline numbers is that 9Proxy runs two separate product lines that behave quite differently:

**Residential by IPs** is a balance-based model. You buy a block of IPs, each one is yours while it's alive, traffic is unmetered, and unused IPs don't expire. Practically, this is aimed at session-based work — the same address held across a login sequence or a multi-step form. Access runs through the desktop app, which does local port forwarding. There's also an Auto Rotation option that swaps IPs at intervals you set on selected ports.

**Residential by GB** is the newer system, and it's the one that will feel familiar if you've used other residential networks. You pay for traffic, generate as many endpoints as you want from a dashboard-based proxy generator, and pick sticky or rotating sessions. Authentication is username/password or IP whitelisting, targeting covers country through ISP, and exports come out as .txt or .csv with code samples. No app required.

That last distinction is the one people miss when they compare 9Proxy to a generic per-GB provider. If your scraping stack lives on a cloud server, the GB line is the one that installs cleanly. The IP line wants a local forwarder.

## Every 9Proxy package, with current prices

Pricing was adjusted on 1 June 2026 for the IP-based and bundle packages; the GB-based packages were left alone. Everything below is the post-adjustment structure.

### Residential proxy by IPs — one-off top-up, unlimited bandwidth, unused IPs don't expire

| Package | Cost per IP | Total | Buy |
| --- | --- | --- | --- |
| 100 IPs | $0.24 | $24 | [Start with the 100 IP pack](https://bit.ly/9-Proxy) |
| 500 IPs | $0.144 | $72 | [Get the 500 IP pack](https://bit.ly/9-Proxy) |
| 1,000 IPs + 500 bonus | $0.084 | $126 | [Take the 1,500 IP pack](https://bit.ly/9-Proxy) |
| 2,500 IPs | $0.084 | $210 | [Buy 2,500 IPs](https://bit.ly/9-Proxy) |
| 5,000 IPs | $0.072 | $360 | [Buy 5,000 IPs](https://bit.ly/9-Proxy) |
| 15,000 IPs | $0.048 | $720 | [Buy 15,000 IPs](https://bit.ly/9-Proxy) |
| 25,000 IPs | $0.035 | $863 | [Buy 25,000 IPs](https://bit.ly/9-Proxy) |
| 50,000 IPs | $0.029 | $1,438 | [Buy 50,000 IPs](https://bit.ly/9-Proxy) |

### Business IP packages

| Package | Cost per IP | Total | Buy |
| --- | --- | --- | --- |
| 100,000 IPs | $0.023 | $2,300 | [Business 100K IP package](https://bit.ly/9-Proxy) |
| 200,000 IPs | $0.021 | $4,140 | [Business 200K IP package](https://bit.ly/9-Proxy) |
| 500,000 IPs | $0.018 | $8,625 | [Business 500K IP package](https://bit.ly/9-Proxy) |

### Residential proxy by GB — 180-day validity unless marked otherwise

| Package | Cost per GB | Total | Validity | Buy |
| --- | --- | --- | --- | --- |
| 5 GB | $3.00 | $15 | 180 days | [Get 5 GB to test](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB bonus | $2.10 | $105 | 180 days | [Get 55 GB](https://bit.ly/9-Proxy) |
| 100 GB | $1.50 | $150 | 180 days | [Get 100 GB](https://bit.ly/9-Proxy) |
| 200 GB | $1.00 | $200 | 180 days | [Get 200 GB](https://bit.ly/9-Proxy) |
| 1,000 GB | $0.80 | $800 | 180 days | [Get 1,000 GB](https://bit.ly/9-Proxy) |
| 2,000 GB | $0.75 | $1,500 | 180 days | [Get 2,000 GB](https://bit.ly/9-Proxy) |
| 3,000 GB (Enterprise) | $0.72 | $2,160 | Unlimited | [Enterprise 3,000 GB](https://bit.ly/9-Proxy) |
| 6,000 GB (Enterprise) | $0.70 | $4,200 | Unlimited | [Enterprise 6,000 GB](https://bit.ly/9-Proxy) |
| 10,000 GB (Enterprise) | $0.68 | $6,800 | Unlimited | [Enterprise 10,000 GB](https://bit.ly/9-Proxy) |

### Bundles — IPs plus traffic in one purchase

| Bundle | Contents | Price | Buy |
| --- | --- | --- | --- |
| Starter | 100 IPs + 5 GB | $30 | [Grab the Starter bundle](https://bit.ly/9-Proxy) |
| Popular | 1,500 IPs + 50 GB | $180 | [Grab the Popular bundle](https://bit.ly/9-Proxy) |
| Pro | 5,000 IPs + 500 GB | $720 | [Grab the Pro bundle](https://bit.ly/9-Proxy) |

Three things worth noticing in those tables.

First, the numbers you'll see quoted in sponsored listings — $0.015/IP and $0.68/GB — are the far end of the curve, not the entry point. $0.015/IP is the 500,000-IP business tier. $0.68/GB is the 10,000 GB Enterprise tier. The realistic entry prices are $0.24 per IP and $3.00 per GB.

Second, the bundles are genuinely cheaper than assembling the same thing yourself. Starter at $30 beats $24 for 100 IPs plus $15 for 5 GB, a saving of $9. Popular at $180 beats roughly $126 in IPs plus $105 in traffic. That's not marketing arithmetic; it's the listed tiers added up.

Third, the GB line is competitive at volume and unremarkable at the low end. Published rates from mid-market residential providers generally sit somewhere between $3 and $8 per GB. At 5 GB, 9Proxy is at the bottom of that band. The real advantage shows up at 200 GB and above, where it lands at $1.00/GB and keeps falling.

## Which package fits which job

- **SEO and SERP rank tracking.** Rotating residential by GB in the 100–200 GB range. You need geographic breadth, not session stability, and each request is small.
- **Price monitoring on retail sites.** The GB line at 200 GB or more. Volume plus rotation, and full-page HTML adds up across thousands of SKUs.
- **Multi-account management in anti-detect browsers.** The IP line. One address, one profile, unlimited traffic, no per-request billing anxiety while a session runs.
- **Sneaker and ticket drops.** The IP line around 500–2,500 IPs, because the failure mode you're insuring against is a blocked checkout, not a bandwidth bill.
- **Heavy-content collection.** The IP line. If your pages carry 2–5 MB each, per-GB billing stops being the cheaper option fast.
- **Agencies reselling to clients.** The Pro bundle or an Enterprise GB package, mostly for the team mode and unlimited traffic validity.

If you're unsure, the honest advice is to skip the guesswork and start at the entry point on each model — 100 IPs for $24 and 5 GB for $15. Fifteen dollars to find out whether your target site likes the network is cheaper than an afternoon of comparison reading.

## Setup details that cause support tickets

Worth knowing before you pay, because none of this is obvious from a pricing table:

- The IP-based line runs through a desktop app doing local port forwarding. If your scraper lives on a VPS, plan for that, or use the GB line instead.
- The GB line is dashboard-only. Generate endpoints, export them as .txt or .csv, drop them straight into your code.
- Authentication is either username/password with sub-users, or IP whitelisting. Sub-users are the cleaner option when several tools or clients share one balance.
- Offline IPs are detected and replaced automatically, with the docs citing a window of about 60 seconds.
- Sticky and rotating sessions are both configurable on the GB line. Sticky is the right setting for anything logged in.
- SOCKS5 is supported out of the box, which is what most anti-detect browsers and proxychains expect.

## What to check before trusting any provider with real money

This applies to 9Proxy and to every competitor.

Third-party coverage of 9Proxy is mixed, and you should know that going in. Geekflare's review is positive and treats the post-adjustment pricing as competitive. Directory listings show a 3.9/5 aggregate rating with a 97% success rate and roughly 1.3 seconds average response time. At the same time, some 2026 review pages have reported service outages, and at least one of those pages was later updated to say the service was back up. Several of the sites publishing the negative takes are proxy resellers themselves, which doesn't make the reports false, but it does mean you should read them with the source in mind.

The practical response is a cheap audit rather than more reading:

1. Buy the smallest pack — $24 for 100 IPs or $15 for 5 GB.
2. Pull IPs from three or four of the regions you actually target, not just the US.
3. Point them at your real target and measure success rate and latency, not just "does it connect".
4. Check the IPs against an IP-quality or fraud-score lookup before you build anything on top of them.
5. Only then scale, and buy volume in one purchase rather than drip-feeding top-ups, since the per-unit price is entirely a function of tier.

And regardless of which provider you pick: rotate on public collection, hold one stable IP per logged-in identity, and stay inside the site's terms. Rotating an authenticated session across addresses is the fastest way to get an account flagged, and no proxy fixes that.

## FAQ

**Are 9Proxy's IPs dedicated or shared?**
They're allocated to you for the life of the address. Residential IPs in the pool have natural uptimes in the range of a few hours to about a day, so treat them as exclusively yours during your session rather than permanently assigned.

**Do unused IPs or traffic expire?**
Unused IPs on the IP-based line don't expire. GB packages carry a 180-day validity, and the Enterprise tier removes that limit entirely and adds team mode with up to five members.

**What's the minimum you can spend?**
$15 for 5 GB, or $24 for 100 IPs. There's no subscription on either line.

**Does it work with anti-detect browsers and scrapers?**
Yes. HTTP/HTTPS and SOCKS5 are both supported, and the GB line authenticates with username/password or IP whitelisting, which is what AdsPower, Dolphin Anty, BitBrowser and standard Python or Node clients expect.

**Is per-IP or per-GB cheaper?**
Per-IP breaks even at roughly 80 MB of traffic per IP against a $3/GB provider. Above that, per-IP is cheaper. Below it — or when you need thousands of distinct exits quickly — per-GB is.

## The short version

If you want the simplest answer to "which private proxy setup is right": start on the model that matches your traffic shape, not the brand with the loudest pool count. Heavy pages and stable sessions want per-IP with unlimited bandwidth. High-rotation, low-payload work wants per-GB.

👉 [Open a 9Proxy account and pick your first package](https://bit.ly/9-Proxy) — at $24 for 100 unmetered IPs or $15 for 5 GB, that's a small enough bet to find out in an afternoon whether it fits, instead of taking someone else's word for it.
