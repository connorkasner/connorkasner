# connor kasner

personal site: sounds, art, architecture, events, posts.
plain html, css and javascript. no build step.

## files
- `index.html`: the whole site (edit releases, posts and links in the script near the bottom)
- `audio/`: one folder per release, with the mp3s that play on the site

## add a track
1. put an mp3 in the release's folder, like `audio/copenhagen/`
2. in `index.html`, find `var releases=` and add the file name (no extension) to that release's `tracks`

## add a release
1. make a new folder in `audio/` and put the mp3s in it
2. add a line to `var releases=` with its name, year, `tracks`, and `dir` (like `audio/akron/`)

wav files are ignored by git (they are too big for github). convert to mp3 before adding.

## open it locally
open the folder in vs code, install the "live server" extension, right click `index.html` and choose "open with live server".

## publish with github pages
1. push this folder to a github repo
2. repo settings > pages > deploy from branch `main`, folder `/ (root)`
3. add your domain under pages > custom domain, then set the dns records at your domain registrar as github describes
