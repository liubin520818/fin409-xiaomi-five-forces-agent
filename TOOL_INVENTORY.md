# Actual application tool inventory

The tested local agent exposes these four authored tools. They are inside the source archive under agent/tools/; default shell, arbitrary file and live web tools are disabled.

| Tool | Actual purpose |
|---|---|
| search_evidence | Keyword search and force filtering over 28 registered summary cards |
| read_evidence | Read a registered summary with original source URL, reader page and metric definitions |
| list_sources | List registered source-card provenance |
| calculate_share | Calculate registered company sales / market total only after matching period, geography, powertrain, retail basis, unit and metric roles |

All four appear in actual run events across T1–T6. The public source archive contains exact wrappers and selected sanitized run traces, while EVALUATION.md explains the bounded observed results and T6 editorial corrections. GitHub and Google Drive were development/research connectors used by the authoring assistant; they are not runtime plugins of this course agent.
