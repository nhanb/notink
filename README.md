Experiments for a web-based eink-friendly manga reader.
Tested on an Onyx Boox Nova 2.

Demo: https://junk.imnhan.com/boox-manga.mp4

The gist:

- assumes chrome browser on android.
- `refreshFullscreen()` forces fullscreen.
- to avoid ghosting: emulates full e-ink refresh by first rendering a negative
  using `filter: invert(1)`, waiting for a few miliseconds (must be long enough
  for the e-ink screen to pick up), then rendering with actual correct color.


Sample images taken from [mangadex](https://mangadex.org/chapter/850141).
