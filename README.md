# web.kartoffel

Minimal interactive portfolio website for **web.kartoffel**.

The site combines generative visuals, soft-matter-inspired nematic fields, and small browser-based audio interactions. It is built as a single static HTML file and is designed to be hosted with GitHub Pages.

## Live site

Once GitHub Pages is enabled, the site will be available at:

```text
https://YOUR-GITHUB-USERNAME.github.io/REPOSITORY-NAME/
```

or, if this repository is named `YOUR-GITHUB-USERNAME.github.io`:

```text
https://YOUR-GITHUB-USERNAME.github.io/
```

## Concept

The page is structured around three connected fields:

- **Sound** — low-frequency rhythms, minimal and hypnotic techno
- **Visuals** — reactive dynamic visuals, projection-related organic forms and noise textures
- **Matter** — soft active matter, nematic fields, and physics-inspired interaction

The design is intentionally minimal: dark background, sparse typography, animated nematic directors, and scroll-dependent section states.

## Features

- Single-file static website
- No build system
- No external JavaScript libraries
- No tracking or analytics
- No external fonts
- GitHub Pages compatible
- Animated nematic director field using `<canvas>`
- Mouse-reactive local vortex interaction
- Section-dependent visual behavior
- Synthetic interaction point in the matter section
- Browser-generated audio in the sound section using the Web Audio API
- Audio starts only after user interaction, following browser autoplay restrictions

## Structure

```text
.
├── index.html
└── README.md
```

The entire website is contained in `index.html`.

## Sections

### Location

Introductory state showing the project location as coordinates.

### Sound

Links to SoundCloud and activates browser-generated sound interaction when hovering over the nematic field.

### Visuals

Links to Instagram and changes the nematic rendering style with thicker, brighter, green-shifted director lines.

### Matter

Links to GitHub and introduces a synthetic moving interaction point that affects the nematic field.

## Deployment with GitHub Pages

1. Push this repository to GitHub.
2. Open the repository on GitHub.
3. Go to:

```text
Settings → Pages
```

4. Under **Build and deployment**, select:

```text
Source: Deploy from a branch
Branch: main
Folder: /root
```

5. Save the settings.
6. Wait until GitHub Pages finishes deployment.

The website should become available after a short delay.

## Local preview

You can open `index.html` directly in a browser.

For a more reliable local preview, start a small local server:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Audio behavior

The sound interaction uses the browser Web Audio API.

Because browsers block autoplaying sound, audio only starts after the first user gesture, such as:

- click
- tap
- key press

The sound is only active in the sound section and is stopped after inactivity or when the page loses focus.

## Privacy

This site is static and does not include:

- analytics
- cookies
- backend server code
- forms
- database connections
- API keys
- third-party embedded players

External links point to SoundCloud, Instagram, and GitHub. Those services may process data once visitors follow the links.

## Public repository note

Before making the repository public, check that it contains only files intended for publication.

The current intended public files are:

```text
index.html
README.md
```
