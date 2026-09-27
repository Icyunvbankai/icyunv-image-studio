# ICYUNV Image Studio

Your own AI image generator. Free, no signup, no blocked prompts.

**Live:** https://icyunvbankai.github.io/icyunv-image-studio/

## What it is

A single-page web app (`index.html` — no build step, no backend) that generates images through [Pollinations.ai](https://pollinations.ai):

- **Free** — no account, no API key, no credits
- **No content blocks** — safety filtering is off by default
- **Private mode** — keeps your generations out of the public feed (on by default)
- **Gallery** — every generation saved in your browser with one-click download
- **Style presets** — tee graphic, graffiti, photoreal, dark fantasy, anime, minimal logo
- **Seed lock** — re-roll variations or lock a seed to reproduce a result

## How it works

The app builds a Pollinations image URL from your prompt and settings:

```
https://image.pollinations.ai/prompt/{prompt}?model=flux&width=1024&height=1024&seed=42&nologo=true&private=true
```

That's the whole backend. Your prompt never touches a server you don't control.

## Develop

Just edit `index.html` and push — GitHub Pages redeploys automatically.

## Ideas for later

- Add a Fal.ai / Replicate key field for FLUX Pro or paid models
- Batch mode: generate 4 variations at once
- Negative prompt field
