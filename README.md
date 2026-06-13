# Neal's Net Calculator v1.0

Companion tool for the paper **"Neal's Net: A Self-Verifying Trigonometric System on the Fibonacci 60-Ring"** (Strassner, 2026).

**▶ Run it live:** https://nealstrassner.github.io/neals-net-calculator/

**📄 Paper + archived copy (OSF):** https://osf.io/n5pwt/

## How to use

Open the live link above — or download [`neals-net-calculator-v1.0.html`](neals-net-calculator-v1.0.html) and double-click it. It runs entirely offline: one file, no installation, no internet connection, and no data leaves your computer.

## What it does

An interactive implementation of the system described in the paper: the 60-digit Fibonacci ring, Neal's Net (the sum-to-ten chord grid), and the self-verifying angle arithmetic built on it. Use it to reproduce and check the paper's results yourself.

| Page | What it shows |
|---|---|
| **Start here** | plain-language tour for newcomers |
| **1 · Ring** | the 60-ring and the net; hover any digit to watch it pair to ten; trace all 28 chords |
| **2 · Angles & Folds** | checksummed folds and rotations — every jump carries its own digit test |
| **3 · COS** | the vesica cosine ruler: slide two rings, measure between centers, halve the distance |
| **4 · SIN** | the quarter-turn complement, then the ruler |
| **5 · TAN** | the gnomon tangent line, with its three certificates |
| **6 · Zoom ladder** | every step opens into 60 finer steps; the net survives at every level |
| **7 · Wheels** | the half-angle wheel, Heron's root wheel, and Archimedes' π ladder |
| **8 · Verify** | re-runs the paper's Appendix A checks **V1–V26** live, plus the acceptance test |

## Checking the paper's claims

Open the **Verify** tab and press **Run V1–V26 + acceptance**. Every check is recomputed from scratch on your machine — nothing is stored or looked up. Click any row to see its work. The ledger panel records a digit certificate for every operation you perform, and each entry expands to show the arithmetic that produced it.

The ring digits themselves are never stored: they are regenerated as Fibonacci mod 10 each time the page loads, and the net immediately checks them. The program is one readable file — View Source shows every line of code that exists.

## Credits

Neal's Net — the pairing-to-ten chord structure on the Fibonacci last-digit ring — was identified by **Neal Strassner** (c. 2015). The code was written by Claude (Anthropic) working under the author's direction; all mathematics is as stated in the paper and is machine-verified by the tool itself.

## License

[CC BY 4.0](LICENSE) — share and adapt freely, with credit to Neal Strassner.
