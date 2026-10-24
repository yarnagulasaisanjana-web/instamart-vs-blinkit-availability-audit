# Quick-commerce availability audit: Instamart vs Blinkit (Vizag)

An informal product audit of 30 everyday grocery items on Instamart and Blinkit.
Checked in Vizag at about 7pm on 23 Oct 2026.

## Headline
12 of 30 items were unavailable on Instamart (sold out or not listed) vs 1 on Blinkit.
On the 18 items in stock on both apps, prices differed by 0.6%.

## Key numbers
| | Instamart | Blinkit |
|---|---|---|
| Items I could add to cart | 18 of 30 (60%) | 29 of 30 (97%) |
| Like-for-like basket (18 shared items) | ₹1,453 | ₹1,444 |
| Items cheaper (shared items) | 6 | 6 (6 tied) |

## What I observed
- Both apps show other products when an exact item is unavailable.
- In my searches, Blinkit labeled the unavailable item as out of stock in the results.
  On Instamart I had to scroll to find out the exact item was sold out.
- Blinkit showed low stock on some items ("3 left" on curd, "2 left" on paneer).

## Proposed fix
Say clearly up front when an item is unavailable, then show matched in-stock
alternatives with a reason tag (closest size, smaller pack, larger pack).
- **Success metric:** checkout completion rate in sessions that hit an unavailable item
- **Guardrail:** cancellation and substitution complaint rate
- **Decision rule:** ship if completion rises by at least 3 points with no guardrail regression after 2 weeks

## Files
- [`DECK/`](DECK): the presentation (PDF)
- [`DATA/`](DATA): the cleaned workbook (.xlsx) and CSV versions of its sheets.
  Start with [`key_findings.csv`](DATA/key_findings.csv), then [`price_comparison.csv`](DATA/price_comparison.csv).
- [`DESIGN/`](DESIGN): concept mock of the proposed screen (sample products, not real inventory)

## Method
30 specific items across 5 categories, searched on both apps. For each item I
recorded the price and whether I could add it to cart. "Unavailable" means sold
out or not listed. Comparisons use only items in stock on both apps.

## Limits
- One city, one time slot, one run
- Screenshots were taken later than the data
- Instamart prices reflect a Swiggy One membership
- Blinkit's low stock means its 97% is a snapshot
- The design mock uses sample products and prices

*Independent personal project, not affiliated with Instamart, Blinkit or their parent companies.*
