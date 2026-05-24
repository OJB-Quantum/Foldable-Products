# Catalog Codebook

## Core identity fields

`product_id` is a stable lowercase identifier derived from brand and product
name. `brand`, `product_name`, and `market_category` describe the product-level
identity.

## Mechanism fields

`transformation_family` and `transformation_subtype` encode the high-level
taxonomy. `fold_mechanism`, `fold_architecture`, and `compacting_motion` record
the physical mechanism in progressively more descriptive language.

## Evidence fields

`source_type`, `source_url`, `normalized_source_url`, and `source_domain`
support source tracking. `review_status` separates canonical seed records from
records needing source or measurement review.

## Measurement fields

Folded and deployed dimensions use millimeters. Mass uses grams. Price uses USD
when available. Compression ratio should compare deployed volume to folded
volume when both volumes are measured consistently.

## Score fields

All sub-scores use a 0 to 5 scale. `foldability_score` is a weighted review
score. It should guide triage while direct evidence should decide catalog
promotion.
