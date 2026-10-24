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

## Proposed fix
Say clearly up front when an item is unavailable, then show matched in-stock
alternatives with a reason tag (closest size, smaller pack, larger pack).
- **Success metric:** checkout completion rate in sessions that hit an unavailable item
- **Guardrail:** cancellation and substitution complaint rate
- **Decision rule:** ship if completion rises by at least 3 points with no guardrail regression after 2 weeks

## Files
- `deck/`: the presentation (PDF)
- `data/`: the cleaned Excel workbook (start at the Key Findings sheet)
- `design/`: concept mock of the proposed screen (sample products, not real inventory)

## Method
30 specific items across 5 categories, searched on both apps. For each item I
recorded the price and whether I could add it to cart. "Unavailable" means sold
out or not listed.

## Limits
One city, one time slot, one run. Screenshots were taken later than the data.
Instamart prices reflect a Swiggy One membership. Blinkit showed low stock
("3 left", "2 left") on some items, so its availability is a snapshot.

Independent personal project, not affiliated with Instamart, Blinkit or their parent companies.
