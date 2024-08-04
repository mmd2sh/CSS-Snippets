# CSS-Snippets

# Responsive Grid
```
.grid-list-wrapper {
  --grid-column-count: 5;
  --grid-layout-gap: 15px;
  --grid-item-min-width: 200px;
  --gap-count: calc(var(--grid-column-count) - 1);
  --total-gap-width: calc(var(--gap-count) * var(--grid-layout-gap));
  --grid-item-max-width: calc((100% - var(--total-gap-width)) / var(--grid-column-count));
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(max(var(--grid-item-min-width), var(--grid-item-max-width)), 1fr));
  grid-gap: 20px var(--grid-layout-gap);
}
```
