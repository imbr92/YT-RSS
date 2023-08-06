# YT-RSS
## RSS-based local syncing for youtube subscriptions

<details>
 <summary><strong>Table of Contents</strong> (click to expand)</summary>

- [Setup](#setup)
- [Configuration](#configuration)
- [Getting Feeds](#getting-feeds)
- [cron](#cron)
</details>

## Setup

```bash
git clone https://github.com/imbr92/YT-RSS.git
cd YT-RSS
chmod +x yt-rss
```
and make sure yt-rss is in your `$PATH` (i.e. by symlinking to `~/bin`)

## Configuration

1. Set `$path_to_feed` and `$default_download_dir` in yt-rss.
2. Set up config directory

```
$path_to_feed
├── rsslist
└── ts
```

where rsslist should have the following format:

```
<RSS URL for channel 1> | <Output path for channel n> | <Flags for channel n>
.
.
.
<RSS URL for channel n> | <Output path for channel n> | <Flags for channel n>
```

See an example config [here](./rsslist). 

## Getting Feeds

1. Go to the main page of a channel and get the channel id
   1. Click view page source on the main page
   2. Search for "?channel_id=" to find the id.
2. The RSS feed link is `https://www.youtube.com/feeds/videos.xml?channel_id=<CHANNEL_ID>`

## cron

This script works well with cron. There is no special set up in order to cron this program specifically (outside of the standard cron setup). See [this](https://wiki.archlinux.org/title/cron) for more information about cron. 
