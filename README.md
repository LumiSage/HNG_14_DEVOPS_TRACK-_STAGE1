# HNG_14_DEVOPS_TRACK-_STAGE1
Build &amp; Deploy a Personal API
# Stage 1 API — DevOps Track

A minimal REST API deployed on a VPS with Nginx reverse proxy.

## Run locally

```bash
npm install
node server.js
# API available at http://localhost:3000
```

## Endpoints

| Method | Path | Response |
|--------|------|----------|
| GET | `/` | `{"message": "API is running"}` |
| GET | `/health` | `{"message": "healthy"}` |
| GET | `/me` | `{"name": "...", "email": "...", "github": "..."}` |

## Live URL

[http://your-server-ip-or-domain](https://emmahngdevops.mooo.com/)

## Deployment

- VPS: Ubuntu 22.04
- App server: Node.js + Express on port 3000
- Reverse proxy: Nginx on port 80
- Process manager: systemd (auto-restarts on crash/reboot)
