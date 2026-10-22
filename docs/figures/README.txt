LEGACY ECOSYSTEM ROLE MAP

Editable source: ecosystem_map.excalidraw
Exports and previews: ecosystem_map.svg, ecosystem_map.pdf, ecosystem_map.png
Vector drawing data: ecosystem_map_inline.tex

These files preserve an earlier editable role map and its exports. They are
not the figure currently included in the active summary.

The active figure source is ../roles_interactions.tex, and its compiled output
is ../roles_interactions.pdf. The summary includes that PDF directly.
It is a standalone TikZ vector figure designed at the manuscript's 160 mm
text width, with matching Latin Modern fonts. The central row follows tasks,
proof production, verification, and records/settlement. Supporting relations
show funding, forecasts, compute, and payments; shared rules apply across roles.

To update the active figure, run these commands from the repository root after
editing roles_interactions.tex:
  latexmk -pdf -no-shell-escape -interaction=nonstopmode -halt-on-error roles_interactions.tex
  latexmk -pdf -no-shell-escape -interaction=nonstopmode -halt-on-error -outdir=output/pdf verification_market_summary.tex
Inspect the figure in the resulting summary PDF.

The ecosystem manuscript is retired in ../archived/ and must not be updated
or reused as part of this workflow. Historical design guidance and rationale
are in ../resources/design/design_decisions.txt.
