# 🌙 NOCTIS (Anti-Google Search)

> **Searching the shadows of the web. Finding insights in raw, unformatted, and non-SEO data.**

**Noctis** is a specialized search engine built to navigate the "blind spots" of modern search algorithms. While mainstream engines prioritize ad-revenue and SEO authority, Noctis focuses on information density, raw technical data, and human-to-human communication found in forums, pastes, and logs.

---

## 🎯 The Philosophy
Most of the web's truly raw data is "dirty"—it’s buried in nested forum threads, obfuscated by anti-bot shields, or hidden in ephemeral paste-sites. **Noctis** treats "noise" as a signal, indexing the parts of the internet that Google purposefully ignores.

## 🔥 Key Capabilities

* **Noise-to-Signal Pipeline:** Advanced normalization that strips away the "web clutter" (navbars, ads, trackers) to extract the core intellectual value.
* **Anti-SEO Ranking:** A custom algorithm that rewards unique data, information density, and technical artifacts rather than domain popularity.
* **OSINT Pattern Recognition:** Automatically identifies and tags:
    * Infrastructure: IPs, Onion links, Subdomains.
    * Security: Leaked API signatures, Hash types, Config snippets.
* **Deep Crawl Logic:** Built-in handlers for infinite scrolls, paginated forums, and JavaScript-heavy dumps.

## 🏗 Engineering Stack

* **Core:** Python 3.11 (Asyncio)
* **Discovery:** Playwright & Stealth-HTTPX
* **Brains:** spaCy for NLP & FastText for language/slang normalization
* **Storage:** * **Elasticsearch/OpenSearch:** For sub-second full-text and fuzzy search.
    * **PostgreSQL:** For structured metadata and thread-relationship mapping.
    * **Redis:** High-speed queue for the distributed crawler.

---

## ⚙️ Project Structure

```text
noctis/
├── api/              # FastAPI main, static for html/css/js/favicon
├── crawler/          # Async spiders & Proxy rotators
├── db/               # Database
├── dumps/            # Local JSON dumps
├── elasticsearch     # Elasticsearch bat shortcut
├── search/           # Elasticsearch mapping & CQS scoring
├── normalizer/       # Text normalizer
├── requirements.txt  # Requirements pip
└── noctis.db         # Minimalist Search Interface (Dark Mode by default)
```

## 📊 Content Quality Score (CQS)

Noctis uses a proprietary ranking formula:

<img width="451" height="74" alt="image" src="https://github.com/user-attachments/assets/90280566-478b-44ec-a3e5-37c7d1c8384d" />

This ensures that a 20-page forum thread with high-quality technical discussion ranks higher than a 500-word SEO-optimized blog post.

## 🛡 Ethical Use & Disclaimer
Noctis is an engineering tool for OSINT, security auditing, and data science. It is designed to be a "polite" crawler, respecting `robots.txt` where possible and implementing smart delays to avoid server stress.

P.S: I will not be posting this tool online for free. Later in the future when its ready yall can buy it :>
