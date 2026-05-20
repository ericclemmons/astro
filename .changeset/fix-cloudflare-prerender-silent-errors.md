---
'@astrojs/cloudflare': patch
---

Fixes an issue where rendering errors during workerd prerendering were silently swallowed, producing truncated HTML output without failing the build. Errors such as `ReferenceError` from missing imports now correctly propagate as build failures with clear error messages, matching the behavior of the Node prerenderer.
