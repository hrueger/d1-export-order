# Export Order Issue

## Setup
1. Create a DB (e.g. `export-order-issue-db-1`) and update `wrangler.toml`
2. Run `npx wrangler d1 migrations apply export-order-issue-db-1 --remote`
3. Run `npx wrangler d1 export export-order-issue-db-1 --remote --output export.sql`
4. Run `npx wrangler d1 execute export-order-issue-db-1 --local --file export.sql` or use export-example-broken.sql