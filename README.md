# Face Detection

A browser-based real-time face detection app using the device camera.

**Live demo:** https://munkys.dev/face

> Requires camera access (getUserMedia); served over HTTPS.

## Run locally
Serve it with Docker (camera APIs need a secure context / localhost):

```bash
docker build -t face-detection .
docker run --rm -p 8080:80 face-detection
```

Then open http://localhost:8080

## Deployment
Deployed as a lightweight Nginx container behind Caddy on munkys.dev under `/face`.
