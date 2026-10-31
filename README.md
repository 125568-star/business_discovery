# Business Discovery Network

Standalone repository for Ground Support Crew's Business Discovery Network.

- Main website: https://groundsupportcrew.com/business-discovery/
- Site source: `index.html`
- Existing Ground Support Crew website listing is retained.

## Supabase connection

- Existing project: `Coordinator` (planned display name `Entry Box`)
- Project reference: `pulbcpjwxliwnmkiyfhe`
- Separate database schema: `business_discovery`
- Tables: `businesses`, `categories`, `submissions`
- Supabase Edge Function: `business-discovery`
- API: `https://pulbcpjwxliwnmkiyfhe.supabase.co/functions/v1/business-discovery`

Do not expose the Supabase service-role key in the browser or repository.

## Deployment

The original site at the Ground Support Crew subpath remains in place. This repository is the new standalone source; pushing code alone does **not** establish a new hosting domain.

The API currently accepts browser requests from `groundsupportcrew.com` only. If this repository is deployed to another domain, update the Edge Function's allowed origins and the canonical URL in `index.html`. An administrator review interface remains to be implemented.

Free submissions do not require reciprocal links. Only approved business listings are published.
