---
name: plate-layout
description: Lay out a multiwell plate. Use when someone plans an ELISA, qPCR, cell-based or compound assay on a 6-, 12-, 24-, 48-, 96- or 384-well plate and needs standards, samples, controls and blanks placed in replicate, optionally keeping the edge wells empty.
---

# Plate layouts with Verbex Lab Tools

1. Collect the plate format, the standard curve (number of points and replicates), the sample names and their replicates, controls, blanks, fill direction (by row or column) and whether to leave edge wells empty.
2. Call `plate_map` once with those inputs.
3. Lead with how many wells are used out of the total, and point out the wells left free. The tool's check confirms every group is placed exactly as many times as its replicates.
4. If the layout doesn't fit, say how many wells are short and offer options: fewer replicates, using edge wells, or a larger plate.

Remind the scientist to mark the A1 corner on the plate and check the map before pipetting.
