# YT-RSS
## RSS-based local syncing for youtube subscriptions

WIP

<details>
 <summary><strong>Table of Contents</strong> (click to expand)</summary>

- [Setup](#-setup)
- [Configuration](#-configuration)

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
