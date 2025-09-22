# Static Site with Nginx + rsync Deploy

This project demonstrates how to set up a basic Linux server on AWS EC2,
serve a static site with Nginx, and deploy changes using rsync.

## Project structure

static-site/
├── index.html
├── styles.css
├── images/
├── .gitignore
└── deploy.sh (local only, excluded from Git)

## Deploy
Run:
```bash
./deploy.sh
```

This syncs files to the EC2 server and reloads Nginx.
Notes

- Secrets (e.g. PEM keys) are never committed.
- deploy.sh and .rsyncignore are excluded from Git.

