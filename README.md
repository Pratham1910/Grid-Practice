# Grid Practice

A CSS Grid layout practice project featuring a bento-box style card grid with 9 panels.

## Preview

A dark-background dashboard-style layout with 9 colored cards arranged in a 5-column, 5-row grid. The centerpiece is **card5** — a pink panel with a radial gradient circle and a portrait image. **card4** includes overlapping circular profile photos with a "+2" badge.

## Layout

The grid uses named template areas across a `5 × 5` track structure:

```
card1  card2  card2  card3  card4
card1  card5  card5  card5  card4
card6  card5  card5  card5  card4
card6  card5  card5  card5  card7
card6  card8  card9  card9  card7
```

**Columns:** `19% | 22% | 8% | 29% | 19%`  
**Rows:** `26% | 24% | 7% | 13% | 22%`

## Cards

| Card | Color | Span | Notes |
|------|-------|------|-------|
| card1 | Red | 2 rows, 1 col | Left tall panel |
| card2 | Blue | 1 row, 2 cols | Top center |
| card3 | Green | 1 row, 1 col | Top right-center |
| card4 | Light pink | 4 rows, 1 col | Right tall — team section with avatar stack |
| card5 | Pink | 3 rows, 3 cols | Center hero — portrait image with gradient circle |
| card6 | Magenta | 3 rows, 1 col | Left bottom tall |
| card7 | Orange | 2 rows, 1 col | Right bottom tall |
| card8 | Purple | 1 row, 1 col | Bottom center-left |
| card9 | Pink | 1 row, 2 cols | Bottom center-right |

## Files

- [index.html](index.html) — markup with grid container and 9 card divs
- [style.css](style.css) — all grid and card styles
- `Girl-removebg-preview.png` — portrait image used in card5

## Techniques Used

- CSS Grid with `grid-template-areas` for named placement
- `grid-template-columns` and `grid-template-rows` with percentage tracks
- Overlapping avatar images using negative `margin-right` and `border-radius: 50%`
- `position: absolute` for the portrait image anchored to the bottom of card5
- `radial-gradient` for the soft circle background in card5
