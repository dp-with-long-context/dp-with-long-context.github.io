# Video assets

Drop the task rollout clips here with these exact filenames and they'll appear
automatically (the page already points at them; until they exist a placeholder
poster is shown):

| Filename | Task |
| --- | --- |
| `push-and-return.mp4` | Push-and-Return |
| `grasp-and-return.mp4` | Grasp-and-Return |
| `marshmallows.mp4` | Marshmallows (hardware) |

## Recommended encoding

Short looping clips, muted, web-optimized H.264 MP4. Keep each well under ~10 MB
so the page stays fast. Example with ffmpeg:

```bash
ffmpeg -i raw.mov -an -vf "scale=640:-2,fps=30" \
  -c:v libx264 -crf 26 -movflags +faststart push-and-return.mp4
```

- `-an` strips audio (clips autoplay muted anyway)
- `-movflags +faststart` lets playback begin before the full file downloads

Optional: add a `<video poster>` still by saving a frame as e.g.
`push-and-return.jpg` and pointing the `poster` attribute at it in `index.html`.
