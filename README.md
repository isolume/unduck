# Unfuck

DuckDuckGo's bang redirects are too slow. Add the following URL as a custom search engine to your browser. Enables all of DuckDuckGo's bangs to work, but much faster.

> [!NOTE]
> This is an "unfucked" version of unduck. Feel free to use it, but it is opinionated. It adds other AI sites as bangs, removes links to Theo's sites, and removes any analytics.

```
https://f.umi.to?q=%s
```

## How is it that much faster?

DuckDuckGo does their redirects server side. Their DNS is...not always great. Result is that it often takes ages.

I solved this by doing all of the work client side. Once you've went to https://f.umi.to once, the JS is all cache'd and will never need to be downloaded again. Your device does the redirects, not me.
