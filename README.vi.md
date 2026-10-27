<div align="center">

<h1>🕵️ NDT Antidetect Tools</h1>

**Danh bạ trình duyệt antidetect, kiểm tra dấu vân tay, runtime tự động hóa và phát hiện bot.**

[![Pricing research date](https://img.shields.io/badge/Price_review-27%20Oct%202026-7c3aed?style=for-the-badge)](https://github.com/nguyenduytan)
[![Direct links](https://img.shields.io/badge/links-direct%20%7C%20no%20affiliate-16a34a?style=for-the-badge)](#methodology)
[![License](https://img.shields.io/badge/license-MIT-64748b?style=for-the-badge)](LICENSE)

**[Trình duyệt](#anti-detect-browsers) · [Kiểm tra](#detection-and-fingerprint-tests) · [Mã nguồn mở](#open-source-runtimes) · [Khả năng và giới hạn](#what-an-antidetect-stack-can-and-cannot-do)**

<p align="center"><a href="README.md">English</a> · <strong>Tiếng Việt</strong></p>

</div>

> [!IMPORTANT]
> Anti-detect không bảo đảm ẩn danh hay truy cập thành công. Website có thể kết hợp IP, ASN, TLS, browser fingerprint, hành vi và lịch sử account. Dùng cho QA, privacy research, test isolation và vận hành hợp pháp.

<a id="quick-picks"></a>
## Chọn nhanh

| Nhu cầu | Bắt đầu với | Nhận xét |
|---|---|---|
| Giá thấp, ít profile | [MoreLogin](https://www.morelogin.com/pricing), [DICloak](https://dicloak.com/pricing), [Hidemyacc](https://hidemyacc.com/pricing) | Có free tier và gói nhỏ |
| Agency/team | [AdsPower](https://www.adspower.com/pricing), [GoLogin](https://gologin.com/pricing/), [Incogniton](https://incogniton.com/pricing/) | Team, API, profile sharing |
| Browser kernel chuyên biệt | [Multilogin](https://multilogin.com/pricing/), [Kameleo](https://kameleo.io/pricing), [Octo Browser](https://octobrowser.net/pricing/) | Nhiều profile và browser/runtime controls |
| Developer-controlled | [Camoufox](https://github.com/daijro/camoufox), [Hexium Browser](https://github.com/HeadlessXLabs/hexium-browser), [Firefox stealth](https://github.com/feder-cr/firefox-stealth) | Có thể self-host và kiểm tra source |
| Chẩn đoán detection | [CreepJS](https://abrahamjuliot.github.io/creepjs/), [BrowserLeaks](https://browserleaks.com/), [Fingerprint Playground](https://demo.fingerprint.com/playground) | Nhìn thấy signal bị lộ hoặc mâu thuẫn |

<a id="anti-detect-browsers"></a>
## Trình duyệt antidetect

Giá là public starting points được kiểm tra 2026-10-27; dashboard, term và profile count có thể làm thay đổi tổng tiền.

| Tool | Giá / free tier | Automation | Điểm mạnh | Cần kiểm tra |
|---|---:|---|---|---|
| [MoreLogin](https://www.morelogin.com/pricing) | Free 2 profile; Pro $9/tháng; tương đương $5.40/tháng khi trả theo năm, 10 profile | Selenium, Puppeteer, Local API | Entry cost thấp, canvas và team | Browser version, OS coherence, target compatibility |
| [DICloak](https://dicloak.com/pricing) | Free 5 profile/15 lần mở mỗi ngày; Base $8/tháng | RPA, API, MCP | Free tier rộng, nhiều tool phụ trợ | Daily open và team limits |
| [Hidemyacc](https://hidemyacc.com/pricing) | Mini $10, Starter $29, Base $49/tháng; trial 7 ngày | API/automation | Bảng profile rõ, Windows/Linux/Mac | Chi phí team tăng nhanh |
| [GoLogin](https://gologin.com/pricing/) | Giá hiển thị từ $4.50/tháng ở annual view; trial 7 ngày | API/integrations | Cloud profile, proxy, team | Giá đổi theo profile và billing term |
| [AdsPower](https://www.adspower.com/pricing) | Free 2 profile; trial đầy đủ 7 ngày | Local API, RPA, Synchronizer | Multi-account và team tốt | Paid price dynamic |
| [Incogniton](https://incogniton.com/pricing/) | Starter Plus $19.99; Entrepreneur $29.99/tháng | Selenium, Puppeteer, API | Cookie collector, synchronizer | Profile/seat limits |
| [Multilogin](https://multilogin.com/pricing/) | Free 5 profile; paid từ $11/tháng monthly entry | API | Browser và mobile profiles | Tăng giá theo profile/seat |
| [Kameleo](https://kameleo.io/pricing) | Free 2 browser; Startup €59/tháng | Playwright/Puppeteer | Custom kernels, mobile emulation | Tính theo concurrent browser |
| [Octo Browser](https://octobrowser.net/pricing/) | Lite €10/tháng cho 3 profile | API | Profile và API mature | Gói team/API đắt hơn |
| [Dolphin Anty](https://dolphin-anty.com/) | Free access; giá live | API, synchronizer | Agency và multi-account | Xác nhận giá hiện tại |
| [NSTBrowser](https://www.nstbrowser.io/en) | Proxy tích hợp từ $0.40/GB | RPA/API | Anti-detect + proxy + cloudflare tools | Sản phẩm mới, test stability |
| [RoxyBrowser](https://roxybrowser.com/) | Trial và gói profile giá thấp | Automation | Social/ecommerce/SEO | Kiểm tra độc lập fingerprint |

## Danh bạ browser mở rộng

Các tên dưới đây để nghiên cứu thêm; chưa xác minh đầy đủ giá, hạn mức API hoặc tình trạng bảo trì. Không dùng giá lịch sử làm giá hiện tại.

| Provider / project | Link trực tiếp | Điểm cần đối chiếu |
|---|---|---|
| Undetectable | [Website](https://undetectable.io/pricing/) | Cloud/local profile và phí cấu hình; giá năm khác giá tháng |
| BitBrowser | [Website](https://www.bitbrowser.net/) | Local API, RPA và số profile |
| VMLogin | [Website](https://www.vmlogin.us/) | OS hỗ trợ, team và API |
| Indigo | [Website](https://indigobrowser.com/) | Phân quyền, migration và profile limits |
| ixBrowser | [Website](https://www.ixbrowser.com/) | Hạn mức tạo/mở profile và quyền automation |
| GPMLogin | [Website](https://gpmloginapp.com/en) | License theo máy, update và API |
| Bablosoft BAS | [Website](https://bablosoft.com/shop/BrowserAutomationStudio) | Automation studio; fingerprint dịch vụ riêng |
| Ghost Browser | [Website](https://ghostbrowser.com/) | Session isolation không tự chứng minh chống fingerprint |
| DonutBrowser | [Website](https://donutbrowser.com/) | Profile local, backup và đồng bộ |
| Wade | [Website](https://wade.is/) | Quyền API theo gói |
| Linken Sphere | [Website](https://linkensphere.info/en/) | Engine, license và update; không lặp tin đồn chưa kiểm chứng |
| WhoLogin | [Website](https://whologin.com/) | Free profile khác quyền automation |
| ADBLogin | [Website](https://adblogin.com/) | Giới hạn thực của free tier |
| DashNull | [Website](https://dashnull.com/) | Phạm vi chỉnh fingerprint và tích hợp VPN |
| ShardBrowser | [Source](https://github.com/ProxyShard/ShardBrowser) | Release, license và platform |
| CloakBrowser | [Source](https://github.com/CloakHQ/CloakBrowser) | Phiên bản kernel và gói thương mại |
| PotaBrowser | [Source](https://github.com/snaberino/pota-browser) | Build, release và compatibility |

<a id="detection-and-fingerprint-tests"></a>
## Kiểm tra phát hiện và dấu vân tay trình duyệt

### Dấu vân tay trình duyệt

- [CreepJS](https://abrahamjuliot.github.io/creepjs/) — canvas, WebGL, fonts, audio, DOM, navigator, worker và headless signals.
- [BrowserLeaks](https://browserleaks.com/) — IP, JavaScript, WebRTC, canvas, WebGL, fonts, DNS và TLS.
- [Fingerprint Playground](https://demo.fingerprint.com/playground) — device-intelligence demo.
- [Pixelscan](https://pixelscan.net/), [AmIUnique](https://amiunique.org/fingerprint), [Cover Your Tracks](https://coveryourtracks.eff.org/), [BrowserScan](https://www.browserscan.net/en), [SannySoft](https://bot.sannysoft.com/).

### Tự động hóa và hành vi

- [Rebrowser Bot Detector](https://bot-detector.rebrowser.net/)
- [Brotector](https://kaliiiiiiiiii.github.io/brotector/)
- [Incolumitas Bot Classification](https://bot.incolumitas.com/)
- [Cloudflare Turnstile demo](https://nowsecure.nl/)
- [Google reCAPTCHA v3 demo](https://recaptcha-demo.appspot.com/recaptcha-v3-request-scores.php)

### Mạng và kết nối

- [BrowserLeaks WebRTC](https://browserleaks.com/webrtc), [BrowserLeaks DNS](https://browserleaks.com/dns)
- [ProxyDetect](https://proxydetect.live/), [IPRoyal WebRTC](https://iproyal.com/webrtc-leak-test/)
- [FingerBank](https://fingerbank.org/), [TLS Client Test](https://tls.peet.ws/), [DNS Leak Test](https://dnsleaktest.com/)

<a id="open-source-runtimes"></a>
## Runtime mã nguồn mở

| Project | Runtime | Mục đích | Lưu ý |
|---|---|---|---|
| [Camoufox](https://github.com/daijro/camoufox) | Firefox/Python | Browser patched cho fingerprint experiments | Self-host, đọc license/release |
| [Hexium Browser](https://github.com/HeadlessXLabs/hexium-browser) | Chromium/Playwright | C++ persona, không JS injector | Linux x86_64 alpha, AGPL |
| [Firefox stealth](https://github.com/feder-cr/firefox-stealth) | Firefox | Patch canvas/WebGL/fonts/audio/WebRTC/timezone | Research-oriented |
| [Apify Fingerprint Suite](https://github.com/apify/fingerprint-suite) | Node.js | Fingerprint generation và automation | Test theo browser version |
| [Rebrowser patches](https://github.com/rebrowser/rebrowser-patches) | Chromium/Puppeteer/Playwright | Isolated automation | Theo dõi compatibility |
| [NoDriver](https://github.com/ultrafunkamsterdam/nodriver) | Python | Driverless browser | API thay đổi nhanh |
| [ZenDriver](https://github.com/stephanlensky/zendriver) | Python | NoDriver-derived automation | Xem maintenance |
| [Selenium Driverless](https://github.com/kaliiiiiiiiii/Selenium-Driverless) | Python | Driverless Selenium-style | Không phải stealth layer hoàn chỉnh |
| [curl-impersonate](https://github.com/lwthiker/curl-impersonate) | CLI/C | TLS/HTTP client profiles | Không thay thế browser fingerprint |
| [curl_cffi](https://github.com/yifeikong/curl_cffi) | Python | Browser-like TLS requests | Chỉ HTTP client |
| [CycleTLS](https://github.com/Danny-Dasilva/CycleTLS) | Node/Go | TLS client experiments | Kiểm tra activity |

## Dịch vụ phát hiện phía website và tài nguyên bổ sung

| Nguồn | Vai trò | Cách đánh giá |
|---|---|---|
| [Fingerprint](https://fingerprint.com/) | Device intelligence / visitor identification | Accuracy và false-positive trên dữ liệu của bạn |
| [DataDome](https://datadome.co/) | Bot management | Tích hợp backend/CDN và quan sát traffic hợp lệ |
| [Kasada](https://www.kasada.io/) | Bot defense / account intelligence | Hiệu quả bảo vệ và ảnh hưởng UX |
| [hCaptcha](https://www.hcaptcha.com/) | Challenge / fraud signals | Friction và accessibility |
| [Cloudflare docs](https://developers.cloudflare.com/bots/) | Bot management | Hiểu score, deployment và logging |
| [Browserbase](https://www.browserbase.com/) | Hosted browser sessions | Compute, proxy và replay; không phải browser desktop |
| [BrowserStack](https://www.browserstack.com/) | Cross-browser/device QA | Baseline trên browser/device thật; không phải antidetect |
| [Playwright](https://playwright.dev/) | Automation và test isolation | Baseline trước khi thêm patch |
| [OpenWPM](https://github.com/openwpm/OpenWPM) | Đo tracking/fingerprinting | Dùng cho nghiên cứu đo lường |
| [FingerprintJS](https://github.com/fingerprintjs/fingerprintjs) | Fingerprint library | OSS khác sản phẩm thương mại |
| [got-scraping](https://github.com/apify/got-scraping) | HTTP client | Không thực thi toàn bộ browser JS |
| [Puppeteer Extra](https://github.com/berstend/puppeteer-extra) | Plugin ecosystem | Kiểm tra release và browser compatibility |

### Đọc kết quả test đúng cách

Một điểm xanh ở demo không chứng minh mọi website sẽ chấp nhận. CreepJS kiểm tra tính nhất quán của signal; một dịch vụ thương mại còn có lịch sử account và dữ liệu phía server. Browser privacy thông thường cũng có thể tạo false positive. Lưu baseline browser sạch, so trước/sau từng thay đổi và ghi phiên bản test. Không coi tính độc nhất thấp, ít leak và ít dấu hiệu automation là cùng một chỉ số.

### Chi phí thực của browser

```text
chi phí tháng = license theo đúng kỳ hạn + team seats + proxy + compute
             + cloud storage/phone + thời gian vận hành
```

Số profile lưu trữ không bằng số browser chạy đồng thời. API rate limit, số lần mở/ngày và RAM/CPU có thể giới hạn trước khi hết profile. Gói năm hiển thị giá tương đương/tháng vẫn phải trả theo kỳ năm; proxy kèm theo không mặc định đủ traffic.

<a id="what-an-antidetect-stack-can-and-cannot-do"></a>
## Khả năng và giới hạn của bộ công cụ antidetect

Một stack thực tế gồm: **network identity** (IP/ASN/DNS/WebRTC), **transport identity** (TLS/HTTP2), **browser identity** (UA/client hints/screen/fonts/WebGL/canvas/audio/timezone), **runtime integrity** (webdriver/hooks/extensions), **behavior** (typing, pointer, focus, dwell) và **account history** (cookies, device graph, login). Browser chỉ đổi user-agent là chưa đủ; proxy chỉ đổi IP cũng chưa đủ.

<a id="evaluation-checklist"></a>
## Danh sách tiêu chí đánh giá

- Browser engine có cập nhật và đồng bộ với OS/locale/timezone/IP không?
- Có export/import profile an toàn, revoke team access và local API rõ ràng không?
- Fingerprint test có tín hiệu mâu thuẫn không?
- Profile có tái tạo được sau upgrade không?
- Proxy credentials có được bảo vệ không?
- Đã test workflow thật với p50/p95, false positive và account history chưa?

<a id="methodology"></a>
## Lưu ý khi sử dụng

Giá là snapshot ngày 27/10/2026, có thể thay đổi theo kỳ hạn, cấu hình và khuyến mại. Chưa benchmark toàn bộ dịch vụ; các mục chưa xác minh được đánh dấu riêng. Link provider là link trực tiếp, không affiliate. Xem [hướng dẫn đóng góp](CONTRIBUTING.md).

<a id="related-ndt-lists"></a>
## Dự án NDT liên quan

- [NDT Proxy Scraper](https://github.com/nguyenduytan/NDT-Proxy-Scraper)

- [NDT Proxy Providers List](https://github.com/nguyenduytan/NDT-Proxy-Providers-List)
- [NDT Captcha Solver Services](https://github.com/nguyenduytan/NDT-Captcha-Solver-Services)

> [!WARNING]
> Chỉ dùng cho automation được ủy quyền, QA, accessibility, privacy testing và nghiên cứu. Không dùng để chiếm account, gian lận hoặc vượt access control.
