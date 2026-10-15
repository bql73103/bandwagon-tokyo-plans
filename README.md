# bandwagonhost tokyo plan: The Tokyo Plan v1 and v2 vs the CN2 GIA lineup — prices, stock, China routing, and the 6.77% coupon

Searching for BandwagonHost's Tokyo plans lands you on two products that share a city and little else. **The Tokyo Plan** is a limited-stock, annual-only line in the Tokyo DC39v2 datacenter: two versions, **$79 and $99 a year**, sold in flash batches that disappear until restock. The **Tokyo CN2 GIA** lineup at Equinix TY8 is the always-available premium tier, starting at **$899.99/year**. Most comparison posts blur the line between them, which makes the $79 plan look like a cheap version of the $899 plan. It isn't, and the differences matter.

The short version: for roughly the price of one month of the CN2 GIA starter, The Tokyo Plan v2 gives you a full year of 2 AMD cores, 2 GB RAM, 40 GB SSD, and 1 TB of monthly traffic on a 5 Gbps port. The standing coupon code **BWHCGLUKKB** takes 6.77% off at checkout, bringing v1 down to **$73.65** and v2 to **$92.30**.

> **Quick picks**
> - Most people: **The Tokyo Plan v2**, $99/year, $92.30 after the coupon. Double the config of v1 for $20 more.
> - Tightest budget, single-purpose box (proxy, small relay, monitoring): **The Tokyo Plan v1** at $73.65 after the code.
> - Audience heavily on China Telecom, or you need more than 2 cores: the **Tokyo CN2 GIA** tiers from $899.99/year.
>
> 👉 [Check The Tokyo Plan v2 stock and current price](https://bwh81.net/aff.php?aff=77528&pid=163)

## What "The Tokyo Plan" actually is

The Tokyo Plan is BandwagonHost's limited-edition annual VPS line hosted in Tokyo DC39v2 (JPTYO_39), running KVM virtualization under the familiar KiwiVM panel. Two versions exist, both annual-only with no monthly billing. Outbound traffic uses a mixed, per-carrier-optimized upstream, and the return path to mainland China rides CMI for all three carriers. Stock is deliberately scarce: when a batch sells out, it's gone until the next restock, so availability changes week to week.

Some context for anyone new to the brand. BandwagonHost, the service behind the "搬瓦工" nickname in Chinese tech circles, has sold self-managed KVM VPS since 2012 under IT7 Networks. It owns its hardware and IP space, which is partly why its Japan pricing is where it is: Tokyo capacity is expensive, and this brand doesn't resell someone else's cage. The plans are marketed at low-latency use cases — game servers, streaming relays, proxies, anything where distance to East Asian users is the whole point. Tokyo sits under 10ms from most of Japan and close enough to mainland China that optimized routing actually changes the experience.

### v1 vs v2, and the fine print most posts skip

|  | The Tokyo Plan (v1) | The Tokyo Plan v2 |
| --- | --- | --- |
| CPU | 1 AMD core | 2 AMD cores |
| RAM | 1 GB | 2 GB |
| SSD | 20 GB RAID-10 | 40 GB RAID-10 |
| Monthly traffic | 500 GB | 1,000 GB |
| Port speed | 2.5 Gbps | 5 Gbps |
| Sustained CPU cap (TOS) | ~30% of one core | ~45% of one core |
| Price | $79.00/yr ($73.65 w/ code) | $99.00/yr ($92.30 w/ code) |

Here's the detail that rarely makes it into the listing pages: the terms of service cap **sustained CPU usage** at roughly 30% of one core on v1 and 45% on v2. For a proxy, a small relay, or a low-traffic site, you'll never feel it. For sustained transcoding or any always-busy workload, neither plan is the right tool, and no amount of port speed fixes a scheduler that's throttling you. This cap is also why v1's 2.5 Gbps port is less generous than it sounds on paper. You'll hit the CPU ceiling long before the port.

If both versions are in stock, v2 is the one to get. The $20 difference amortizes to under $1.70 a month, and you get double the cores, RAM, storage, and traffic, plus a port twice as wide.

## The full Tokyo lineup and current prices

BandwagonHost currently sells eight Tokyo plans across two product lines: the two flash-stock Tokyo Plan versions at DC39v2, and six CN2 GIA tiers at Equinix TY8. The CN2 GIA tiers were all showing in stock in the latest data synced from BandwagonHost's own stock feed; the Tokyo Plan versions come and go.

| Plan | CPU · RAM · SSD | Traffic · port | Routing | Annual price | Order |
| --- | --- | --- | --- | --- | --- |
| The Tokyo Plan (v1) | 1 core · 1 GB · 20 GB | 500 GB · 2.5 Gbps | Hybrid out, CMI return | $79.00 | [Order v1](https://bwh81.net/aff.php?aff=77528&pid=162) |
| The Tokyo Plan v2 | 2 cores · 2 GB · 40 GB | 1,000 GB · 5 Gbps | Hybrid out, CMI return | $99.00 | [Order v2](https://bwh81.net/aff.php?aff=77528&pid=163) |
| SPECIAL 40G KVM PROMO V5 (Tokyo CN2 GIA) | 2 vCPU · 2 GB · 40 GB | 500 GB · 1.2 Gbps | CN2 GIA · 9929 · CMI | $899.99 | [Order](https://bwh81.net/aff.php?aff=77528&pid=108) |
| SPECIAL 80G KVM PROMO V5 (Tokyo CN2 GIA) | 4 vCPU · 4 GB · 80 GB | 1 TB · 1.2 Gbps | CN2 GIA · 9929 · CMI | $1,559.99 | [Order](https://bwh81.net/aff.php?aff=77528&pid=109) |
| SPECIAL 160G KVM PROMO V5 (Tokyo CN2 GIA) | 6 vCPU · 8 GB · 160 GB | 2 TB · 1.2 Gbps | CN2 GIA · 9929 · CMI | $2,999.99 | [Order](https://bwh81.net/aff.php?aff=77528&pid=110) |
| SPECIAL 320G KVM PROMO V5 (Tokyo CN2 GIA) | 8 vCPU · 16 GB · 320 GB | 4 TB · 1.2 Gbps | CN2 GIA · 9929 · CMI | $5,899.99 | [Order](https://bwh81.net/aff.php?aff=77528&pid=111) |
| SPECIAL 640G KVM PROMO V5 (Tokyo CN2 GIA) | 10 vCPU · 32 GB · 640 GB | 6 TB · 1.2 Gbps | CN2 GIA · 9929 · CMI | $9,989.99 | [Order](https://bwh81.net/aff.php?aff=77528&pid=123) |
| SPECIAL 1280G KVM PROMO V5 (Tokyo CN2 GIA) | 12 vCPU · 64 GB · 1280 GB | 8 TB · 1.2 Gbps | CN2 GIA · 9929 · CMI | $18,989.99 | [Order](https://bwh81.net/aff.php?aff=77528&pid=125) |

Two billing notes. The CN2 GIA tiers can also be billed monthly if you'd rather not commit annually; the starter runs $89.99/month. Everything else in the table is annual USD, and traffic is monthly, with 1 TB counted as 1,000 GB.

## The Tokyo Plan or Tokyo CN2 GIA: which one deserves your money

For most readers searching this exact keyword, the decision is simpler than the comparisons suggest. If your budget is anywhere near $79–$99, the CN2 GIA line isn't in play at all — its entry tier costs about nine times the v2's annual price, and v2's entire first year costs roughly what one month of the CN2 GIA starter does. You're really choosing between v1 and v2, and v2 wins unless you need the absolute cheapest box for a single lightweight job.

The CN2 GIA tiers earn their price in one specific situation: your users sit heavily on China Telecom and you want the dedicated premium return path. At Equinix TY8, Telecom traffic rides CN2 GIA, Unicom rides 9929, and Mobile rides CMI. That's tri-carrier optimization with the carrier-grade Telecom route guaranteed, which matters for live streaming or anything latency-sensitive where a Telecom audience pays the bills. Hardware matches the price: a 2026 performance review of the JPTYO_8 facility measured disk I/O around 1,126 MB/s on NVMe storage, and the 1.2 Gbps port held up under real load.

A few differences worth weighing before you pick a side:

- **Port speed flips the expectation.** The $99 plan has a 5 Gbps port; the $899.99 plan has 1.2 Gbps. If raw bandwidth matters more than routing pedigree, the cheap plan wins on paper.
- **Both Tokyo lines are locked to their datacenter.** No migration on the Tokyo Plan, no migration on the CN2 GIA tiers either. If you think you might want to relocate the VPS later, neither is the flexible option.
- **Scaling stops differently.** The Tokyo Plan tops out at v2's 2 cores. The CN2 GIA line climbs to 12 cores, 64 GB RAM, and 8 TB of traffic if you need a genuinely big box in Tokyo.

👉 [See the Tokyo CN2 GIA tiers and current stock](https://bwh81.net/aff.php?aff=77528&pid=108)

## What you'll really pay: the coupon, renewals, and refunds

The listed prices aren't the floor. **BWHCGLUKKB** is BandwagonHost's standing 6.77% discount code. Enter it at checkout and The Tokyo Plan v1 lands at **$73.65/year**, v2 at **$92.30/year**. The same code works on the regular CN2 GIA plans too, whose listed prices are pre-discount, so there's no reason to ever order without it. It's a standing code rather than a first-order gimmick; long-running coverage of it notes that it shaves money off renewals as well.

Billing on the Tokyo Plan is annual-only, so the number you see at checkout is the number you pay for the whole year. No surprise month-two price jump, because there is no month two at a different rate.

Refund terms give you a genuine test window. A 30-day money-back guarantee applies across the plans, and the Tokyo Plan listings add two specifics: if the assigned IP gets blocked by the GFW within 30 days, you can claim a refund, and the standard refund holds as long as you've used under 10% of the traffic. Read that as permission to test the routes hard in week one. If your local line and the return path don't get along, you'll know quickly, and you should act within the window rather than in week four.

👉 [Order The Tokyo Plan v1 — runs $73.65 after the coupon](https://bwh81.net/aff.php?aff=77528&pid=162)

## How the China routing works, and where it can disappoint

Both Tokyo lines reach mainland China directly, but they take different roads. The Tokyo Plan's outbound is a hybrid that the provider describes as an asymmetric, dynamically adjusted mix of CMI, Unicom 9929, regular Unicom 4837, CN2 GIA, and ChinaNet paths, picking the best available route per carrier. The return trip for all three Chinese carriers rides CMI (China Mobile International). That return choice is a big part of why the plan is cheap: CMI return is solid, but it's not the premium Telecom experience the CN2 GIA tiers sell.

One caveat comes up repeatedly from people running these boxes: China Mobile's QoS behavior can dent performance depending on your local line. The 30-day refund window exists partly for this reason, so deploy, test from your actual connection, and decide early.

On real throughput, a reviewer who bought both Tokyo Plan versions and ran them side by side reported the v2's 5 Gbps port holding close to 4 Gbps during off-peak Tokyo hours and settling around 2–3 Gbps during Asia evening peak. On v1, users report the nominal 500 GB monthly allowance actually metering out closer to 550 GB. Neither number is a guarantee for your line, but both suggest the specs aren't fictional.

The v2 listing provides 74.82.192.0/24 as a test range. Run a trace from your own connection to it before you order; five minutes of traceroute tells you more than any spec table.

## When The Tokyo Plan is the wrong pick

Skip it in two situations. First, if your audience is in Japan itself, or you need broad Asia coverage without China-optimized routing: BandwagonHost's Osaka line on Softbank routes starts at $49.99/month or $499.99/year, and unlike the Tokyo plans it supports free migration between datacenters through KiwiVM. That flexibility alone can be worth the price difference if your requirements might change.

Second, if The Tokyo Plan is out of stock when you're reading this. Flash stock means waiting for a restock with no queue and no ETA. The practical fallback within the same brand is the general CN2 GIA line: the cheapest tier runs $49.99/quarter or $169.99/year for 2 cores, 1 GB RAM, 20 GB SSD, and 1 TB of traffic at 2.5 Gbps. It defaults to Los Angeles DC6/DC9 or Japan SoftBank, and after purchase you can migrate it across 14 regions including Hong Kong, Australia, Canada, and the Netherlands. Less Tokyo-specific, considerably more flexible.

👉 [Browse the full plan list if The Tokyo Plan is sold out](https://bwh81.net/aff.php?aff=77528)

## FAQ: quick answers before you order

### Can I pay monthly for The Tokyo Plan?

No. Both versions are annual-only. The CN2 GIA tiers are the ones with a monthly option, starting at $89.99/month for the 2 GB starter.

### Can I migrate The Tokyo Plan to another datacenter later?

No. Both versions are locked to DC39v2, and the Tokyo CN2 GIA tiers are locked to JPTYO_8. Only the general CN2 GIA and Osaka lines support migration.

### What do you get besides the raw specs?

Every Tokyo plan runs on KVM with the KiwiVM panel, supports CentOS, Debian, Ubuntu, Rocky Linux, and AlmaLinux, includes a fast ISO mount mode, free snapshots, and free automatic backups. You get one dedicated IPv4 plus a /64 IPv6 subnet, instant rDNS edits from the panel, and a 99.9% uptime guarantee.

### Is the 5 Gbps port on v2 real?

Off-peak, close to it. The side-by-side review measured around 4 Gbps during quiet Tokyo hours, dropping to 2–3 Gbps at Asia evening peak. Keep the 45% sustained CPU cap in mind when you plan what the box will actually carry.

### Does the coupon work on the CN2 GIA tiers?

Yes. The listed CN2 GIA prices are original prices, and BWHCGLUKKB applies its 6.77% discount at checkout on those plans as well.

## Picking in ten seconds

Budget under $100 a year for a general-purpose Japan VPS with real bandwidth: The Tokyo Plan v2. Absolute cheapest entry for a single lightweight job: v1. Telecom-heavy audience, or you need 4 cores and up: Tokyo CN2 GIA. Pure Japan-domestic traffic: the Osaka Softbank line instead. Before you click order, confirm the version you want is actually in stock, and have BWHCGLUKKB ready to paste at checkout, since the discount doesn't apply itself.

👉 [Grab The Tokyo Plan v2 before this batch clears](https://bwh81.net/aff.php?aff=77528&pid=163)
