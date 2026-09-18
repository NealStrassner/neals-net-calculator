# Neal's Net Calculator v3.0

Companion tool for the paper **"Neal's Net: A Self-Verifying Trigonometric System on the Fibonacci 60-Ring"** (Strassner, 2026).

**▶ Run it live:** https://nealstrassner.github.io/neals-net-calculator/

**📄 Read the paper (Zenodo, citable DOI):** https://doi.org/10.5281/zenodo.20754147

## How to use

Open the live link above — or download [`neals-net-calculator-v3.0.html`](neals-net-calculator-v3.0.html) and double-click it. It runs entirely offline: one file, no installation, no internet connection, and no data leaves your computer.

## What it does

An interactive implementation of the system described in the paper: the 60-digit Fibonacci ring, Neal's Net (the sum-to-ten chord grid), and the self-verifying angle arithmetic built on it. Every trigonometric value on the page is computed by Neal's Net's own engine, from the ring's anchors — never the browser's `Math.sin/cos/tan`. The one place the browser's library appears is a side-by-side self-check that proves the two agree.

| Tab | What it shows |
|---|---|
| **1 · Ring** | the 60-ring and the net; hover any digit to watch it pair to ten; the twin grid and the 12-point skeleton; trace all the chords |
| **2 · Angles & Folds** | checksummed folds and rotations — every jump carries its own digit test |
| **3 · COS (two-ring ruler)** | slide two rings, measure between centres, halve the distance |
| **4 · SIN** | the crossing distance read at the same setting |
| **5 · TAN (gnomon)** | the gnomon tangent line, with its certificates |
| **6 · Zoom ladder** | every step opens into 60 finer steps; the net survives at every level |
| **7 · Wheels** | the half-angle wheel, the root wheel, and the π ladder |
| **8 · Polygon checks** | the surds the ring produces — tan 60° = √3, cos 36° = φ⁄2, tan 36°·tan 72° = √5 |
| **9 · Why 60** | why sixty is the smallest wheel that carries the 3-, 4- and 5-fold figures |
| **10 · Sister nets** | the other digit nets and how they compare |
| **11 · Verify** | re-runs the paper's checks live, plus the self-check of the trig engine against the standard library |

## Checking the paper's claims

Open the **Verify** tab and run the checks. Every one is recomputed from scratch on your machine — nothing is stored or looked up. Click any row to see its work. The ledger panel records a digit certificate for every operation you perform, and each entry expands to show the arithmetic that produced it.

The ring digits themselves are never stored: they are regenerated as Fibonacci mod 10 each time the page loads, and the net immediately checks them. The program is one readable file — View Source shows every line of code that exists.

## Credits

Neal's Net — the pairing-to-ten chord structure on the Fibonacci last-digit ring — was identified by **Neal Strassner** (c. 2015). The code was implemented by Claude (Anthropic) working under the author's direction; all mathematics is as stated in the paper and is machine-verified by the tool itself.

## License

[CC BY 4.0](LICENSE) — share and adapt freely, with credit to Neal Strassner.
