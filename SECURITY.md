# Security

Sorify processes files locally and talks to the network only to download its components, speech models and updates from GitHub, PyPI, the PyTorch index and the FFmpeg builds published on GitHub. Update downloads are verified by SHA-256 against the digest GitHub reports for the release asset before they run.

## Reporting a vulnerability

Please do not open a public issue for security problems. Use GitHub's private report form instead: **Security → Report a vulnerability** on this repository (https://github.com/AnthonyFararoni/Sorify/security/advisories/new). Include the Sorify version, what you found and how to reproduce it. You will get an answer within a week, and a fix is published as a new release.

## Verifying a download

Every release ships `SHA256SUMS.txt`. On Windows:

```text
certutil -hashfile Sorify-Setup-1.0.0.exe SHA256
```

The printed hash must match the line for that file.
