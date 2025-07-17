# NowCooing
A modern-looking Now Playing overlay for OBS, with Last.fm and Spotify support

This project is based on [OBS-NowPlaying](https://github.com/sorachan/OBS-NowPlaying/#) by **sorachan**.
This is very much a work in progress and I would like to make it more user-friendly in the near future by offering an online version.
Make sure to check out vzsg's fork, [PyNowCooing](https://github.com/vzsg/PyNowCooing), which uses Windows' SystemMediaTransportControl and supports most (if not all) modern media players, including Spotify, Foobar2000, Apple Music and YouTube.

## Functionalities

- Last.fm support
- Overlay automatically resizes based on title name/artist name length

With a medium title:

![Screenshot of the overlay with a short title](/src/screenshots/NowCooing_screenshot_short-title.png?raw=true "Screenshot of the overlay with a short title")

Long title:

![Screenshot of the overlay with a long title](/src/screenshots/NowCooing_screenshot_long-title.png?raw=true "Screenshot of the overlay with a long title")

![Second screenshot of the overlay with a long title](/src/screenshots/NowCooing_screenshot_long-title-2.png?raw=true "Second screenshot of the overlay with a long title")

- When the album cover is unavailable, it is hidden entirely.
- You can define a set of 4 colors which will be used to generate random backgrounds.
  These backgrounds will change on every song!

  ![First screenshot of the overlay with no cover](/src/screenshots/NowCooing_screenshot_no-cover-1.png?raw=true "First screenshot of the overlay with no cover")
  
  ![Second screenshot of the overlay with no cover](/src/screenshots/NowCooing_screenshot_no-cover-2.png?raw=true "Second screenshot of the overlay with no cover")

## Setup
The instructions below are only there if you already know what you're doing, otherwise I would advise waiting for the next update!

1. **Clone or download the repo**
2. **Fill in your credentials:**
   - Open `main.js` and enter your Last.fm or Spotify details as shown in the comments.
3. **Run locally**
   - Serve with any static file server (e.g. `npx http-server .`)
   - Or open `main.html` directly.

## Usage

- Set up as a browser source in OBS (change the URL, other default settings will do)
- Switch between Spotify and Last.fm by setting `musicSource` in `main.js`.


## Releases

### v1.0.0 (2025-06-20)
- Initial release, working locally with Lastfm

