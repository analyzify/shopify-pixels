# shopify-pixels

> **Status: Archived on 2026-11-25**. Open-source GA4 custom pixel code and guide for Shopify Customer Events (Shopify Pixels), published by Analyzify in 2022.

## What it is

A single JavaScript file (`ga4/index.js`) to paste into Shopify Admin > Settings > Customer Events as a custom pixel. It loads gtag.js and sends Google Analytics 4 e-commerce events (page view, product view, collection view, add to cart, begin checkout, add payment info, purchase) from Shopify's Customer Events API. Public companion code for Analyzify's Shopify Pixels guide.

## Why it existed

Shopify launched Customer Events (Shopify Pixels) in October 2022. Analyzify published this open-source code block and a tutorial the same week as free content for Shopify merchants, to show expertise in Shopify + GA4 tracking and bring visitors to analyzify.com. It received a few community pull requests (tracking ID constant, typo fix, double page view fix, collection view event) until December 2022 and was then left as is. Analyzify's own paid tracking moved into the Analyzify Shopify app and its pixel extensions.

## Status

Archived on 2026-11-25 as part of the analyzify GitHub org cleanup. It has not been updated since 2022-12-15 and Shopify's Customer Events API has changed since; the guide page on analyzify.com is the maintained resource. The repo stays read-only for reference.

## Where it ran

| What | Value |
|---|---|
| Domains / URLs | Guide: https://analyzify.app/shopify-pixels (old repo homepage), now redirects to https://analyzify.com/hub/shopify-pixels (serves 200 on 2026-11-25). Video: https://www.youtube.com/watch?v=m2lw2ET9Uf4 |
| Hosting | None. The code runs inside the merchant's Shopify store as a custom pixel (Shopify Customer Events sandbox). |
| DNS zone | None (no domain of its own). |
| Database | None. |
| Storage | None. Images in the old README come from GitHub user-images and cdn.analyzify.app. |
| Deploy | None. Merchants copy-paste the file into Shopify Admin. |

## Tech stack

Plain JavaScript for the Shopify Customer Events (Web Pixels) API, Google gtag.js / GA4.

## History

- First commit: 2022-10-08 ("ga4 script added"); last commit: 2022-12-15 (merge of PR #5); 12 commits (9 without merges).
- Authors: the Analyzify team, plus three outside contributors through pull requests.
- 2022-10-08: repo created, GA4 custom pixel script added; 2022-10-09: README and guide link written.
- 2022-10-17: PR #1 (one place to set the tracking ID) merged.
- 2022-12-02: PR #2 (typo in function name) merged; issue #3 (page views counted twice) reported.
- 2022-12-05: PR #4 (double view and tracking ID fixes) merged.
- 2022-12-15: PR #5 (collection view event) merged, last change.
- Open at archive time: issue #8 (2025-06-05, duplicate session counts). Closed: issues #3, #6, #7.
- 2026-11-25: archived.

## Related repos

- https://github.com/analyzify/shopify-ga4-kit: the earlier GA4 data layer kit (theme-based, same period).
- https://github.com/analyzify/GTM-Kit: a later (2024-2025) Customer Events pixel that sends events to Google Tag Manager instead of GA4 directly.

## Who to ask

The Analyzify team (via https://analyzify.com).

## Original README

### Shopify Customer Events & Shopify Pixels

Shopify has announced yet another phenomenal feature: Shopify Customer Events also known as Shopify Pixels. Our team at Analyzify has prepared open-source code blocks and tutorials for Shopify merchants to get the best out of this feature. 

![Shopify customer events shopify pixels sectin in admin panel](https://user-images.githubusercontent.com/53745475/194758408-02a49082-e366-4b5e-9dc7-8e68070b65de.jpg)

With this feature, Shopify merchants can: 

- Manage marketing & tracking pixels from one place, 
- Use Shopify's server-side event and Shopify's liquid objects to track events. 

More importantly, 3rd party tracking scripts will no longer be needed. Analyzify team has already prepared an open-source code block for Shopify & Google Analytics 4 integration. 

#### Set up Google Analytics 4 using Shopify Pixels

You can use the GA4 code block in this repo and follow the tutorial on this page: [Shopify Pixels](https://analyzify.app/shopify-pixels) to achieve a Google Analyics 4 tracking including e-commerce events such as:
- Add to cart
- Product View
- Begin checkout
- Add payment info
- Purchase.

Analyzify's open-source solution doesn't only cover the events but also the metrics/dimensions along with them. 


[![Set up GA4 E-commerce Tracking using Shopify Pixels](https://cdn.analyzify.app/img/yt-shopify-pixels-ga4-setup.jpg)](https://www.youtube.com/watch?v=m2lw2ET9Uf4 "Set up GA4 E-commerce Tracking using Shopify Pixels")



#### More resources on Shopify Customer Events

Shopify Customer Events is a recently released featured. We strongly recommend reading Shopify's documentation, changelog and tutorials before you take any action here. Shopify clearly stated that they won't be supporting the pixels that you add on these sections. 

[Shopify Pixels and Customer Events](https://help.shopify.com/en/manual/promoting-marketing/pixels/)

[Pixels Overview](https://help.shopify.com/en/manual/promoting-marketing/pixels/overview)

[Custom Pixels](https://help.shopify.com/en/manual/promoting-marketing/pixels/custom-pixels)

[Youtube: How to add or modify custom pixels in your Shopify Store?](https://www.youtube.com/watch?v=o82QdfHIwt8)


Our updates on this repo will continue! Stay tuned!
