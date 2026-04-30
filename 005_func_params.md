# Func Params

Try using:
- `cib` - change in brackets (works for `()`)
- `cab` - change around brackets
- `ci(` or `ci)` - change in parentheses
- `ci{` or `ci}` - change in curly braces
- `ci[` or `ci]` - change in square brackets
- `ci"` or `ci'` - change in quotes
- `vib` - highlight in brackets
- `vab` - highlight around brackets

```typescript
function filterAndFormatProducts(
  products: Product[], // list of products
  categoryFilter: string, // category to filter
  sortDirection: "asc" | "desc" // sort order by price
): string[] {
  const filtered = products.filter((product) => {
    return categoryFilter
      ? product.category.toLowerCase() === categoryFilter.toLowerCase()
      : true;
  });

  const sorted = filtered.sort((a, b) => {
    if (sortDirection === "asc") {
      return a.price - b.price;
    }
    return b.price - a.price;
  });
  const formatted = sorted.map((product) => {
    return `${product.name} - $${product.price.toFixed(2)}`;
  });

  console.log(`Filtered ${products.length} products down to ${formatted.length}`);
  console.log(`Category: ${categoryFilter || "All"}`);
  console.log(`Sort direction: ${sortDirection}`);

  return formatted;
}
```
