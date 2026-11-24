# Evoxt Osaka: Premium Japan Pricing, Real Latency Numbers, and Which of the 11 Plans You Actually Need

Evoxt lists Osaka under its Premium Network tier, next to Hong Kong. Every plan costs the same as the identical plan in Tokyo, and the monthly transfer allowance is roughly half. Entry is VM-0.5 at $2.99/month with 250 GB of Osaka traffic; the plan most readers end up on is VM-1 at $5.99/month for 1 core, 2 GB RAM, 20 GB storage and 500 GB per month. What follows is the full 11-plan Osaka price list, third-party latency and disk figures for the node, the add-on prices that decide whether you upgrade a plan or buy extra bandwidth, and the cases where Tokyo or Hong Kong is the better buy.

> **Short version:** VM-1 at $5.99/month handles a WordPress site, a small API, a proxy or a game server for a handful of players. Move to VM-2 at $11.99 (2 cores, 4 GB RAM, 30 GB disk, 1,000 GB transfer) if a database runs alongside the app or traffic will pass a few hundred GB a month. Neither plan costs more in Osaka than in Tokyo.
>
> 👉 [Check current Osaka plans and pricing](https://bit.ly/EvoXt)

## Evoxt Osaka plans and prices: all 11 tiers

All prices are USD per month, billed monthly to three years. Every plan includes weekly offsite backups and the same CPU line, "up to 6.0 GHz," which is the only clock figure Evoxt publishes for these VMs.

| Plan | vCPU / RAM | Storage | Osaka transfer | Price | Order |
| --- | --- | --- | --- | --- | --- |
| VM-0.5 | 1 core / 512 MB | 5 GB | 250 GB | $2.99/mo | [Order VM-0.5](https://bit.ly/EvoXt) |
| VM-0.75 | 1 core / 1 GB | 10 GB | 250 GB | $4.99/mo | [Order VM-0.75](https://bit.ly/EvoXt) |
| VM-1 | 1 core / 2 GB | 20 GB | 500 GB | $5.99/mo | [Order VM-1](https://bit.ly/EvoXt) |
| VM-1.5 | 2 cores / 2 GB | 20 GB | 500 GB | $6.95/mo | [Order VM-1.5](https://bit.ly/EvoXt) |
| VM-2 | 2 cores / 4 GB | 30 GB | 1,000 GB | $11.99/mo | [Order VM-2](https://bit.ly/EvoXt) |
| VM-3 | 4 cores / 4 GB | 30 GB | 1,000 GB | $14.99/mo | [Order VM-3](https://bit.ly/EvoXt) |
| VM-4 | 4 cores / 8 GB | 60 GB | 2,000 GB | $23.99/mo | [Order VM-4](https://bit.ly/EvoXt) |
| VM-6 | 8 cores / 8 GB | 60 GB | 2,000 GB | $29.99/mo | [Order VM-6](https://bit.ly/EvoXt) |
| VM-8 | 8 cores / 16 GB | 80 GB | 3,000 GB | $47.99/mo | [Order VM-8](https://bit.ly/EvoXt) |
| VM-12 | 16 cores / 16 GB | 80 GB | 3,000 GB | $60.95/mo | [Order VM-12](https://bit.ly/EvoXt) |
| VM-16 | 16 cores / 32 GB | 100 GB | 5,000 GB | $95.99/mo | [Order VM-16](https://bit.ly/EvoXt) |

The price column is identical to Evoxt's Standard regions (Los Angeles, London, Frankfurt, Tokyo and the rest). Only the transfer column changes: VM-1 gets 1,000 GB in Tokyo and 500 GB in Osaka, VM-2 gets 2,000 GB in Tokyo and 1,000 GB in Osaka, VM-16 gets 10 TB in Tokyo and 5 TB in Osaka. You pay the Osaka premium in bandwidth, not in dollars.

Double-check that column before you order. Several Osaka plan tables circulating on blogs and affiliate pages list 375 GB for VM-0.75, 750 GB for VM-1.5 and 4,000 GB for VM-8, and some leave out VM-3, VM-6 and VM-12 entirely. Evoxt's own pricing page shows 250 GB, 500 GB and 3,000 GB for those three tiers, which is what the table above uses.

Every plan, including the $2.99 one, ships with KVM virtualisation, IPv4 and IPv6, a 1 Gbps port, an enterprise Layer 3 firewall you configure from the panel, rescue mode, VNC console, API access and deployment in around 2.5 minutes. Traffic between your own VMs over private IP is not counted against the transfer allowance. Uptime is guaranteed at 99.99%. The pricing page also lists an optional paid backup plan priced by VM storage size, which sits on top of the weekly backups every plan already includes.

## How fast is the Osaka node?

Evoxt's own description of the location is short: Osaka is "connected to BBIX and JPIX," with primary transit through SoftBank. BBIX is a SoftBank-operated exchange, so the Osaka box has a short path to SoftBank's backbone and from there into Japan and across to China and Korea. Compare that with Tokyo, which the same page describes as connected to "multiple tier 1 ISPs and BBIX."

Published third-party tests on an Osaka VM-2 (2 cores, 4 GB RAM, 30 GB) recorded the following. These figures come from that test, not from Evoxt and not from anything run for this article.

| Destination | Latency | Upload / download |
| --- | --- | --- |
| Local Speedtest node | 7.41 ms | 842 / 822 Mbps |
| Tokyo | 7.96 ms | 820 / 841 Mbps |
| Shanghai | 50 ms | 806 / 690 Mbps |
| Hong Kong | 57 ms | 817 / 637 Mbps |
| Singapore | 85 ms | 759 / 926 Mbps |
| Los Angeles | 110 ms | 732 / 570 Mbps |

Those throughput numbers sit close to a full gigabit in both directions, which matches the 1 Gbps port Evoxt advertises on every tier. For a $12 VM, Osaka to Tokyo at under 8 ms and Osaka to Shanghai at 50 ms covers most of the reason people look at a Japan location in the first place: East Asian users get a fast first byte, and China-adjacent users get a hop that is competitive with Hong Kong without paying Hong Kong prices.

Disk performance from the same test was well above what the price implies: 950 MB/s on the first pass, 2.4 GB/s on the second, 2.6 GB/s on the third, averaging around 2,023 MB/s.

Routing into China depends on the carrier. The same third-party testing reports China Telecom on a 163 plus SoftBank path with short, consistent latency; China Mobile workable but slightly less consistent; China Unicom on a longer route with noticeably higher latency. That single detail decides a lot of purchases, and it gets its own section below.

👉 [Check the VM-2 (2 cores / 4 GB) Osaka price](https://bit.ly/EvoXt)

## The add-on prices that decide which plan you should buy

Evoxt sells individual resources on top of any plan, and the numbers are worth knowing because they are high enough that upgrading is often the cheaper move.

| Add-on | Price |
| --- | --- |
| Extra IPv4 address | $3/month |
| Extra vCore | $3/month |
| Extra 1 GB RAM | $2/month |
| Extra transfer, Premium (Osaka, Hong Kong) | $12/TB |
| Extra transfer, Standard regions | $3/TB |
| Extra transfer, Premium Plus (Malaysia) | $24/TB |

That $12/TB on Osaka is the part to plan around. Run the arithmetic on three common situations:

| Situation | Buy extra transfer | Upgrade instead |
| --- | --- | --- |
| VM-1 (500 GB) needs 1 TB more | $5.99 + $12 = $17.99, still 1 core / 2 GB | VM-3 at $14.99 gives 1,000 GB, 4 cores, 4 GB, 30 GB |
| VM-2 (1,000 GB) needs 1 TB more | $11.99 + $12 = $23.99, still 2 cores / 4 GB | VM-4 at $23.99 gives 2,000 GB, 4 cores, 8 GB, 60 GB |
| VM-12 (3,000 GB) needs 2 TB more | $60.95 + $24 = $84.95, still 16 GB RAM | VM-16 at $95.99 gives 5,000 GB and 32 GB RAM |

In the first two rows the upgrade is cheaper or exactly the same price and adds cores, RAM and disk. Only near the top of the range does buying transfer separately save money. The same logic applies to RAM at $2/GB: adding 2 GB to VM-1 costs $4, bringing it to $9.99 for 1 core and 500 GB, while VM-2 at $11.99 gives you 2 cores, 4 GB, 30 GB and 1,000 GB. Two extra dollars buys a lot more machine.

The practical rule: pick the plan whose included transfer already covers your month, and treat overage as an emergency measure rather than a plan. If you expect sustained traffic above 500 GB, the jump from VM-1 to VM-2 is the cheapest way to buy it.

👉 [See all Evoxt plans and current add-on pricing](https://bit.ly/EvoXt)

## Osaka vs Tokyo vs Hong Kong

Osaka and Tokyo are the same price and never more than about 8 ms apart, so the choice comes down to transfer, routing and who your users are.

|  | Osaka | Tokyo |
| --- | --- | --- |
| Tier | Premium Network | Standard |
| VM-1 monthly transfer | 500 GB | 1,000 GB |
| Peering (official) | BBIX and JPIX, primary transit SoftBank | Multiple Tier 1 ISPs and BBIX |
| Latency to China / Korea (third party) | Slightly better | Good |
| Latency to US West (third party) | About 110 ms | About 105 ms |
| Plan price | Same | Same |

The decision rules that follow from that:

- **Mostly China Telecom or China Mobile users:** Osaka. The 163 plus SoftBank path is short and consistent, and 50 ms to Shanghai is a good number for a $5.99 box.
- **Mostly China Unicom users:** Hong Kong. Unicom takes a longer route into Osaka, and Evoxt's own description of Hong Kong states optimized routing to China over CN2. If you need a CN2 guarantee, Hong Kong is the only location in the lineup that offers it.
- **Mostly European or American visitors:** a Standard region. You get the same CPU and RAM for the same money with double the transfer, and Osaka's advantage disappears once your traffic is not in Asia.
- **Heavy media or file distribution:** Standard regions, or a bigger Osaka plan. At $12/TB, Osaka overage is four times the Standard rate.
- **Japan-only audience with high traffic:** Tokyo. Identical hardware, double the allowance, sub-10 ms to Osaka anyway.
- **Japan plus Korea, Taiwan, the Philippines, or eastern China:** Osaka earns its place here, which is the case it was built for.

## How Evoxt stacks up against Vultr, DigitalOcean and Linode

The comparison most buyers actually make is against the big three, and the honest version is short. Evoxt's published pitch is single-core clock speed: every plan is listed at "up to 6.0 GHz," and the homepage runs a bar chart comparing 6.0 GHz against 2.4, 2.3 and 2.2 GHz with a footnote saying the data was collected in 2020 and may differ later. The chart does not name the providers it measures, so treat it as vendor marketing rather than an independent benchmark. What is verifiable on Evoxt's side is the plan sheet: 2 GB RAM and 20 GB of storage for $5.99, weekly offsite backups included on every tier including the $2.99 one, and one flat monthly price with no bandwidth or CPU burst surcharges.

Vultr, DigitalOcean and Linode (now part of Akamai) sell a broader platform: more regions, managed add-ons, larger contractual SLAs. Their Japan plans are priced differently and change often, so line-by-line price comparison belongs on their own pages rather than in a table here. What you are trading at Evoxt is scale for clock speed and bundled backups at a low monthly rate.

## Things that trip people up

**IPv6 does not always geolocate to Japan.** Third-party testing found that on some Osaka deployments the IPv6 address is announced from a Malaysian range while the IPv4 address is Japanese. Anything that depends on where the IP appears to be, streaming catalogues included, should be judged on IPv4.

**The $2.99 plan is a test box.** 512 MB RAM runs a proxy, a static page, a tunnel or a bot. It does not run a control panel plus WordPress plus MySQL.

**Payment methods.** Evoxt's FAQ lists credit cards, debit cards, PayPal, Bitcoin and USDt on Tron. Reviews sometimes mention other coins; the checkout page is the authoritative list.

**Billing and renewals.** Terms run from monthly to three years, and you can top up account credit that gets applied to future invoices. The pricing page shows one monthly price per plan, with no separate renewal rate listed alongside it.

**Coupon codes.** Evoxt's pricing page and homepage list no promo codes. Aggregator sites publish several, and they contradict each other, so the only figure worth trusting is the total on the checkout page after any code is applied. Confirm the refund terms on that same page before paying.

## FAQ

**Is Osaka more expensive than Tokyo?** No. Plan prices are identical across Standard and Premium Network tiers. The difference is transfer: 500 GB instead of 1,000 GB on VM-1, 1,000 GB instead of 2,000 GB on VM-2.

**Can I upgrade later without rebuilding?** Yes. Evoxt's panel supports scaling a VM up in a few clicks, and you can also add individual resources such as a vCore, RAM or an IPv4 address without changing plans.

**Do I get a Japanese IP?** The IPv4 address geolocates to Japan, which is why streaming and geo-targeted tests are usually run against it. Check the IPv6 caveat above.

**Is Osaka suitable for a proxy or VPN endpoint?** It is one of the more common uses. 50 ms to Shanghai, 57 ms to Hong Kong and a full gigabit port cover it, provided your users are not on China Unicom.

## Which plan to order

Match the plan to the workload rather than to the price you hoped to pay:

- A single small site, a proxy, a tunnel or a test box: **VM-0.5 at $2.99**. Deploy it, run a traceroute to your actual users, and see whether the path holds up.
- WordPress, a small API, a database-backed app, a Minecraft server for a few friends: **VM-1 at $5.99**, or **VM-2 at $11.99** if 500 GB of monthly transfer feels tight.
- Several sites, a busier application, or anything with concurrent users: **VM-4 at $23.99**, which also doubles the transfer to 2,000 GB.
- More than 2 TB of monthly traffic on Premium bandwidth: price the next tier up before you price overage, because $12/TB adds up faster than a plan upgrade does.

Two things to confirm before you pay: that the monthly transfer matches what your site actually pushes, and whether you need a Japanese IPv4 for geo-locked services, which you should test within the first hour of deployment rather than after you have migrated everything.

👉 [Deploy the VM-1 in Osaka](https://bit.ly/EvoXt)
