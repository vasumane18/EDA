# EDA
Inconsistent Country Naming Conventions
Challenge: Merging and grouping data was initially disrupted by inconsistent regional names and varying string formats across data entries (e.g., shorthand abbreviations vs. full official names), which can lead to dropped records during analysis.
Standardized the dataset by mapping and renaming country identifiers into a uniform format during the initial data-cleaning phase, ensuring seamless aggregation and indexing.

Time-Series Data Sparsity (Missing Timelines)
Challenge: The raw dataset contained gaps and unrecorded years for specific nations. Using a simple global average to fill these gaps would completely distort an individual country's true economic scale.
Handled missing data by grouping the dataset by country and applying a localized Forward Fill (ffill) and Backward Fill (bfill) sequence. This ensured missing values were realistically estimated based on that specific country's closest historical trends.
