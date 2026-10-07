# HAUS OF SMELL 212: a small scent-number lookup

The [HAUS OF SMELL 212 custom scent builder](https://hausofsmell.com/212) offers 212 numbered scents for custom candles and sprays. In the live candle flow, a shopper chooses a product and vessel before reaching the scent step. The scent picker can be filtered by family or searched by name or number; it asks for **one scent per item**. This repository is a compact, source-checked sample for testing a number lookup interface, not a copy of the full live catalog.

## Why search by number?

Names can sound similar. A person who noted “007 Alpine Air” should be able to search 007 and see the same card rather than scroll through 212 options. A short lookup is useful when discussing a choice with someone else or checking a saved note before returning to the builder. It does not reserve stock, put anything in a cart, or establish that a particular scent is suitable for a person.

The sample entries below were visible in the live picker on 7 October 2026. The official page can change; use it for current choices, product formats, vessel pricing, label text and fulfillment.

| Number | Name | Picker imagery |
|---|---|---|
| 001 | Sea Salt & Driftwood | Sea Salt; Driftwood |
| 002 | Morning Dew | Morning Dew; Green Leaf |
| 003 | Clean Linen | Linen |
| 004 | Coastal Air | Ocean Wave; Open Sky |
| 005 | Crisp Cucumber | Cucumber |
| 006 | Watermint | Mint; Still Water |
| 007 | Alpine Air | Alpine Peaks; Open Sky |
| 008 | After Rain | Rain; Green Leaf |

## Lookup behavior

A minimal search can normalize the input with `trim().toLowerCase()` and match either the padded number or the name. Keep leading zeroes in display, because the actual picker uses three-digit labels. A result should show the exact number and name and point back to the live builder. The sample does not infer ingredient composition from a scent name or promise a finished fragrance outcome.

The 212 interface also offers family filters—Fresh, Floral, Woody, Citrus, Herbal, Gourmand, Spicy, Aquatic, Earthy and Smoky. Those filters help navigate the current list, but a shopper should still confirm the selected card before continuing to Label, Fulfillment and Review.

![Official HAUS OF SMELL candle collection image](https://hausofsmell.com/assets/candles-CgxNMBEq.png)

Source: [live HAUS OF SMELL 212 builder](https://hausofsmell.com/212).
