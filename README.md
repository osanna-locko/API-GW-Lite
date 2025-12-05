# API-GW Lite
>API-GW Lite is a simple, lightweight API gateway actor that forwards HTTP requests to target APIs. It lets you send custom-formatted input and translates it into standard HTTP calls — handling headers, query params, JSON bodies, and proxy support — and returns structured responses. It’s ideal when you want to wrap third-party APIs behind a uniform interface or integrate external services into your Apify workflows.

<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/Bitbash333" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>

<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>API-GW Lite</strong> you've just found your team — Let's Chat. 👆👆
</p>

## Introduction
Instead of building a full backend to call external APIs, API-GW Lite lets you use a minimal configuration to forward requests. You pass “destination” URLs, the HTTP method, optional headers, query parameters, request bodies, and optionally proxy settings. The actor then performs the request (optionally via Apify proxy) and returns the result. It works both on the Apify platform and with local testing.

### Why It’s Useful
- Acts as a universal proxy/HTTP client — great for integration or orchestration tasks.  
- Supports any HTTP method (GET, POST, PUT, DELETE, PATCH, etc.).  
- Allows custom headers, authentication, query params, and JSON payloads.  
- Can forward requests through Apify proxy to bypass blocking or rate limits.  
- Returns structured results so you can easily consume responses in other workflows or automation pipelines.

---
## Features
| Feature | Description |
|---------|-------------|
| Multi-Method HTTP Support | Handles GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD requests. |
| Custom Headers & Auth | Lets you specify custom headers or authentication tokens. |
| Query Params & Body Support | Supports URL query parameters and JSON request bodies. |
| Proxy Integration | Optionally uses Apify proxy for requests to avoid blocking or rate limits. |
| Structured Output | Returns response data and metadata in a consistent JSON format. |
| Error Handling | Gracefully handles HTTP errors and returns meaningful error info. |
| Lightweight Implementation | Minimal dependencies — efficient and easy to run. |

---
## What This Actor Accepts
| Input Field | Description |
|-------------|-------------|
| destination (string, required) | Target API endpoint URL. |
| actionType (string) | HTTP method to use (GET by default). |
| requestSignals (object) | Custom HTTP headers and auth info. |
| queryDetails (object) | URL query parameters. |
| payloadContent (object) | JSON body for POST/PUT/PATCH requests. |
| proxySettings (object) | Optional proxy configuration for the request. |

---

---
## Directory Structure Tree

    api-gw-lite/
    ├── src/
    │   └── main.js
    ├── package.json
    └── README.md

---
## Use Cases
- **Integrators** wrap external APIs behind a single uniform interface for dashboard or workflow usage.  
- **Automation engineers** chain multiple API calls in a pipeline, routing through proxies when needed.  
- **Developers** avoid building custom backends — instead use this actor as a micro-gateway in serverless workflows.  
- **Data engineers** fetch data from public APIs with proxy support and forward results to datasets or other actors.  
- **SaaS platforms** embed external API calls securely without exposing credentials or complexity.  

---
## FAQs

**Can I use it with any HTTP API?**  
Yes — as long as the API is reachable via HTTP/S, API-GW Lite can forward the request with headers, params, and body.

**Does it support proxies?**  
Yes — you can enable Apify proxy or other proxy settings to route requests, useful for avoiding rate limits or regional blocks.

**What format does output come in?**  
The actor returns a JSON object containing status code, headers, and parsed body (if JSON), making it easy to process programmatically.

**Is it suitable for production?**  
Yes — it’s lightweight, flexible, and works both in Apify cloud and local environments, making it a solid choice for micro-service style integration layers.

---
### Performance Benchmarks and Results

**Primary Metric:**  
Handles individual HTTP requests with minimal latency — typically under 200 ms for most standard APIs (excluding network delays).

**Reliability Metric:**  
High success rates when used with stable target APIs and proper proxy settings. Graceful error handling ensures stability.

**Efficiency Metric:**  
Low overhead due to minimal code, making it efficient even when used for many sequential calls or as part of larger pipelines.

**Quality Metric:**  
Structured, consistent outputs with full response metadata, enabling seamless integration into downstream processing or analysis.


---


<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/m-dRE1dj5-k?si=5kZNVlKsGUhg5Xtx" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review3.gif" alt="Review 3" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Exceptional results, clear communication, and flawless delivery. <br>Bitbash nailed it."
      </p>
      <p style="margin:1px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
         </p>
