# Mathematics Market Manuscript

- [Summary](verification_market_summary.tex) · [PDF](output/pdf/verification_market_summary.pdf)
- [Current roles and interactions figure](roles_interactions.tex) · [PDF](roles_interactions.pdf)
- [Overleaf project](https://www.overleaf.com/project/6ab6baa74349edae79fa13fc)

The summary is the only active manuscript. It uses the AMS `amsart` mathematics
article class, Latin Modern fonts, numbered equations, and blue
alphabetic citations and reference links. Its figure is loaded from
`roles_interactions.pdf` in this directory. The figure uses TikZ and matching
Latin Modern fonts, with a central task-to-settlement flow and separate
funding, information, and compute relations.
The current manuscript PDF is in `output/pdf/`, and research materials are in
`resources/`.

Text provenance, checked October 14, 2026: the user-designated text baseline is
`/Users/moqian/Downloads/MathMarket.pdf`; its body matches Overleaf commit
`3e8c7b3`. The user has confirmed the revised manuscript with the restored
introduction, requested Section 3 revisions, and consolidated Justin Sun Prize
citations. See [the version audit](resources/version_audit.md) for the checked
differences and synchronization history. After publishing, compare the local
commit with Overleaf's remote `main`; agreement between local PDF builds alone
does not establish agreement with Overleaf.

The ecosystem manuscript was retired on October 14, 2026. Its source and PDF
are preserved in [archived/](archived/README.md) for historical reference only.
We no longer maintain or reuse it as a manuscript or template. Make future
manuscript changes in `verification_market_summary.tex`.

With a TeX installation and `latexmk`, run these commands from this directory:

```sh
latexmk -pdf -no-shell-escape -interaction=nonstopmode -halt-on-error roles_interactions.tex
latexmk -pdf -no-shell-escape -interaction=nonstopmode -halt-on-error -outdir=output/pdf verification_market_summary.tex
```

Compilation auxiliaries are ignored by Git. Review the summary PDF after changing
the source, including figure placement, section transitions, and references.

Keep the active source, its current PDF, and supporting figure in sync.
Older role-map files remain in `figures/`; see its README for their status.
