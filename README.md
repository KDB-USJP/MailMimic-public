# MailMimic — Fictional Email World Studio

<div align="center">
  <img src="ui/mailmimic.svg" width="100" height="100" alt="MailMimic Logo" />
  <h3>Local-first developer studio for synthesizing rich, realistic, coherent fictional inboxes.</h3>
  <p><strong>Zero Cloud • Zero Telemetry • 100% Deterministic & Seeded • No Real Customer Data</strong></p>
</div>

---

## 🧭 What is MailMimic?

**MailMimic** is a privacy-respecting developer tool and desktop app that synthesizes believable fake inboxes, employee rosters, and email ecosystems without using, scraping, or exposing real customer data.

Developers, sales engineers, QA testers, and security researchers constantly face a frustrating dilemma:
- **Using real customer/employee mailboxes** exposes confidential communications, personal phone numbers, and private credentials.
- **Handcrafted fixtures** produce dry, repetitive single-message files that fail to stress-test MIME parsers, threading logic, attachment downloaders, or consent workflows.

MailMimic generates coherent fictional worlds: real companies, full employee org charts, multi-turn threaded conversations, transactional receipts, newsletters, marketing clutter, and safe simulated attachments.

---

## ✨ Features

- **100% Deterministic & Seeded**: The same scenario preset and seed recreate the exact identical people, timestamps, headers, and conversation flows for repeatable QA runs and regression testing.
- **Realistic Threading & MIME**: Generates compliant RFC 5322 MIME messages with stable `Message-ID`, `In-Reply-To`, and `References` headers.
- **Safe Fake Attachments**: Simulates 1–4 realistic attachments (PDF, PNG, CSV, ICS, XLSX, DOCX) safely generated in-memory without malware or payload risk.
- **Multi-Format Exports**:
  - `.eml` individual RFC 5322 email files
  - `.mbox` standard mail archive files
  - `Maildir/` directory structures (`cur/`, `new/`, `tmp/`)
  - `Contacts` in standard CSV and vCard (`.vcf`)
  - `Mailboat` unencrypted ship-deck bundles (`.mailboat`)
  - `manifest.json` structured world export
- **Custom Templates**: Add your own custom scenarios, templates, or translations via `user-templates.json`.
- **Local-First & Offline**: Operates completely offline with zero network calls, no telemetry, no tracking, and no external AI API requirements.

---

## 🖥️ Supported Platforms

- **Windows**: Standard installer (`.exe` setup) and portable single-file executable.
- **Linux**: Universal `.AppImage` (runs on Ubuntu, Fedora, Arch, Debian, Mint) and `.deb` package.
- **macOS**: Universal DMG (Apple Silicon M1/M2/M3/M4 & Intel).
- **CLI**: Cross-platform Node.js command line tool (`mailmimic` / `email-maker`).

---

## 🚀 Quickstart

### Desktop Application
1. Download the release package for your operating system from the **Releases** tab.
2. Launch MailMimic.
3. Select a scenario preset (e.g. *Series A SaaS*, *Cybersecurity Research*, *E-Commerce Customer*).
4. Enter a seed (or click the dice to randomize) and target message count.
5. Click **Generate World** to synthesize the mailbox.
6. Review messages and personas in the viewer panes.
7. Choose your desired export formats and click **Export All Artifacts**.

### Command Line Interface (CLI)
```bash
# Generate a scenario directly from the terminal
mailmimic generate --scenario startup-team --seed 42 --count 50 --output ./demo-inbox
```

---

## 💼 Licensing & Donationware

MailMimic is distributed under a donationware model:
- **Free for Personal, Educational & Hobby Use**: Completely free for personal projects, student coursework, open-source testing, and non-commercial development.
- **Commercial Use**: A perpetual **$10 commercial license** is available on [Gumroad](https://trigram.gumroad.com/l/mailmimic) for business, corporate, and enterprise use.

---

## 🏛️ Project & Authors

Conceived and crafted by **Trigram** ([trigr.am](https://trigr.am)).  
Designed and built with modern local-first principles.
