---
name: lab-documentation
description: Lab documentation for wet-lab work. Use when someone needs a template for an SOP, protocol, experiment plan, lab notebook entry, deviation or troubleshooting log, risk assessment, freezer or chemical inventory, calibration or maintenance log, training record or cell culture records; wants a protocol or notebook entry structured; wants reagent label text turned into a materials table; or asks how to write SOPs, keep lab notebooks, track inventory or meet data-integrity and GLP expectations.
---

# Lab documentation with Verbex Lab Tools

## Templates and guides

1. Call `search` with the scientist's need in plain words, for example "freezer sample inventory" or "deviation log".
2. Call `fetch` on the best result. Templates come back with their full text, a worked example where there is one, and a link to the editable Word or Excel file (licensed CC BY 4.0). Guides come back with a short summary and the full text.
3. Describe what the template contains and give the link to the editable file. For a how-to question, answer from the guide and cite its url.

## Structured documents

- To draft a protocol, call `protocol_template` with the protocol title and, if known, a preset; to draft a lab notebook entry, call `eln_template`. Both return Markdown ready to fill in.
- To turn reagent label text (typed or from OCR) into a materials table, call `parse_reagent_label` with the text. Point out fields flagged for checking against the bottle.

Templates and guides are documentation aids, not regulatory advice; the scientist follows their institution's procedures.
