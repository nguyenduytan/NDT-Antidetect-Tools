<div align="center">

<h1>🕵️ NDT Antidetect Tools</h1>
<p><a href="LICENSE"><img alt="MIT license" src="https://img.shields.io/badge/License-MIT-64748b?style=flat-square"></a> <img alt="Pricing review date" src="https://img.shields.io/badge/Price_review-2026--10--27-2563eb?style=flat-square"></p>


**Anti-detect browsers, fingerprint testing, automation runtimes and bot-detection resources.**

[![Language](https://img.shields.io/badge/language-English-7c3aed?style=for-the-badge)](README.md) [![Tiếng Việt](https://img.shields.io/badge/README-Ti%E1%BA%BFng%20Vi%E1%BB%87t-16a34a?style=for-the-badge)](README.vi.md) [![Direct links](https://img.shields.io/badge/links-direct%20%7C%20no%20affiliate-16a34a?style=for-the-badge)](#methodology)

**[Browsers](#anti-detect-browsers) · [Tests](#detection-and-fingerprint-tests) · [Open source](#open-source-runtimes) · [Limits](#what-an-antidetect-stack-can-and-cannot-do)**

</div>

> [!IMPORTANT]
> Anti-detect does not guarantee anonymity or access. Sites can combine IP reputation, ASN, TLS, browser signals, behavior and account history. Use these tools for authorized QA, privacy research, test isolation and legitimate profile operations.

## Quick picks

| Need | Start with | Why |
|---|---|---|
| Low-cost profiles | [MoreLogin](https://www.morelogin.com/pricing), [DICloak](https://dicloak.com/pricing), [Hidemyacc](https://hidemyacc.com/pricing) | Small free tiers and low entry plans |
| Agencies and teams | [AdsPower](https://www.adspower.com/pricing), [GoLogin](https://gologin.com/pricing/), [Incogniton](https://incogniton.com/pricing/) | APIs, sharing and collaboration |
| Browser kernels | [Multilogin](https://multilogin.com/pricing), [Kameleo](https://kameleo.io/pricing), [Octo Browser](https://octobrowser.net/pricing/) | Mature profile and runtime controls |
| Developer-controlled | [Camoufox](https://github.com/daijro/camoufox), [Hexium Browser](https://github.com/HeadlessXLabs/hexium-browser), [Firefox stealth](https://github.com/feder-cr/firefox-stealth) | Self-hosted and source-visible options |
| Detection diagnosis | [CreepJS](https://abrahamjuliot.github.io/creepjs/), [BrowserLeaks](https://browserleaks.com/), [Fingerprint Playground](https://demo.fingerprint.com/playground) | Browser, network and device signals |

<a id="anti-detect-browsers"></a>
## Anti-detect browsers

| Tool | Public price/free tier | Automation | Practical note |
|---|---:|---|---|
| [MoreLogin](https://www.morelogin.com/pricing) | Free 2 profiles; Pro $9/month or $5.40/month equivalent when billed yearly for 10 profiles | Selenium, Puppeteer, Local API | Low entry cost; validate browser/OS consistency |
| [DICloak](https://dicloak.com/pricing) | Free 5 profiles/15 opens daily; Base $8/month | RPA, API, MCP | Generous small free tier; daily limits matter |
| [Hidemyacc](https://hidemyacc.com/pricing) | Mini $10; Starter $29; Base $49/month; 7-day trial | API/automation | Clear profile tiers; team cost rises quickly |
| [GoLogin](https://gologin.com/pricing/) | Public view from $4.50/month annual; 7-day trial | API/integrations | Cloud profiles and proxy support |
| [AdsPower](https://www.adspower.com/pricing) | Free 2 profiles; 7-day full trial | Local API, RPA, Synchronizer | Strong team workflow; paid price is dynamic |
| [Incogniton](https://incogniton.com/pricing/) | Starter Plus $19.99; Entrepreneur $29.99/month | Selenium, Puppeteer, API | Cookie collector and synchronizer |
| [Multilogin](https://multilogin.com/pricing/) | Free 5 profiles; paid from $11/month monthly entry | API | Cloud and mobile profiles; scales by seats |
| [Kameleo](https://kameleo.io/pricing) | Free 2 concurrent browsers; Startup €59/month | Playwright/Puppeteer | Custom kernels and mobile emulation |
| [Octo Browser](https://octobrowser.net/pricing/) | Lite €10/month for 3 profiles | API | Mature profile/API model; team plans cost more |
| [Dolphin Anty](https://dolphin-anty.com/) | Free access; live pricing | API, synchronizer | Agency and multi-account workflows |
| [NSTBrowser](https://www.nstbrowser.io/en) | Built-in proxy from $0.40/GB | RPA/API | Anti-detect plus proxy and Cloudflare tools |
| [RoxyBrowser](https://roxybrowser.com/) | Trial and profile plans | Automation | Social, ecommerce and SEO use cases |

## Extended browser directory

These entries require further review of pricing, API quotas and maintenance. Historical prices are not current quotes.

| Provider / project | Direct link | What to verify |
|---|---|---|
| Undetectable | [Website](https://undetectable.io/pricing/) | Cloud/local profiles and configuration fees; annual differs from monthly |
| BitBrowser | [Website](https://www.bitbrowser.net/) | Local API, RPA and profile limits |
| VMLogin | [Website](https://www.vmlogin.us/) | Supported OS, team and API |
| Indigo | [Website](https://indigobrowser.com/) | Permissions, migration and profile limits |
| ixBrowser | [Website](https://www.ixbrowser.com/) | Profile creation/launch quotas and automation access |
| GPMLogin | [Website](https://gpmloginapp.com/en) | Per-machine license, updates and API |
| Bablosoft BAS | [Website](https://bablosoft.com/shop/BrowserAutomationStudio) | Automation studio; fingerprint services are separate |
| Ghost Browser | [Website](https://ghostbrowser.com/) | Session isolation does not establish fingerprint resistance |
| DonutBrowser | [Website](https://donutbrowser.com/) | Local profiles, backup and synchronization |
| Wade | [Website](https://wade.is/) | API access by plan |
| Linken Sphere | [Website](https://linkensphere.info/en/) | Engine, license and updates; avoid unverified rumors |
| WhoLogin | [Website](https://whologin.com/) | Free profiles do not imply free automation |
| ADBLogin | [Website](https://adblogin.com/) | Actual limits of the free tier |
| DashNull | [Website](https://dashnull.com/) | Fingerprint controls and VPN integration |
| ShardBrowser | [Source](https://github.com/ProxyShard/ShardBrowser) | Releases, license and platforms |
| CloakBrowser | [Source](https://github.com/CloakHQ/CloakBrowser) | Kernel version and commercial tiers |
| PotaBrowser | [Source](https://github.com/snaberino/pota-browser) | Builds, releases and compatibility |

## Detection and fingerprint tests

### Browser fingerprint

- [CreepJS](https://abrahamjuliot.github.io/creepjs/), [BrowserLeaks](https://browserleaks.com/), [Fingerprint Playground](https://demo.fingerprint.com/playground)
- [Pixelscan](https://pixelscan.net/), [AmIUnique](https://amiunique.org/fingerprint), [Cover Your Tracks](https://coveryourtracks.eff.org/), [BrowserScan](https://www.browserscan.net/en), [SannySoft](https://bot.sannysoft.com/)

CreepJS inspects canvas, WebGL, fonts, audio, DOM, navigator, workers and headless signals. BrowserLeaks covers IP, JavaScript, WebRTC, rendering, DNS and TLS. Fingerprint Playground is a device-intelligence demo.

### Automation and network

- [Rebrowser Bot Detector](https://bot-detector.rebrowser.net/), [Brotector](https://kaliiiiiiiiii.github.io/brotector/), [Incolumitas](https://bot.incolumitas.com/)
- [BrowserLeaks WebRTC](https://browserleaks.com/webrtc), [BrowserLeaks DNS](https://browserleaks.com/dns), [ProxyDetect](https://proxydetect.live/)
- [FingerBank](https://fingerbank.org/), [TLS Client Test](https://tls.peet.ws/), [DNS Leak Test](https://dnsleaktest.com/)

- [Cloudflare challenge demo](https://nowsecure.nl/), [reCAPTCHA v3 score demo](https://recaptcha-demo.appspot.com/recaptcha-v3-request-scores.php), [IPRoyal WebRTC test](https://iproyal.com/webrtc-leak-test/)

## Open-source runtimes

| Project | Runtime | Purpose | Note |
|---|---|---|---|
| [Camoufox](https://github.com/daijro/camoufox) | Firefox/Python | Patched browser for fingerprint experiments | Self-hosted; read license and releases |
| [Hexium Browser](https://github.com/HeadlessXLabs/hexium-browser) | Chromium/Playwright | C++ persona approach | Linux x86_64 alpha; AGPL |
| [Firefox stealth](https://github.com/feder-cr/firefox-stealth) | Firefox | Source-level fingerprint patches | Research-oriented |
| [Apify Fingerprint Suite](https://github.com/apify/fingerprint-suite) | Node.js | Fingerprint generation and automation | Test supported browser versions |
| [Rebrowser patches](https://github.com/rebrowser/rebrowser-patches) | Chromium/Puppeteer/Playwright | Isolated automation | Compatibility changes quickly |
| [NoDriver](https://github.com/ultrafunkamsterdam/nodriver) | Python | Driverless automation | Not a universal stealth layer |
| [Selenium Driverless](https://github.com/kaliiiiiiiiii/Selenium-Driverless) | Python | Driverless Selenium-style control | Validate maintenance |
| [curl-impersonate](https://github.com/lwthiker/curl-impersonate) | CLI/C | TLS/HTTP client profiles | Does not replace browser identity |
| [curl_cffi](https://github.com/yifeikong/curl_cffi) | Python | Browser-like TLS requests | HTTP client only |

- [ZenDriver](https://github.com/stephanlensky/zendriver): Python automation derived from NoDriver; review maintenance.
- [CycleTLS](https://github.com/Danny-Dasilva/CycleTLS): Node/Go TLS client experiments; check current activity.

## Detection vendors and QA resources

| Resource | Role | What to evaluate |
|---|---|---|
| [Fingerprint](https://fingerprint.com/) | Device intelligence | Accuracy and false positives |
| [DataDome](https://datadome.co/) | Bot management | Backend/CDN integration and valid traffic |
| [Kasada](https://www.kasada.io/) | Bot and account intelligence | Protection and UX impact |
| [Browserbase](https://www.browserbase.com/) | Hosted browser sessions | Compute, proxy and replay costs |
| [BrowserStack](https://www.browserstack.com/) | Real browser/device QA | Clean baseline; not an antidetect browser |
| [Playwright](https://playwright.dev/) | Automation baseline | Behavior before adding patches |
| [OpenWPM](https://github.com/openwpm/OpenWPM) | Fingerprinting research | Measurement and reproducibility |
| [FingerprintJS](https://github.com/fingerprintjs/fingerprintjs) | Open-source fingerprinting | Separate OSS library from commercial service |

- [hCaptcha](https://www.hcaptcha.com/): challenge and fraud signals; evaluate friction and accessibility.
- [Cloudflare bot documentation](https://developers.cloudflare.com/bots/): scoring, deployment and logging.
- [got-scraping](https://github.com/apify/got-scraping): HTTP client; does not execute a full browser environment.
- [Puppeteer Extra](https://github.com/berstend/puppeteer-extra): plugin ecosystem; check browser compatibility and releases.

### Interpreting test results

A green demo result does not guarantee acceptance elsewhere. Commercial services may also use server-side data and account history. Ordinary privacy browsers can produce false positives. Keep a clean-browser baseline, compare one change at a time and record versions. Low uniqueness, fewer leaks and fewer automation signals are different measurements.

### Total browser cost

```text
monthly cost = license for the actual billing term + team seats + proxy + compute
             + cloud storage/phone + operating time
```

Included proxy traffic may not cover your workload.

<a id="what-an-antidetect-stack-can-and-cannot-do"></a>
## What an antidetect stack can and cannot do

A real stack has network identity (IP/ASN/DNS/WebRTC), transport identity (TLS/HTTP2), browser identity (client hints, screen, fonts, WebGL, canvas, audio and timezone), runtime integrity (webdriver/hooks/extensions), behavior and account history. Changing only the user-agent is insufficient; changing only the IP is insufficient.

Stored profiles are not the same as concurrent browsers. API rate limits, opens per day and CPU/RAM can become the first limit. Annual prices shown as a monthly equivalent still require an annual payment.

## Evaluation checklist

- Are browser engine, OS, locale, timezone and IP coherent?
- Can profiles be exported, restored and revoked safely?
- Are APIs documented and rate-limited?
- Do independent tests show contradictory signals?
- Can a profile be reproduced after an upgrade?
- Have you measured false positives and real workflow outcomes?

<a id="methodology"></a>
## Notes and contributions

Prices were checked on 2026-10-27 and are not quotes. Provider links are direct and contain no affiliate parameters. Vendor success claims are not independent benchmarks. See [CONTRIBUTING.md](CONTRIBUTING.md).

## Related NDT projects

- [NDT Proxy Scraper](https://github.com/nguyenduytan/NDT-Proxy-Scraper)
- [NDT Proxy Providers List](https://github.com/nguyenduytan/NDT-Proxy-Providers-List)
- [NDT Captcha Solver Services](https://github.com/nguyenduytan/NDT-Captcha-Solver-Services)

> [!WARNING]
> Use these tools for lawful, authorized automation, QA, accessibility, privacy testing and research. Do not use them to take over accounts or bypass access controls.
