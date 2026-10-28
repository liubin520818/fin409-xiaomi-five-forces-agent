# FIN409 Xiaomi automotive Five Forces agent

A working local research application for mainland China's new battery-electric passenger-car market. Xiaomi Corporation is the listed parent; Tesla and XPeng are the principal automotive comparators.

## Download the complete implemented source

**[Download the complete source archive](fin409-xiaomi-agent-source.zip)**, then extract it and enter the `fin409-xiaomi-agent` folder. The archive preserves all 32 source/configuration/evidence/evaluation files with their tested directory structure. Downloading GitHub's outer ZIP or cloning this repository still requires extracting this inner source archive before running npm.

This repository uses a source archive because the connected GitHub integration could read this new repository but refused Git tree writes; publication was completed through the signed-in browser's file upload. The archive is ordinary source code, not a binary executable. Its contents and individual SHA-256 values are listed in [SOURCE_MANIFEST.json](SOURCE_MANIFEST.json).

Archive SHA-256: `9489aba3241020d1b5c7d658e6af11bff854efcc77781157df7c902ab5c150d5`

## Start the local application

Requirements: **Node.js 24**, npm and an installed [Codex CLI](https://developers.openai.com/codex/cli/) with the user's own supported ChatGPT login and available usage. In the **extracted source folder**:

```sh
npm ci
npm test
npm run typecheck
npm start
```

Open **http://127.0.0.1:3037**. The app starts eve locally on port3038. Keep the terminal open; Ctrl+C stops it. The source archive's README includes CLI questions and troubleshooting. No account credentials are included.

This is the public **source repository**, not a continuously hosted public chatbot. Source and evidence can be inspected without login; fresh model calls require the reader's own authenticated local setup.

## Exact prompt, tools and actual tests

- [Actual application instructions](AGENT_SYSTEM_PROMPT.md), version `fin409-v1.1.0`. eve/provider runtime envelopes may also apply; undisclosed provider instructions are not claimed to be reproduced.
- [Four enabled tools and their purposes](TOOL_INVENTORY.md).
- [Observed real-model evaluation](EVALUATION.md) and [structured run identities/hashes](EVALUATION_RESULTS.json).
- Actual runtime model observed: `codex/gpt-6-luna-fast`; eve0.85.0; production corpus `2026-10-28-v3`, **28 source-checked summary cards**.
- Five bounded verification scenarios met their objectives. T6 actually generated a seven-section report and computed historical BEV shares, but required editorial corrections to source attribution and the revenue-peer map. The authoring assistant applied those corrections to the private revised coursework draft; student review remains pending.
- Eleven deterministic tests, TypeScript checking and a fresh-source dependency installation passed. These are separate from model accuracy checks.

## Evidence boundaries

The application searches curated summaries and reads their original-source locations; it does not browse live websites or embed whole PDFs. Group, vehicle and mixed EV/AI financial measures remain distinct. September2025 BEV shares are historical author calculations with portfolio-based reclassification and a rounded denominator; the September2026 BEV numerator gap remains unresolved. The explicitly synthetic T5 injection fixture is separated from production data and proves only its observed test case.

Selected actual answers and tool traces are inside `examples/` in the source archive. The complete T6 report-generation output and edited coursework report remain in the private local delivery package. This repository does not contain the student's course PDFs, signed declaration, video, Turnitin result or submission receipt. GitHub and Google Drive are development/research connectors, not enabled runtime plugins.
