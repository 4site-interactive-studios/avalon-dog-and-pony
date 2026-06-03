# Avalon Dog and Pony: Demo Plan

We're presenting to people who don't know what we do, so the demo has to do two jobs. Prove we ship real work, and drop a couple of things new enough that the room walks out thinking we're ahead of everyone. The format helps here. An interactive page instead of a slide deck is its own quiet flex.

Thirty minutes to demo, fifteen for Q&A. A tight thirty beats a loose forty-five, so we lock three demos and keep the rest as a bench we pull from based on what Avalon asks for.

Descriptions below now carry the real numbers, demo links, and scope I pulled from the sites, Slack, and Drive.

## The three we lead with

These are locked.

### Cart abandonment (Bryan)
The PETA cart abandonment microservice, and the numbers are the whole pitch. Over a recent run it tracked 28,211 abandonment sessions, sent 2,543 recovery emails, and turned 482 of them into donations. That is a 19% email-to-donation rate (you said you'd expected 3 to 5%), worth $26,174.84 so far, $25,460.39 one-time plus $714.45 monthly, averaging about $4,000 a week. PETA cleared these for our marketing. This is the credibility anchor: real recovered revenue from a name the room knows.
Demo: PETA shopping cart at support.peta.org/page/85309/donate/1?mode=DEMO. Recovery-logs link is a placeholder for now.
Internal Q&A note: PETA owns this specific code, so building it for another client means a fresh build and a conversation, not a copy.

### Stupski GA4 dashboard (Stef)
A custom GA4 and GTM dashboard Stef built for Stupski, more flexible than Looker Studio and not boxed in by a client's messy analytics connection. She updates it monthly today and is moving it toward a nightly automated refresh. Frame it as the report we reach for when Looker can't keep up.
https://4site-interactive-studios.github.io/stupski-control-report/

### Email editor (Bryan and Stef)
The MJML editor Bryan's been building. Named sections, AI on a per-block basis, live MJML validation, theme a whole email from one prompt, convert a screenshot or an existing email into MJML. This is the future-positioning piece. Every agency codes emails in scattered places, and we're building the thing that fixes it. Pitch it as something we could build out for Avalon specifically if they wanted to drive its direction.
Runs locally. The EN Marketing Tools package is its shippable cousin.

## Shipped work we can pull up

Visual, done, defensible. Good for "show us something else" moments and Q&A. SmartChart and CASSI are the two I'd reach for first.

### SmartChart for Spitfire Strategies (Bryan)
smartchart.org is Spitfire's communications-planning tool, and we built it. We did the 2017 rebuild (brand update, backend re-architecture, a fast onboarding flow) and then the current Smart Chart 4.0. It walks nonprofit teams through six steps, program decisions, context, strategic choices, objectives, tactics, and evaluation, to produce a downloadable communications plan, with accounts so a team can build, save, and share multiple plans. Strong proof we build real applications, not just pages.
https://smartchart.org/

### CASSI, the California Strong Start Index (Stef)
Also ours, end to end. The Index measures the conditions babies are born into using 12 indicators from state birth records, so funders and policymakers can direct resources earlier and more fairly. We built the site and the interactive map: filter by census tract with type-ahead search, compare across years, toggle map layers, and pull up embedded data dashboards. This is the data-and-infographic example Stef wanted.
https://strongstartindex.org/map

### Save Tibet scrolling map (Bryan)
A scroll-driven story for the International Campaign for Tibet's "Become an Ally for Tibet" campaign. It moves chapter by chapter through access, environment, religious freedom, and the Dalai Lama's succession, each with full-bleed photography, one big statistic, and a sign-up ask. Pure visual payoff.
https://alliesfortibet.savetibet.org

### Stupski interactive grant map (Stef)
The public side of our Stupski work: an interactive map of the foundation's spend-down giving since 2014, by California county and Hawaiian island, filterable by issue area. Proof we build interactive data elements inside a normal site, not just standalone microsites.
https://stupski.org/about/where-we-work

### PaintCare site locator (Stef)
Custom locator form Tayo built. It's beautiful, and it's a different flavor than donation pages, which is the variety we want in the room. Worth confirming we keep it in.
(Tayo is a contractor, but the work is ours to show)

### Social proof popup (Stef)
The pill lightbox from Shatterproof, an Engaging Networks client and one of Stef's first builds. It gets forgotten, but orgs are still running things like it. A cheap-to-implement example that punches above its size.
https://4site-interactive-studios.github.io/js-social-proof-pop-up/

### DTFA FundraiseUp customization (Sydney)
Work we did with Avalon for one of their own clients, the Dave Thomas Foundation for Adoption: a customized FundraiseUp donation experience, with fresh 2026 opportunities Sydney is scoping right now. A clean "here's what we've already built together" proof point for the Avalon room.
(No live version or before-and-after, so this one runs as a talking point on the call.)

## Fundraising tech and products

### Promotions plugin / Raise More (Bryan)
Our WordPress plugin for on-site promotions. Schedule a sitewide fundraising lightbox for a week, then auto-swap it for a pushdown promoting signups, and tailor the content per landing page, all with no code. Seven promotion types: multistep lightbox, raw code, pushdown, floating tab, overlay, signup, and roll up. The multistep lightbox embeds an Engaging Networks donation page directly. The angle Stef wants: it isn't only for donations. Show foundations using it for signups and campaign promos.
https://www.4sitestudios.com/products/4site-promotions-plugin/
WordPress: https://github.com/4site-interactive-studios/4site-wordpress-promotions
Drupal: https://github.com/4site-interactive-studios/4site-drupal-promotions

### Remember Me (Stef)
Our cross-domain autofill cookie. A small static file on the main domain sets one cookie that any of an org's Engaging Networks pages can read, so returning supporters are recognized across subdomains and their details pre-fill, cutting friction on donation and advocacy forms. Live for WWF, PETA, and RAN, and Stef is scoping it now for Food & Water Watch.
https://act.ran.org/page/90802/donate/1

### Opt-in ladder (Bryan)
A smart form on thank-you pages that shows only the opt-ins a supporter hasn't taken yet, one at a time, with one-click subscribe. Numbers: NWF added 10,371 opt-ins from October to March, about 1,000 participants a month, each taking roughly two more. RAN runs around a 7.5% conversion, and the people who say yes tend to say yes to about three more. Runs locally.

### TidyContact (Bryan)
Our data-quality product: address standardization, phone standardization, and email validation, with nonprofit pricing that gives everyone the same rate from one check to a million.
https://www.4sitestudios.com/products/4site-tidycontact-email/

### EN Marketing Tools package (Stef)
New, and under ten hours to stand up for a client. Worth a mention as the "you can have this fast" option, and as the contrast that makes the email editor look as far ahead as it is.

## Where this is going (the wow)

The thought-leadership block. Less polished, more direction. Honesty about what's experimental plays well here.

### Hermes (Bryan)
The AI agent running in Slack, on a Raspberry Pi, 24/7. It produces a daily brief from multiple sources and posts it to a channel. You can talk to it, give it feedback, add sources. Frame it two ways: here's what we're experimenting with internally, and here's something we could stand up for Avalon or its clients.
https://public.4sitestudios.com/dailybrief/2026-06-03.html
https://public.4sitestudios.com/dailybrief/2026-05-27.html

### GA4 MCP / Data Studio data agents (Bryan)
A direction, not a finished demo. Connecting a client's platforms and letting AI assemble one holistic report across them. Worth gesturing at. Be straight that for some setups it gets cost-prohibitive fast.
https://docs.cloud.google.com/data-studio/conversational-analytics-data-agents

### UTM builder (Stef)
Most clients track campaigns badly, and the spreadsheet they're stuck with doesn't get used. A friendlier builder that people actually open. Early concept, but it fits the "we build small tools to fix real pain" story.

## Cut or de-prioritized

So we don't reopen these mid-prep.

Server-side analytics. Dropped, per your call. The DTFA discovery work continues on its own track, it just isn't a dog and pony item.

Capacity and time-tracking report. Too niche, and agencies famously don't track their own time. Skip it.

## Presenters and next step

Bench assignments are my first pass, split by who owns each piece. Swap them freely. Sydney is the only name outside you and Stef, on DTFA.

Settled with you:
- DTFA: Fundraise Up customization, no live version or before-and-after, so it runs as a talking point.
- Server-side analytics: dropped.
- PETA recovery logs: placeholder link for now.

Optional: we also built a data infographic for Spitfire with Tayo (the California Community Colleges social-determinants graphic). If you want a second pure-infographic example alongside CASSI, that's a candidate.

The interactive page is built from this: a blue carnival hero, three leads up front, the bench grouped, presenter avatars on each item, and the wow block, all styled from the capabilities deck. It lives in index.html.
