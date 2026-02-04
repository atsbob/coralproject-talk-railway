# Deploying Coral Talk Comments on Railway
Deploy Vox Media's Coral Talk commenting platform on Railway.

## CORS (required when embedding Talk on a website)

For production, add the origin domain you plan to embed your Talk service to to avoid CORS errors. 

`ALLOWED_ORIGINS=https://example.com`

`ALLOWED_ORIGINS=https://example.com,https://www.example.com` (for multiple domains or variations)


## Front with proxy or CDN for production

It’s recommended to run Talk behind a reverse proxy or CDN (e.g. Cloudflare, Fastly, or CloudFront). Since Talk serves dynamic, user-specific content, disable edge caching and forward all headers, cookies, and query strings to avoid unexpected behavior.
