# Free phone rain alerts (₹0)

Mazhai uses **GitHub Actions** as a free backend and **[ntfy](https://ntfy.sh)** for phone notifications.

No SMS fees. No server bill. Works when the website is closed.

## 1. Install ntfy

- **Android:** [Play Store – ntfy](https://play.google.com/store/apps/details?id=io.heckel.ntfy)
- **iPhone:** [App Store – ntfy](https://apps.apple.com/app/ntfy/id1625396343)
- Or open **https://ntfy.sh** in a mobile browser

## 2. Subscribe to your topic

Default topic for this repo:

```text
mazhai-chennai-samdaniel05
```

In the ntfy app: **+** → subscribe → paste that topic → Subscribe.

You’ll get a high-priority notification when rain is expected **this hour** at any of:

- Kodambakkam  
- Chennai Central  
- Wimco Nagar  

## 3. (Optional) Private topic

Anyone who knows the topic name can subscribe. To use a secret name:

1. Pick a hard-to-guess topic, e.g. `mazhai-sam-x7k9`
2. Repo → **Settings → Secrets and variables → Actions → New repository secret**
3. Name: `NTFY_TOPIC`  
   Value: your secret topic
4. Subscribe to **that** topic in the ntfy app instead

## 4. Test

GitHub → **Actions → Rain phone alerts → Run workflow**

If any station is wet this hour, your phone should ping within about a minute.

The checker also runs automatically about every **15 minutes**.

## Notes

- Free tier GitHub Actions can run a few minutes late — normal.
- Alerts are for the **next hour** rainfall (MET Norway), not minute-by-minute radar.
- To stop alerts: unsubscribe in ntfy, or disable the workflow under Actions.
