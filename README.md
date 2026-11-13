# Nuvio Comprehensive Badges (image-backed)

This pack contains a Fusion/Nuvio `badges.json` and one transparent PNG label asset per filter.

## Install

1. Create a **public GitHub repository** named `nuvio-comprehensive-badges`.
2. Upload the contents of this folder (`badges.json` and the `badges/` folder) to the repository root.
3. In `badges.json`, replace every occurrence of `YOUR-GITHUB-USERNAME` with your GitHub username. (Use Find & Replace.)
4. Commit the changes.
5. Open the raw `badges.json` file in GitHub and copy its Raw URL.
6. Import that Raw URL in Nuvio → Settings → Streams → Fusion Badge URLs.

The JSON references the PNGs in the same repository at `/badges/<filter-id>.png`.

## Important test note

Nuvio matches the stream title returned by the add-on, not the movie's catalogue title. A catalogue title such as `Mirzapur The Movie` contains no source/resolution token, so it cannot match WEB-DL, HDTC, 1080p, etc. Use the full stream result title/filename shown in the source picker for testing.

This pack's badges are image-backed; it does not rely on undocumented empty-image fallback behaviour.
