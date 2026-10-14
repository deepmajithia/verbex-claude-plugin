---
name: bench-calculations
description: Exact numbers for wet-lab bench work. Use when someone needs how many grams to weigh for a molar solution or buffer, how much stock to dilute (C1V1), a serial dilution or standard curve, a PCR or qPCR master mix for several wells, or a lipid nanoparticle (LNP) formulation, or asks to check one of these calculations.
---

# Bench calculations with Verbex Lab Tools

Scientists act on these numbers at the bench, so they should come from the Verbex Lab Tools calculators, which are deterministic and check their own arithmetic, rather than from mental math.

## Pick the tool

| The scientist needs | Tool |
| --- | --- |
| Grams to weigh for X mM in Y mL, or a percent solution | `solution_prep` with `mode: "solid"` |
| Volume of stock for a dilution (C1V1 = C2V2) | `solution_prep` with `mode: "stock"` |
| A dilution series across tubes or wells | `serial_dilution` |
| A PCR or qPCR master mix for N reactions with excess | `pcr_master_mix` |
| An LNP formulation from RNA mass, N/P ratio and lipid mol% | `lnp_formulation` |

## Steps

1. Collect the inputs. Ask for anything missing that changes the answer, such as the molecular weight of the exact form being weighed (hydrate or salt), stock concentrations, or lipid molecular weights from the certificates of analysis. Don't guess them.
2. Call the tool once with all inputs and units (uL for µL, uM for µM).
3. Lead with the number to use, exactly as the tool returns it, with units and the same significant figures. If a Verbex card is shown, it already holds the table, drawing and check line, so keep the reply short.
4. Pass on the tool's check line, warnings and safety notes. Describe the result as checked by Verbex Lab Tools; don't call it validated, and there's no need to redo the arithmetic by hand.
5. If the tool reports an input problem, fix the input or ask the scientist, then call it again.

Results are calculation aids. The scientist checks them against their own lab's requirements before use.
