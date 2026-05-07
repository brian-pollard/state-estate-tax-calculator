# 2026 State Estate Tax Calculator

A browser-based tool that computes estate tax liability for all 13 U.S. estate tax jurisdictions — no installation, no account, no spreadsheet required.

**[Live Tool →](https://brian-pollard.github.io/state-estate-tax-calculator/)**

---

## What It Does

Select a state and enter an estate value. The calculator instantly shows:
- Detailed tax computation for your selected state (computation method, exemption, bracket breakdown)
- A summary of all other estate tax states for comparison
- Whether the estate exceeds each state's exemption threshold

Covers all **13 jurisdictions** with an estate tax in 2026: Connecticut, DC, Hawaii, Illinois, Maine, Maryland, Massachusetts, Minnesota, New York, Oregon, Rhode Island, Vermont, and Washington.

---

## The 13 Estate Tax Jurisdictions (2026)

| State | Exemption | Top Rate | Method |
|-------|-----------|----------|--------|
| Connecticut | $15,000,000 | 12% flat | Flat rate |
| DC | $4,988,400 | 16% | Direct bracket table |
| Hawaii | $5,490,000 | 20% | Graduated on excess |
| Illinois | $4,000,000 | ~16% | Old federal credit table |
| Maine | $7,160,000 | 12% | Graduated on excess |
| Maryland | $5,000,000 | ~16% | Old federal credit table + 10% inheritance tax |
| Massachusetts | $2,000,000 | ~16% | Old federal credit table |
| Minnesota | $3,000,000 | 16% | Graduated on excess |
| New York | $7,350,000 | 16% | Graduated with cliff provision |
| Oregon | $1,000,000 | ~16% | Old federal credit table |
| Rhode Island | $1,838,056 | ~16% | Old federal credit table |
| Vermont | $5,000,000 | 16% flat | Flat rate |
| Washington | $3,000,000–$3,076,000 | 20–35% | Dual rate structure (two periods in 2026) |

The remaining 37 states + territories have no estate tax.

---

## Key Notes

- **New York cliff:** Estates between $7.35M and $7.72M face a phase-out that can make a slightly larger estate owe more tax than a slightly smaller one — the tool shows this explicitly
- **Washington 2026:** Two different rate structures apply depending on date of death (Period A: Jan–Jun, Period B: Jul–Dec)
- **Maryland:** The only state with both an estate tax and a separate inheritance tax on non-lineal heirs
- **"Old federal credit table" states** (IL, MA, MD, OR, RI): These states compute tax using the pre-2001 federal State Death Tax Credit table (IRC § 2011), which produces a graduated effective rate

---

## Implementation

Single self-contained HTML file. No build step, no external JS dependencies, no server required. Open `docs/index.html` directly in any browser.

All computation logic validated against official state tax authority forms and statutes (April 2026).
