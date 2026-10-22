# Mazhai

Next **60 minutes** of rain for three Chennai stations only:

1. **Kodambakkam** — near the railway station  
2. **Chennai Central** — near Park Station  
3. **Wimco Nagar** — near Wimco Nagar Metro  

Live radar (RainViewer) + hour outlook (MET Norway).

## Live site

**https://samdaniel05.github.io/mazhai-chennai/**

## Phone alerts (free, ₹0)

Get a notification on your phone when rain is expected at any of the three stations — even when the website is closed.

→ Full steps: **[ALERTS.md](./ALERTS.md)**

Short version:

1. Install **[ntfy](https://ntfy.sh)** (Android / iOS / web)
2. Subscribe to topic: `mazhai-chennai-samdaniel05`
3. Optional: set a private topic via GitHub secret `NTFY_TOPIC`

Backend = free **GitHub Actions** cron (no server cost).
