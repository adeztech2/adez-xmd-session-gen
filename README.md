# ADEZ XMD Pair Site

Static page that calls the ADEZ XMD pairing API on Heroku.

## Setup

1. In `index.html`, set `API` to your Heroku app URL (no trailing slash).
2. On Heroku, set the allowed origin to this site's address:
   heroku config:set ALLOWED_ORIGIN=https://your-site.netlify.app
3. Deploy this folder to Netlify Drop or GitHub Pages.
4. Turn on the Heroku web dyno while pairing: heroku ps:scale web=1 worker=1
5. After pairing, turn it off: heroku ps:scale web=0 worker=1

Developed by Arnold Adez
