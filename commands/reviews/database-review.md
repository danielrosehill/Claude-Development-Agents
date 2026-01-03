# Database Architecture Review

Conduct a thorough review of this project's database design and usage.

Analyze the following areas:

## Performance & Optimization
- **Indexing**: Are frequently-queried columns properly indexed? Are there missing indexes causing slow queries?
- **Query Efficiency**: Are there N+1 query patterns, unnecessary JOINs, or queries that could be optimized?
- **Connection Management**: Is connection pooling configured appropriately?

## Schema Design
- **Relationships**: Are foreign keys and relationships properly defined? Are there logical connections that should exist but don't?
- **Normalization**: Is the schema appropriately normalized, or are there denormalization opportunities for performance?
- **Data Types**: Are column types optimal for their actual usage?

## Untapped Potential
- **Unused Relationships**: What useful data relationships exist in the schema that the application isn't leveraging?
- **Missing JOINs**: Could we create beneficial joins or views that would enable new features?
- **Aggregations**: Are there summary tables or materialized views that would improve common queries?

## Fundamental Fit
- **Right Database?**: Given the actual data patterns (relational, document, time-series, graph), is this the right type of database?
- **Scaling Considerations**: Will this design handle anticipated growth?

Provide specific recommendations with SQL examples where helpful.
