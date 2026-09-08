PROBLEMS / SOLUTIONS

1.) Often long hang times on webpages

- Enabled parallel requests
- Set rate limit to 0 (no limit)
- Changed DNS servers from default "https://dns10.quad9.net:443/dns-query" to Cloudflare's 1.1.1.1, 1.0.0.1 (36ms vs 15ms)
