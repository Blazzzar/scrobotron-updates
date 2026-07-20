# scrobotron-updates

The public update channel ("shelf") for the **Scrobotron** WordPress
plugin — served by GitHub Pages at
`https://blazzzar.github.io/scrobotron-updates/`.

Sites running Scrobotron read `scrobotron.json` (which versions exist on
the `stable` and `beta` tracks, plus retained releases for one-click
rollback) and download the built zips from `zips/`.

Nothing sensitive lives here: the zips contain only the plugin code — no
GIF libraries, no passkey. The source, history, and docs live in the
private [`scrobotron`](https://github.com/Blazzzar/scrobotron) repo.

**Don't edit this repo by hand** — `bin/publish-channel.sh` in the code
repo writes the manifest, adds the new zip, trims retention to the last
5 releases, and prunes unreferenced zips.
