<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:1e3a8a,100:0ea5e9&height=180&section=header&text=MrVenomWolf&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=35" alt="Anu profile banner" />

[![GitHub](https://img.shields.io/badge/GitHub-MrVenomWolf-181717?style=for-the-badge&logo=github)](https://github.com/MrVenomWolf)
[![Email](https://img.shields.io/badge/Email-Contact-0ea5e9?style=for-the-badge&logo=protonmail&logoColor=white)](mailto:mrvenomwolf@proton.me)
</div>

## About me

I build practical software with **Python, TypeScript, JavaScript, and Java**, focusing on data-intensive applications, market-data experimentation, API integrations, and reliable user-facing systems.

My strongest work combines analytical logic with implementation: collecting and normalizing external data, handling dependency failures, writing testable components, and turning rough ideas into usable applications.

I also dabble in using Linux and cybersecurity puzzles - cryptography, forensics and Web exploitation.

## Featured projects

### [NSE Trade Anomaly Detector](https://github.com/MrVenomWolf/NSE-Trade-Anomaly-Detector)

A Python market-data research prototype for detecting statistically unusual trading-volume behavior across 2,500+ NSE equities. The core engine uses log-normalized Z-scores and an outlier-resistant median/MAD baseline, with a dual-threshold flagging rule to isolate genuine anomalies from noise. Supporting modules handle parallel data retrieval, local caching, CSV alert logging, and visualization.

- A median + Median Absolute Deviation (MAD) baseline, resistant to distortion from prior volume spikes.
- A log-transformed relative volume (RVOL) and Z-score, correcting for volume's log-normal, right-skewed distribution.
- Introduced a dual-threshold flagging rule (Z-score ≥ 2.5σ AND RVOL ≥ 2.0x) to reduce false positives from single-metric heuristics.
- CSV alert logging to record RVOL, Z-score, and modified Z-score instead of a flat delta percentage.
- RVOL/Z-score columns to the results table, and replaced an arbitrary fixed-percentage buy/sell zone with a 14-day Average True Range (ATR) volatility band tied to real price data.
- Dynamically fetches the official master list of all active equities from NSE India archives.

### [Streamdrops.stream](https://streamdrops.stream)

A full-stack TypeScript application that ingests TMDB movie/TV data and normalizes inconsistent, loosely-typed external API responses into a stable, strongly-typed data model shared end-to-end via tRPC.

- Implemented resilient API handling with server-side credential protection, request timeouts, bounded retries, rate-limit detection, and short-lived in-memory caching with a stale-cache fallback so the app degrades gracefully instead of failing when TMDB is slow or unavailable.
- Developed deterministic data-selection logic for trailers and streaming providers — sorting candidate videos by official status, type, language, and recency, and deduplicating providers by priority across multiple availability tiers (stream, rent, buy) — to resolve cases where TMDB returns several valid candidates for the same title.
- Used tRPC for end-to-end type safety, with a single shared `AppRouter` type consumed directly by the React client so API contracts can't silently drift between server and frontend.
- Built automated unit and component-level tests with Vitest and Testing Library, covering normalization logic, fallback behavior, and provider-ordering edge cases.
- Served 1,000+ active users in production.

### [Gemini API Chatbot / GemOS](https://github.com/MrVenomWolf/Gemini-API-chatbot-GemOS)

A Python desktop chatbot built with Tkinter and the Gemini API. It includes a themed chat interface, local file attachments, language-aware file handling, content truncation, background request processing, and formatted code responses with copy controls.

## Technology stack

<div align="center">

<img src="https://skillicons.dev/icons?i=python,typescript,javascript,java,react,nodejs,tailwind,mysql,git,github,linux,vite" alt="Technology icons" />

<br /><br />

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=111827)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)

</div>

## Engineering highlights

| Area | Demonstrated work |
| --- | --- |
| Market-data logic | Log-normalized Z-scores, median/MAD baselines, dual-threshold anomaly isolation, and historical rolling-window handling. |
| Data integration | TMDB and market-data APIs, response normalization, external regulatory-data exploration, and server-side credential handling. |
| Reliability | Timeouts, bounded retries, caching, stale-cache behavior, safe error messages, and local fallback behavior. |
| Concurrency | Parallel market-data retrieval with Python's `ThreadPoolExecutor` and background API requests in the desktop application. |
| Testing | Vitest, Testing Library, JSDOM, TypeScript checking, and behavior-focused tests for data transformations and UI flows. |

## Contact

- Email: [mrvenomwolf@proton.me](mailto:mrvenomwolf@proton.me)
- GitHub: [@MrVenomWolf](https://github.com/MrVenomWolf)

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0ea5e9,50:1e3a8a,100:0f172a&height=100&section=footer" alt="Profile footer banner" />

</div>