# import JSON Takeout in google-chrome database

I use google-chrome because vivaldi don't watch chromium config.

You maybe use this program for chromium, but this has no guarantees. 

# Init settings

I deleted folder with config google-chrome

```bash
rm -r ~/.config/google-chrome
```

Then I visit the page, thereby creating a small story

copy History file to dist_folder

```bash
cp ~/.config/google-chrome/Default/History ~/Downloads/History.db
```

This filse sqlite database

As a result, I got that there are empty and non-empty tables

# DB tables

## empty 

- cluster_keywords
- cluster_visit_duplicates
- clusters
- clusters_and_visits
- downloads
- downloads_slices
- downloads_url_chains
- history_sync_metadata
- segment_usage
- segments
- visit_source

## Not empy

- content_annotations
- context_annotations
- keyword_search_terms
- meta
- sqlite_sequence
- urls
- visited_links
- visits

# Step 1

Use this tables

- sqlite_sequence
- urls
- visited_links
- visits
