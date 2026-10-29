# Protomaps on Cloudflare

> **Deprecated for Norgeskart.** The `tiles` Worker deployed from this folder no longer serves
> tiles.norgeskart.net. Since 2026-10-29 that domain is served by the `norgeskart-tiles` Worker
> (github.com/norgeskart/tiles), with the same tile URLs. Don't redeploy this one.

See installation and configuration instructions at [Protomaps Docs: Deploy on Cloudflare](https://docs.protomaps.com/deploy/cloudflare)

## Development

### Web Console (basic)

Generate the Workers script using `npm run build` and copy `dist/index.js` to the editor.

### Wrangler (advanced)

The `preview_bucket_name` value in `wrangler.toml` should be changed to your bucket used for development.

Run `npm run start` to serve your Worker at http://localhost:8787. The cache will not be active in development.
