# Bronco Board of Fame

## Overview

A static website project. The repository currently contains a single `index.html` file (the entry point) and a LICENSE.

## Project Layout

- `index.html` — Site entry point (currently empty).
- `LICENSE` — Project license.

## Tech Stack

- **Language / Runtime:** Static HTML (served with Python 3.11's built-in `http.server` during development).
- **No build step.** Files are served directly.

## Replit Setup

### Development Workflow

A single workflow named **"Start application"** runs:

```
python3 -m http.server 5000 --bind 0.0.0.0
```

- Binds to `0.0.0.0` on port `5000` so the Replit preview iframe can reach it through the proxy.
- Python's `http.server` does not validate the `Host` header, so it works correctly behind Replit's proxy.

### Deployment

Configured for **static** deployment (`deploymentTarget: "static"`) with `publicDir: "."`. No build command is required since there is nothing to compile.

## Notes

- The project is in a minimal starter state — `index.html` has no content yet. Add markup to start building the site.
