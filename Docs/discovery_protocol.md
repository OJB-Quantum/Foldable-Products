# Discovery Protocol

This document describes how the repository expands beyond manually curated seed
products.

## Goal

The discovery notebook searches broad product-category queries, captures
candidate URLs, classifies each candidate by physical transformation family,
scrapes metadata when allowed, and exports review tables.

## Candidate status

Rows in `data/discovery_candidates.csv` and
`data/discovery_candidates_enriched.csv` are leads. A lead becomes a canonical
catalog record only after manual review confirms the product exists, the source
is credible, and the transformation mechanism is correctly classified.

## Transformation families

- Foldable products compact through hinges, creases, flexures, flexible display
  laminates, or origami-like panel networks.
- Collapsible products compact through nesting, telescoping, shell collapse,
  soft-vessel volume evacuation, or frame-assisted collapse.
- Rollable products compact by winding a flexible sheet or membrane.
- Inflatable products compact through deflation.
- Modular products compact through disassembly or flat-pack conversion.
- Hybrid products combine multiple transformation families.

## Review checklist

1. Verify the URL points to a real product, official page, standards page,
   manufacturer page, or high-quality retailer listing.
2. Confirm whether the transformation is foldable, collapsible, rollable,
   inflatable, modular, or hybrid.
3. Record dimensions, mass, folded volume, deployed volume, price, release year,
   certifications, and material stack when available.
4. Promote reviewed rows into `data/products_seed.csv` or a future canonical
   `data/products.csv`.
