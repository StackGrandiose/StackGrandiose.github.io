---
title: Making Youtube Less Fun
date: 2024-02-26
tags: Internet
draft: false
---

**[<-- Back]({{< ref "_index.md" >}})**

Youtube.com can be argued as a non-social media platform. It can be used
simply as a way to host videos or a place to learn new things. However,
this guise of educational value can lead to a cyclical addiction. I have
struggled with using Youtube in a moderated way and have unfortunately
spent a lot of time wasting away watching Youtube videos. Yes, youtube has
some value in terms of personal development and learning, but the
destructive patterns Youtube makes you go into makes the tradeoff seem
unwise. However, I have overtime been able to make Youtube less enjoyable
to watch mindlessly yet still be available to refer to as a way to learn. 

### UNHOOK

As of now, I find the browser extention [Unhook](https://unhook.app/) to
be the easiest to use solution in terms of blocking most addicting
features. The extention allows you to toggle on and off features
individually. I have almost all features turned off except hiding the top
header, as searching up videos is easier than using a search engine like
DuckDuckGo.

### UBLOCK ORIGIN

For a while, I was using a browser extention that focused on blocking
youtube shorts. However, I am now using a filter for Ublock Origin from
[letsblock.it](https://letsblock.it/filters/youtube-shorts). Copy and
pasting these lines into "My Filters" in Ublock completely blocks the
viewing of shorts.

```
www.youtube.com##ytd-guide-renderer a.yt-simple-endpoint path[d^="M10 14.65v-5.3L15 12l-5 2.65zm7.77-4.33"]:upward(ytd-guide-entry-renderer)
www.youtube.com##ytd-mini-guide-renderer a.yt-simple-endpoint path[d^="M10 14.65v-5.3L15 12l-5 2.65zm7.77-4.33"]:upward(ytd-mini-guide-entry-renderer)
www.youtube.com##ytd-browse[page-subtype="home"] .ytd-thumbnail[href^="/shorts/"]:upward(ytd-rich-item-renderer)
www.youtube.com##ytd-browse[page-subtype="subscriptions"] .ytd-thumbnail[href^="/shorts/"]:upward(ytd-grid-video-renderer,ytd-rich-item-renderer)
www.youtube.com##ytd-search .ytd-thumbnail[href^="/shorts/"]:upward(ytd-video-renderer)
www.youtube.com##ytd-browse[page-subtype="subscriptions"] ytd-video-renderer .ytd-thumbnail[href^="/shorts/"]:upward(ytd-item-section-renderer)
www.youtube.com##ytd-watch-next-secondary-results-renderer .ytd-thumbnail[href^="/shorts/"]:upward(ytd-compact-video-renderer,ytd-shelf-renderer)
www.youtube.com##ytd-browse[page-subtype="trending"] .ytd-thumbnail[href^="/shorts/"]:upward(ytd-video-renderer)
www.youtube.com##ytd-search .ytd-thumbnail[href^="/shorts/"]:upward(ytd-video-renderer)
www.youtube.com##ytd-notification-renderer:has(> a[href^="/shorts/"])
www.youtube.com##ytd-rich-shelf-renderer[is-shorts]
www.youtube.com##ytd-rich-shelf-renderer[is-shorts].ytd-rich-section-renderer:upward(ytd-rich-section-renderer)
www.youtube.com##ytd-reel-shelf-renderer
m.youtube.com##ytm-reel-shelf-renderer
m.youtube.com##ytm-pivot-bar-renderer div.pivot-shorts:upward(ytm-pivot-bar-item-renderer)
m.youtube.com##ytm-browse ytm-item-section-renderer ytm-thumbnail-overlay-time-status-renderer[data-style="SHORTS"]:upward(ytm-video-with-context-renderer)
m.youtube.com##ytm-browse ytm-item-section-renderer ytm-thumbnail-overlay-time-status-renderer[data-style="SHORTS"]:upward(ytm-compact-video-renderer)
m.youtube.com##ytm-search ytm-thumbnail-overlay-time-status-renderer[data-style="SHORTS"]:upward(ytm-compact-video-renderer,ytm-video-with-context-renderer)
m.youtube.com##ytm-single-column-watch-next-results-renderer ytm-thumbnail-overlay-time-status-renderer span:has-text(/^(0:\d\d|1:0\d)$/):upward(ytm-video-with-context-renderer)
youtube.com##ytd-rich-grid-row, #contents.ytd-rich-grid-row:style(display:contents !important;)
```

Lastly, to make the last way of browsing videos (typing in the search bar)
even more boring, I removed all video information except the title, view
count, published date and description. Searching up videos now presents
you with a list.

```
i.ytimg.com/$domain=www.youtube.com,image
www.youtube.com###channel-info
www.youtube.com###left-section
www.youtube.com###header
www.youtube.com##ytd-thumbnail.ytd-video-renderer.style-scope
> .ytd-thumbnail.style-scope.inline-block.yt-simple-endpoint
www.youtube.com##ytd-thumbnail.ytd-video-renderer.style-scope 
```
