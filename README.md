# Beacon demo (publisher walkthrough)

Static site, no build step, no backend.

## Files
- `index.html`: the four-step demo (Enrich, Derive, Discover, Apply)
- `portal.html`: reader-portal mockup used in step 3 (Discover)
- `article-graph.html`: article explorer opened from step 4
- `beacon-logo.svg`, `TNQTech-Logo.svg`: logos

## Live dependency
Steps 1 and 3 embed the live Beacon app at `https://beacon-scmy.onrender.com/`.
The free host sleeps when idle, so open it once shortly before a demo.
Change the URL in `CONFIG.beaconUrl` inside `index.html` if the host changes.

## Run locally
    python3 -m http.server 8080
Then open http://localhost:8080/

## Deploy
Upload the whole folder as-is to any static host (GitHub Pages, Netlify, S3).
Keep all files in the same folder: `index.html` loads the others by relative path.

## Content
All abstracts, entities and session summaries are real outputs. Step 1's passage and tags, and step 4's product mock-ups, are illustrative samples and are labelled as such on screen.
