# Browser and Client-Side Hardening

- Disabling "remember me" features.
- Disabling caching for sensitive pages
- HTTPS everywhere: server and application
- Newest version of TLS

## Use every possible security header

- `X-XSS-Protection: 1; mode=block`
- `Content-Security-Policy: default-src ‘self’; block-all-mixed-content;`
- `X-Frame-Options: SAMEORIGIN (to allow your site to frame itself)` or `X-Frame-Options: DENY (to block all framing)`
- `X-Content-Type-Options: nosniff`
- `Referrer-Policy: strict-origin-when-cross-origin`
- `Strict-Transport-Security: max-age=31536000; includeSubDomains`
- `X-Permitted-Cross-Domain-Policies: none`
- `Access-Control-Allow-Origin: https://site-that-you-trust.com`
- `Expect-CT: max-age=86400, enforce, report-uri=”https://myserver/report"`
- `Feature-Policy: camera ‘none’; microphone ‘none’; speaker ‘self’; vibrate ‘none’; geolocation ‘none’; accelerometer ‘none’; ambient-light-sensor ‘none’; autoplay ‘none’; encrypted-media ‘none’; gyroscope ‘none’; magnetometer ‘none’; midi ‘none’; payment ‘none’; picture-in-picture ‘none’; usb ‘none’; vr ‘none’; fullscreen *;`
- `<httpRuntime enableVersionHeader=”false” />`
- Also remove it on the server

securityheaders.com
ssllabs.com
harderize.com
