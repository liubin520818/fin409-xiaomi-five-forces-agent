# Local-agent verification — 6 November 2026

This refresh publishes the existing working source in a new dated archive while retaining the original October source ZIP and evaluation history. It does not migrate the application to Coze or host a public model endpoint.

## Observed checks

- 11 deterministic tests passed, zero failed; TypeScript checking passed.
- One new real-model question was submitted through Chrome at `http://127.0.0.1:3037/`; the completed response and two original-source links were visibly read back.
- Run: `2aea82d0-928c-4da8-b232-9f9111941b58`, 6 November 2026, 19:02:58–19:03:16 China time (about 18.4 seconds).
- Actual runtime model: `codex/gpt-6-luna-fast`; eve `0.85.0`; application prompt `fin409-v1.1.0`; corpus `2026-10-28-v3`; test mode disabled.
- Five tool calls completed: `search_evidence`, `list_sources`, `read_evidence` for September 2025, `calculate_share`, and `read_evidence` for September 2026.
- Calculation returned `ok: true`: 41,948 / 826,000 × 100 = 5.07845%; the answer explicitly reported approximately **5.1%** and the rounded denominator.
- The response stated that one month's share cannot establish overall rivalry or industry concentration. It rejected replacing the September 2025 BEV denominator with a September 2026 NEV denominator on period and powertrain grounds. That incompatible ratio was explained, not separately passed to the calculator in this run; deterministic mismatch tests and the older T2 live run provide separate evidence.

The sanitized question, answer and actual tool trace are in [T7](fin409-xiaomi-agent-2026-11-06.zip); hashes and check results are in [the verification record](VERIFICATION_2026-11-06.json). These records contain no model login credentials, hidden reasoning, private student cover or final coursework report.

## Scope of the evidence

The application instructions and runtime logic were preserved; this test did not regenerate the full report. The report's later editorial supplements are separate from the frozen 28-card Agent collection. The check is not a new live verification of financial sources or a guarantee that all future LLM answers will be correct. A student-owned, new local-Agent demonstration video remains pending.

GitHub contains inspectable and reproducible source. Fresh execution still requires Node.js 24, installed dependencies, Codex CLI, a compatible authenticated model account and available usage. No hosted chat service was deployed by this refresh.

## Download and reproduce

Download [fin409-xiaomi-agent-2026-11-06.zip](fin409-xiaomi-agent-2026-11-06.zip), extract it, and enter `fin409-xiaomi-agent`. Run `npm ci`, `npm test`, `npm run typecheck`, and `npm start` using Node.js 24 and a compatible Codex CLI login. Open http://127.0.0.1:3037/. The archive includes the full source, exact prompt, 28 evidence cards, deterministic tests and sanitized model-run evidence.

Archive SHA-256: `619aeb7a28af6cdb591899c880004907f985655d913317d4826c492d1ce64ed5`.

The integration returned HTTP 403 for tree writes, so publication uses the authenticated GitHub website. The October archive remains unchanged. No personal report, cover, local credential or `.runs` directory is included.
