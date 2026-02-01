# 🛡️ Discerning Shield v5.0

**A lightweight, privacy-focused security terminal for auditing Agent Skills and Markdown data.**

Discerning Shield is a static, client-side utility designed to provide a "first-look" security audit of text files, robotic datasets, and agentic workflows. Built with an Apple-inspired aesthetic, it operates entirely within your browser to ensure your sensitive data never leaves your local environment.

---

## ⚠️ CRITICAL DISCLAIMER & LIMITATION OF LIABILITY

**Prompt Injection is an inherently unsolvable problem.** Because Large Language Models (LLMs) process instructions and data within the same context window, there is no mathematical guarantee that any scanner can catch 100% of malicious attempts.

- **NO GUARANTEE:** This tool is a simple heuristic scanner. It is designed to identify *known* patterns and basic exfiltration techniques. It **cannot** and **will not** catch sophisticated, novel, or deeply obfuscated injections.
- **USER RESPONSIBILITY:** You are solely responsible for the files you upload to your agents. You must independently review every file before deployment.
- **NO LIABILITY:** The creators and contributors of Discerning Shield are **not liable** for any damages, data leaks, financial losses (including Bitcoin/Nostr asset theft), or agent malfunctions resulting from the use or failure of this software.
- **USE AT YOUR OWN RISK:** This software is provided "as-is" without warranty of any kind.

---

## 🚀 Features

- **Proximity Analysis:** Detects malicious verbs (share, reveal, output) in close proximity to sensitive nouns (nsec, xprv, api_key).
- **Entropy Detection:** Identifies high-randomness strings that may indicate hidden private keys or encoded payloads.
- **Anti-Smuggling Normalization:** Flattens Unicode homoglyphs and invisible characters used to bypass standard filters.
- **Privacy First:** 100% Static HTML/JS. No tracking, no backend, and no data collection.
- **Sikorski Logic UI:** High-contrast Dark/Light mode terminal with a "Perfect Parallel" aesthetic.

---

## 🛠️ How to Use

1. **Deploy:** Host the `index.html` file on GitHub Pages or run it locally on your machine.
2. **Input:** Paste your Markdown content or drag-and-drop a `.md` or `.txt` file into the terminal.
3. **Analyze:** Click **"Analyze Content"**.
4. **Interpret:**
   - ✅ **Scan Clean:** No common signatures found (Still requires manual review!).
   - 🚨 **Risk Detected:** Specific patterns identified. Investigate the highlighted lines immediately.

---

## 🛡️ Best Practices for Agent Stewardship

To best protect yourself and your assets:
1. **Manual Audit:** Never trust an automated tool as your only line of defense.
2. **Key Isolation:** Never include `nsec` or `xprv` keys in files accessible to an LLM.
3. **Sandboxing:** Run your agents with the minimum necessary permissions.

---

## 📜 License

This project is open-source. Be a good steward of the code.