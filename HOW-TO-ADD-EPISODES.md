# How to add an episode to beyondtheprocedurepodcast.com

The page reads every episode from `episodes.json`. You never need to edit the page design.

## 1. Publish the audio with a podcast host
Upload the finished MP3 to a podcast host (for example Spotify for Creators, Buzzsprout or Riverside's hosting).
The host sends the episode to Apple Podcasts and Spotify and gives you share links.
Episode audio files are too large to store on this site directly.

## 2. Update episodes.json
On GitHub, open `episodes.json`, click the pencil icon, and for the episode:

- `"status"`: change `"soon"` to `"live"`
- `"release_date"`: e.g. `"2026-12-01"`
- `"embed_url"`: the Spotify episode link (or your host's embed link). This shows a player on the page.
- `"spotify_url"`, `"apple_url"`, `"youtube_url"`: paste any you have; each becomes a "Listen on" button
- `"audio_url"`: optional direct MP3 link if you have no embed link
- `"cover"`: optional artwork path, e.g. `"assets/episode-2-cover.jpg"` (upload the image into `assets/`)

Keep the quotes and commas exactly as they are. Click **Commit changes**. The site updates within about a minute.

The newest `live` episode is featured at the top automatically.

## 3. Adding Episode 4 and beyond
Copy one episode block (from `{` to `}`), paste it after the last one, add a comma between blocks, and change the number and details.

Or send Computer the links and it will do this for you.
