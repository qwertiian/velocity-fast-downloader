# Security policy

## Reporting a vulnerability
Please **don't** open a public issue. Use GitHub's private reporting instead: **Security** tab
→ **Report a vulnerability**. Include the Velocity version, Windows version, steps to
reproduce and the impact. You'll get a reply within 72 hours.

## Supported versions
Only the latest release receives security fixes. Please update before reporting.

## Verifying downloads
Every release includes `SHA256SUMS.txt`. Check your installer with:

```powershell
Get-FileHash .\Velocity_x64-setup.exe -Algorithm SHA256
```

Official downloads come only from
`https://github.com/qwertiian/velocity-fast-downloader/releases` and the official website
linked from this repository. Copies from anywhere else may be tampered with.

## What Velocity guarantees
- TLS certificates are always verified; secure (https) downloads can't be silently downgraded to http.
- Server-supplied file names are sanitized (no writing outside your download folder).
- Downloaded files are never executed automatically.
- No telemetry, and no open network ports on your machine.
