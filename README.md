# nginx on Blossom

The smallest app Blossom can deploy: nginx serving a static page. It builds in
seconds, so Blossom QA uses it where a test needs many deploys, such as
Preview Environments.

- Build: **Dockerfile** (the root `Dockerfile`)
- Port: `80`
- Health check: `/`

`/marker.txt` returns a one-line marker. Change it in a commit to prove which
commit a deploy serves.
