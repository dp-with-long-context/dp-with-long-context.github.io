# Training and Evaluating Diffusion Policies with Long Context Lengths

Project website for the paper *Training and Evaluating Diffusion Policies with Long Context Lengths*.

🌐 **Live site:** https://training-long-context-dp.github.io/

## Authors

Abhinav Agarwal\*, Adam Wei†, Taylan Kargin†, Michael Zeng, Cole Becker,
Arif Kerem Dayı, Pablo Parrilo, Asuman Ozdaglar, Russ Tedrake — MIT

\* Corresponding author · † Equal contribution

## Structure

| File | Purpose |
| --- | --- |
| `index.html` | Single-page project site |
| `style.css` | Styling |
| `paper.pdf` | Paper PDF |
| `.nojekyll` | Tells GitHub Pages to serve files as-is (no Jekyll) |

## Local preview

It's a static site — just open `index.html`, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

Hosted on GitHub Pages from the `main` branch (root). Pushing to `main` redeploys automatically.
