# CFWorkers-wrangler-bug-local-cors

## Bug

When using JS frontend code, Wrangler run locally in Dev mode causes a CORS error that can not be remedied.

But when I use the the same local HTML directly in the browser, it works as intended, with the results of the API call. (see console.log)  Also works correctly [deployed](https://video-transcript.video.workers.dev/).

submitted bug: https://github.com/cloudflare/workers-sdk/issues/9276

#### Testing

Put a YouTube video URL (with video ID) into the input field.
When you click the button, in the console you should see JSON response.

## Attempted fixes

In `public\_headers`, `Access-Control-Allow-Origin: *`

No help found in [Discord](https://discord.com/channels/595317990191398933/1371592359585906718/1371592359585906718) nor [/r/](https://www.reddit.com/r/CloudFlare/comments/1kl7w44/wrangler_blocked_by_cors_policy_the/)

## LICENSE

MIT, contains code from [my fork](https://github.com/tomByrer/youtube-captions-scraper) of  [algolia/youtube-captions-scraper](https://github.com/algolia/youtube-captions-scraper)
