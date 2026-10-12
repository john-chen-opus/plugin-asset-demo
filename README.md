# plugin-asset-demo

Static demo assets for prototyping the AI Producer plugin's caption style picker, served through jsDelivr.

## Layout

```
images/captions/
  thumb/    540x320 PNG, the picker tile crop (4x of the 135x80 design tile)
  full/     1080x1920 PNG, the caption on a black 9:16 frame
  overlay/  1080x1920 PNG, the caption alone on a transparent background
videos/
  caption-styles-demo.mp4         1080x1920, H.264, 8 s, one style per second
  caption-styles-demo-poster.jpg  first frame, 540 px wide
manifest.json                     every asset, keyed by caption style token
```

File names use the caption style tokens: `blur-ladder`, `editorial-stack`, `inverted-stack`, `lead-in-flare`, `pace-adaptive`, `scribble-subtitle`, `solo-word-punch`, `tilt-slam`.

## CDN

Pin a tag so the files never change under a page:

```
https://cdn.jsdelivr.net/gh/john-chen-opus/plugin-asset-demo@v0.1.0/images/captions/thumb/blur-ladder.png
https://cdn.jsdelivr.net/gh/john-chen-opus/plugin-asset-demo@v0.1.0/videos/caption-styles-demo.mp4
```

These are prototype assets, not a supported API. Publish a new tag for any change instead of moving an existing one.
