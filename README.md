# bsky-dl
Download videos and extract json from Bluesky posts. Requires ffmpeg.

`bsky-dl [post_url] [download_path] [options]`

OPTIONS:
    --m3u8: download m3u8 video rather than blob
    --json: print the getPostThread JSON to file
    --replies: include replies and parents in JSON

The file download path uses the following hierarchy:
    1. Path specified in command
    2. default_dir specified in script
    3. Current working directory

Works with both python and bash. Download the bsky-dl file and run `python bsky-dl` or `./bsky-dl`. Or put the file in `~/.local/bin` (or anywhere else in your $PATH) and run `bsky-dl`.
