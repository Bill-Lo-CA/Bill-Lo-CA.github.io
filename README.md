# Bill-Lo-CA.github.io

Personal portfolio for Bill Lo, published through GitHub Pages.

**Live site:** https://bill-lo-ca.github.io/

## Purpose

The site presents four connected areas of work:

- Enterprise software engineering experience
- Applied AI and local-model tooling
- Cybersecurity / SOC investigation practice
- Technical writing and public learning profiles

The portfolio intentionally separates implemented work from planned experiments. Public project claims should link to a repository, article, or public profile whenever possible.

## Featured work

- [ContextBubble](https://github.com/Bill-Lo-CA/contextbubble) — Chromium learning extension with caption-first ingestion, local ASR fallback, reviewed concept generation, and in-page overlays.
- [SummerDay](https://github.com/Bill-Lo-CA/SummerDay) — local-first French lesson pipeline using SvelteKit, FastAPI, Stanza NLP, Ollama, and TTS review/publishing stages.
- [SIEM Incident Response Lab](https://medium.com/@lagane100/building-a-siem-based-incident-response-lab-with-splunk-snort-kali-linux-and-windows-server-720a20f44620) — Splunk, Snort, Kali Linux, and Windows Server lab writeup.
- [Hack The Box public profile](https://app.hackthebox.com/public/users/3095335) — ongoing hands-on security practice.

## Technology

The site is deliberately simple and dependency-free:

- Static HTML
- Plain CSS
- GitHub Pages
- JSON-LD person metadata
- Open Graph / Twitter metadata
- Responsive and reduced-motion styles

## Local preview

From the repository root:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Repository structure

```text
.
├── index.html      # Portfolio content and metadata
├── style.css       # Hacker-inspired responsive theme
├── favicon.svg     # Site icon
├── robots.txt      # Search crawler policy
├── sitemap.xml     # Canonical page listing
└── README.md       # Maintenance notes
```

## Updating the portfolio

When adding or changing a project:

1. Confirm the project status from its public repository or article.
2. Describe the problem, implementation, important decision, and current status.
3. Keep future work in the **Lab Queue** instead of presenting it as completed.
4. Add only technologies that are actually used or verified.
5. Test keyboard focus, mobile layout, and reduced-motion behavior.
6. Verify all external links after publishing.

## Deployment

GitHub Pages serves the repository's `main` branch. Changes normally appear after GitHub finishes the Pages deployment and CDN refresh.
