# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 3.0.x   | :white_check_mark: |
| < 3.0   | :x:                |

## Reporting a Vulnerability

If you discover a security vulnerability, please:

1. **DO NOT** open a public issue
2. Email the maintainer directly (see package.json)
3. Include:
   - Description of the vulnerability
   - Steps to reproduce
   - Potential impact
   - Suggested fix (if any)

We'll respond within 48 hours and work on a fix ASAP.

## Security Considerations

This app:
- Runs entirely client-side (no server)
- Uses localStorage for favorites/history (local only)
- Service Worker caches assets (offline support)
- No external API calls except Google Fonts CDN
- No user authentication or sensitive data storage

## Best Practices

- Keep dependencies updated
- Review service worker cache strategy
- Validate all user inputs
- Use Content Security Policy headers when hosting
