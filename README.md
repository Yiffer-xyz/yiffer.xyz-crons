# Yiffer Crons

This is a Cloudflare Worker that runs crons for yiffer.xyz.

So far, there's one cron running a handful jobs every midnight UTC:

- Publish comics from the queue
- Expire ads
- Clear spammable actions table
- Sync patrons from Patreon

The API key for the worker's requests is stored in the `CRON_KEY` secret, which is set in Cloudflare cli/dashboard.

Deploy to Cloudflare using Wrangler.
