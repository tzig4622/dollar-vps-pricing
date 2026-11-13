# $1 VPS: Is the $1 Real, What Specs Do You Get, and Which Plan Should You Pick? (Verified Prices, Renewal Math, IPv4 Caveats)

A $1 VPS almost never bills $1 a month. The plans that come closest are annual deals in the $10–12 per year range, which works out to $0.83–$1.00 a month once you divide the total, plus the occasional first-month promo that renews at the normal rate. JustHost's own entry box is $1.99/month for 512 MB of RAM, and its 1 GB plan lands at $3.88/month on annual billing, which is about the realistic floor for something you intend to keep running.

Below you'll find the full JustHost price list, a formula for turning any headline price into a monthly cost, what 512 MB and 1 GB actually run, and the checks that decide whether a cheap box is usable or just cheap.

## Quick pick: what most readers should buy

> **Most readers:** JustHost **Sirius**, 1 vCPU / 1 GB RAM / 20 GB NVMe / 300 Mbps fair-share port, **$4.85/month, or $3.88/month if you prepay 12 months**. 1 GB is where a control panel plus a small site actually fits, and 20 GB leaves room after the OS.
>
> **Absolute minimum:** **VPS Promo** at **$1.99/month** (1 core / 512 MB / 5 GB NVMe). The catch is the port: 10 Mbps fair-share, which JustHost itself equates to roughly 4 TB a month.
>
> 👉 [Check the current Sirius price and 12-month rate](https://justhost.asia/en/services/vps/tariffs/sirius?ref=196392)

If you'd rather see the whole lineup before picking, the tables are right below.

## JustHost's VPS lineup, in one table

JustHost runs several parallel VPS lines, and the one most people land on is the NVMe series priced per month, with a 20% cut applied when you pay for a year.

| Plan | vCPU / RAM / NVMe | Port (fair-share) | Monthly | 12-month (per month) | Order |
| --- | --- | --- | --- | --- | --- |
| VPS Promo | 1 / 512 MB / 5 GB | 10 Mbps (~4+ TB) | $1.99 | not listed | [ Order](https://justhost.asia/en/services/vps/tariffs/promo-c1r512nvme?ref=196392) |
| New Star | 1 / 1 GB / 10 GB | 100 Mbps (~31+ TB) | $3.81 | $3.05 | [ Order](https://justhost.asia/en/services/vps/tariffs/new-star-c1r1024nvme?ref=196392) |
| Sirius | 1 / 1 GB / 20 GB | 300 Mbps (~93+ TB) | $4.85 | $3.88 | [ Order](https://justhost.asia/en/services/vps/tariffs/sirius?ref=196392) |
| Arcturus | 1 / 2 GB / 30 GB | 300 Mbps (~93+ TB) | $6.92 | $5.53 | [ Order](https://justhost.asia/en/services/vps/tariffs/arcturus?ref=196392) |
| Double Star | 2 / 2 GB / 20 GB | 200 Mbps (~62+ TB) | $7.08 | $5.67 | [ Order](https://justhost.asia/en/services/vps/tariffs/double-star-c2r2048nvme?ref=196392) |
| Alpha Centauri | 2 / 2 GB / 40 GB | 400 Mbps (~124+ TB) | $8.99 | $7.19 | [ Order](https://justhost.asia/en/services/vps/tariffs/alpha_centauri?ref=196392) |
| Bright Star | 4 / 4 GB / 30 GB | 300 Mbps (~93+ TB) | $9.80 | $7.84 | [ Order](https://justhost.asia/en/services/vps/tariffs/bright-star-c4r4096nvme?ref=196392) |
| Vega | 2 / 4 GB / 80 GB | 500 Mbps (~155+ TB) | $13.44 | $10.75 | [ Order](https://justhost.asia/en/services/vps/tariffs/vega?ref=196392) |
| Capella | 4 / 4 GB / 120 GB | 750 Mbps (~232+ TB) | $18.30 | $14.64 | [ Order](https://justhost.asia/en/services/vps/tariffs/capella?ref=196392) |

Read the port column as carefully as the RAM column. Core count and bandwidth don't move together: Double Star gives you two cores and 2 GB for $7.08 but only 200 Mbps, while Sirius gives you one core and 1 GB for $4.85 with 300 Mbps. If you're serving pages, the port is usually the earlier bottleneck; if you're compiling or running containers, it's the core count.

The discount tiers require a minimum term. New Star, Double Star and Bright Star are marked as available when you order three months or more, so the 12-month rate only exists if you commit to a year. A few larger plans (up to 8 cores / 24 GB / 600 GB NVMe) sit above Capella on the same pages.

**The "Special" line.** JustHost's VPS landing page lists a separate set of discounted variants under the same plan names, at lower headline prices than the all-tariffs page:

| Plan | vCPU / RAM / NVMe | Port | Monthly | 12-month (per month) | Order |
| --- | --- | --- | --- | --- | --- |
| Sirius Special | 1 / 1 GB / 20 GB | 300 Mbps | $2.81 | $2.25 | [ Check current price](https://justhost.asia/?ref=196392) |
| Arcturus Special | 1 / 2 GB / 30 GB | 300 Mbps | $4.01 | $3.21 | [ Check current price](https://justhost.asia/?ref=196392) |
| Vega Special | 2 / 4 GB / 80 GB | 500 Mbps | $7.79 | $6.23 | [ Check current price](https://justhost.asia/?ref=196392) |
| Yildun Special | 4 / 8 GB / 200 GB | 750 Mbps | $16.20 | $12.96 | [ Check current price](https://justhost.asia/?ref=196392) |
| Betelgeuse Special | 6 / 12 GB / 400 GB | 750 Mbps | $26.40 | $21.12 | [ Check current price](https://justhost.asia/?ref=196392) |
| Altair Special | 8 / 24 GB / 600 GB | 750 Mbps | $47.40 | $37.92 | [ Check current price](https://justhost.asia/?ref=196392) |

The same plan name appears at two different prices across those pages. Take the number in the cart as final rather than either table.

**IPv4 changes the entry price.** JustHost prices IPv6-only KVM VPS from **$1.60/month**, and its IPv4 + IPv6 line from **$2.60/month** on annual billing. On that IPv4 + IPv6 line you also choose the disk type, and the choice moves the price: 1 core / 512 MB / 5 GB is $3.25 monthly or $2.60 on 12 months with HDD, $3.90 / $3.12 with SSD, $4.22 / $3.38 with NVMe. That gap between $1.60 and $2.60 is the single most consequential detail in this article for anyone on a $1 budget.

## What $1 actually buys: the specs behind the price

Across the low-end market, the $1 tier settles into a narrow band: one or two vCPUs, 256 MB to 1 GB of RAM, 10–30 GB of SSD or NVMe, and 500 GB to 1 TB of monthly transfer. Recent examples that were live when checked:

- **CloudServer:** 1 vCPU, 1 GB RAM, 20 GB SSD RAID, 1 TB transfer, one IPv4, $10.00/year.
- **DediRock:** 1 vCPU, 768 MB RAM, 10 GB SSD, 1 TB transfer, one IPv4, $10.18/year.
- **Server Host:** 1 vCPU, 1 GB RAM, 15 GB storage, unmetered bandwidth, one IPv4, $11.00/year.
- **VPS1Dollar:** 1 Xeon vCPU, 1 GB RAM, 20 GB storage, 100 Mbps unmetered, €1/month, IPv6-only.
- **RackNerd:** 768 MB / 10 GB / 1 TB at $10.28/year, marked out of stock on the listing.

Two things stand out. First, the honest $1/month offers are almost all annual: $10 to $11 a year is $0.83 to $0.92 a month, and that's the real number. Second, the 768 MB configurations come with 10 GB disks, which is tight once a Linux install and a control panel are on it.

## The real monthly cost, in one formula

Take the total amount you pay for the term and divide by the number of months. That's it.

- CloudServer: $10.00 ÷ 12 = **$0.83/month**
- DediRock: $10.18 ÷ 12 = **$0.85/month**
- Server Host: $11.00 ÷ 12 = **$0.92/month**

Run the same math on the monthly-versus-annual gap at JustHost. Sirius costs $4.85 monthly; paying for 12 months brings it to $3.88, a saving of $0.97 a month, or **$11.64 over the year**. New Star drops from $3.81 to $3.05, which is $9.12 a year. Neither is a rounding error at this price level, and both only exist if you prepay.

Two traps to check for before the formula is even useful. A "$1" figure is sometimes the first month only, with the normal rate applied afterwards, and sometimes it needs a specific promo code to appear at all. And the page title is not the price. One host currently runs a landing page headed "1 Dollar VPS" whose cheapest plan card reads **$7.71/month** for 2 GB of RAM, 1 vCPU, 50 GB NVMe and 1 TB of transfer; the site's own note says locations, operating systems, transfer allowances and taxes may differ. The headline and the checkout are two different documents.

👉 [See JustHost's full plan list with the 12-month rates applied](https://justhost.asia/en/services/vps/tariffs-all?ref=196392)

## What a $1 box runs, and what it won't

At 512 MB to 1 GB you can run a basic LAMP or LEMP stack for PHP, a small Node.js service, a minimal database container, or a single small WordPress site with basic plugins and caching. 1 GB is the comfortable side of that line: WooCommerce or a light SaaS app generally wants the full gigabyte, and a panel plus a database plus a site is where 512 MB starts swapping.

The disk matters as much as the RAM. A 5 GB NVMe volume, which is what JustHost's $1.99 plan gives you, holds a minimal Linux install and not much else. Add a control panel and a database and you're managing free space in the first week. If you plan to install anything on top of the OS, treat 20 GB as the practical minimum; that's the Sirius tier at $3.88.

What this class of hardware is not for: heavy computation, large databases, high-traffic sites, or anything where a couple of hours of downtime costs real money. Low-end providers also oversell, meaning several VPS instances share the same physical hardware, and performance drops when neighbours get busy. Support at this price is thin by design.

## Five checks before you pay

**1. Is IPv4 included, or is the price IPv6-only?** This is the one that catches people. JustHost's own pricing shows the difference: IPv6-only from $1.60/month, IPv4 + IPv6 from $2.60/month. A host can also sell you an IPv6-only box and hand you an IPv4 SSH proxy so you can still log in from a normal connection, with a public IPv4 as a paid add-on you attach and move between servers later. That works, but it changes what your site can reach and be reached by, and the IPv4 add-on has its own cost.

👉 [Compare JustHost's IPv4 + IPv6 plans, which start at $2.60/month on annual billing](https://justhost.asia/?ref=196392)

**2. What's the port speed, not just the traffic allowance?** "Unmetered" describes a cap that doesn't exist, not a fast pipe. JustHost's $1.99 plan runs a 10 Mbps fair-share port (roughly 4 TB a month if saturated around the clock); the $3.88 plan runs 300 Mbps. Both are unmetered. Only one of them will pull a Docker image without you noticing.

**3. Are backups automatic?** None of the JustHost plan listings mention automated backups, so assume the server is unmanaged and the backup is your job. Some low-end hosts include a snapshot and a separate FTP backup volume, but that's a feature to verify, not to assume.

**4. What does it cost in month 13?** The 12-month column is a prepay discount, and the monthly column is what you'll pay if you let it roll month to month. Write both numbers down before choosing a term.

**5. What happens when it breaks?** Third-party reviews of JustHost on Trustpilot describe support as slow and scripted, and one reviewer reports a full outage on 2 March 2026 with no status page and no reply for 15 hours; others describe downtime lasting a day or more. Cheap unmanaged hosting means you are the operations team. If you need someone to answer at 3 a.m., budget for a managed host instead.

## How the alternatives stack up

| Provider | Specs | Price | Note |
| --- | --- | --- | --- |
| CloudServer | 1 vCPU / 1 GB / 20 GB SSD / 1 TB | $10.00/yr (~$0.83/mo) | KVM, one IPv4 included |
| DediRock | 1 vCPU / 768 MB / 10 GB SSD / 1 TB | $10.18/yr (~$0.85/mo) | Los Angeles and New York |
| Server Host | 1 vCPU / 1 GB / 15 GB / unmetered | $11.00/yr (~$0.92/mo) | Several US and EU locations |
| RackNerd | 1 vCPU / 768 MB / 10 GB / 1 TB | $10.28/yr | Listed as out of stock |
| VPS1Dollar | 1 vCPU / 1 GB / 20 GB, 100 Mbps unmetered | €1/mo | IPv6-only; public IPv4 is an add-on |
| LightNode | 1 vCPU / 2 GB / 50 GB NVMe / 1 TB | $7.71/mo | Page is titled "1 Dollar VPS" |
| CloudSurph | "VPS For 1 Dollar" product line | not listed in the page section reviewed | States a 5-day full refund and a 99.99% uptime SLA |

Rough read: if the lowest possible annual outlay is the goal, the $10–11/year crowd wins, and CloudServer's 1 GB at $10/year is the strongest of those on paper. If you want a real IPv4 and something you can grow, JustHost's $3.88 Sirius tier costs more per month but gives you 20 GB of NVMe and a 300 Mbps port. If a refund window matters more than the price, CloudSurph's stated 5-day policy is the outlier in this group.

## FAQ

**Is a $1 VPS real?**
Yes, as an annual price of roughly $10–12 per year, which is $0.83–$1.00 a month. As a monthly recurring price with no prepay, it's rare, and where it appears it's often a first-month promotion or requires a code.

**Monthly or annual?**
Nearly always annual if you want the $1 figure. JustHost's own discount of 20% requires a 12-month term on most plans, and some tiers require at least three months.

**Can I run WordPress on a $1 VPS?**
One small site with basic plugins and a caching layer, yes, at 1 GB. At 512 MB with a 5 GB disk you'll fight the box. WooCommerce and multi-site setups want 1 GB plus headroom.

**What if the plan is IPv6-only?**
You can still reach it over SSH through an IPv4 proxy, and you can publish sites over IPv4 via NAT64 or a Cloudflare proxy. If you need a dedicated public IPv4 for mail, game servers or legacy clients, price that add-on before you compare totals.

**How long does setup take?**
It varies by host and isn't published on the JustHost plan pages, so confirm before you plan an evening around it. Some competitors in this bracket advertise deployment in under a minute.

## Which one to pick

- **One test box, throwaway projects:** JustHost VPS Promo at $1.99/month. Accept the 10 Mbps port and 5 GB disk, and don't put anything you'd miss on it.
- **A small site, a panel, or a couple of containers:** Sirius at $3.88/month on 12 months. The 20 GB and 300 Mbps are worth the extra $1.89 over the promo.
- **Multiple services or a small database:** Arcturus at $5.53 (1 core / 2 GB / 30 GB) or Alpha Centauri at $7.19 (2 cores / 2 GB / 40 GB, 400 Mbps).
- **You need a fixed public IPv4:** start from the IPv4 + IPv6 line at $2.60/month rather than paying for an add-on later.

Before you pay, confirm the renewal rate for the term you selected and the refund window that applies to it. Neither is worth discovering after the card is charged.

👉 [Start with the $1.99 VPS Promo plan and upgrade later if you outgrow it](https://justhost.asia/en/services/vps/tariffs/promo-c1r512nvme?ref=196392)
