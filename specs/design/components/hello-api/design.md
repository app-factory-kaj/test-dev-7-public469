---
type: service
language: Go
buildpack: docker
appPath: hello-api
entrypoint: deployment/service
---

# hello-api

Build a minimal Go HTTP service using net/http on port 9090. Expose GET /hello returning {"message": "Hello, World!"} as JSON. Include GET /health returning 200 OK. This is a public API — no authentication required. Use the golang:1.25-alpine builder base image in the Dockerfile. Follow the go skill's multi-stage Dockerfile pattern with a slim alpine runtime. No database or persistence needed.
