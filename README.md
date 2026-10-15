# Verbex Lab Tools

Wet-lab calculations and lab documentation for AI assistants: Claude, Cursor, Grok Build and any MCP client.

Exact answers to the calculations and paperwork of wet-lab work, right in the chat.

Ask your assistant how much to weigh for a molar solution, how much stock to dilute, or how to plan a serial dilution, a PCR or qPCR master mix, a lipid nanoparticle (LNP) formulation or a 6- to 384-well plate layout. Each result shows the mass or volumes to use with a drawing of the bench step, the formula, and a check that back-calculates the answer, ready to copy into a lab notebook. The numbers come from deterministic code, so the same inputs always give the same answer.

The plugin also finds 16 editable lab documentation templates (Word and Excel, CC BY 4.0) and practical guides on SOPs, lab notebooks, inventory and data integrity, builds protocol and lab notebook entry templates, and turns reagent label text into a materials table.

## Install

| Client | How |
|---|---|
| Claude Code | Add it as a plugin from this repository (Claude directory listing in review) |
| Cursor | Copy this repository to `~/.cursor/plugins/local/verbex-lab-tools` and reload Cursor (Cursor Marketplace listing in review) |
| Grok Build | Add the MCP server below (xAI plugin marketplace listing in review) |
| Any MCP client | Add `https://www.verbalexperiment.com/mcp` as a remote MCP server (Streamable HTTP, no sign-in) |

The same plugin works in each: `.claude-plugin/`, `.cursor-plugin/` and `.grok-plugin/` hold each client's manifest, `.mcp.json` and `mcp.json` point at the same server, and `skills/` is shared.

## What's inside

- **Connector:** the Verbex Lab Tools MCP server at `https://www.verbalexperiment.com/mcp`. No sign-in.
- **Skills:**
  - `bench-calculations`: solution prep, dilutions, serial dilutions, PCR and qPCR master mixes, LNP formulations
  - `plate-layout`: multiwell plate maps with standards, samples, controls and blanks in replicate
  - `lab-documentation`: templates, guides, protocol and notebook entry drafts, reagent labels

## Try it

- How much NaCl (MW 58.44 g/mol) do I weigh to make 500 mL of 150 mM NaCl?
- Make a qPCR master mix for 30 reactions of 20 µL with 10% excess.
- Lay out a 96-well ELISA plate: 7 standards in duplicate, 12 samples in triplicate, edge wells empty.
- I need a template to track samples in our -80 freezer, including freeze-thaw cycles.

## Privacy

Tool inputs are used only to compute the answer and are not stored. See the [privacy policy](https://www.verbalexperiment.com/privacy) and [terms](https://www.verbalexperiment.com/terms).

Results are calculation and documentation aids, not scientific, safety or regulatory advice; check them against your lab's requirements.

## Support

support@verbalexperiment.com · [verbalexperiment.com/agents](https://www.verbalexperiment.com/agents)

Verbex and Verbal Experiment are products of Multimod Labs LLC.
