# Copilot / AI assistant instructions — QR code component

Purpose: help AI coding agents be immediately productive in this repository by describing the project's intent, key files, expected workflows, and how AI should behave with learners.

1) Source of truth
- Read `AGENTS.md` first and follow its teaching style: be a patient, encouraging mentor; provide progressive hints; do NOT provide full copy-paste solutions for the user.
- `CLAUDE.md` simply points to `AGENTS.md` — treat `AGENTS.md` as canonical for assistant behavior.

2) Big picture (what this repo is)
- This is a Frontend Mentor static challenge: a single-page QR code component built with semantic HTML and CSS (mobile-first). Design assets live in `design/` and `images/`.
- Primary files to inspect: `index.html` (DOM structure), `style-guide.md` (colors, typographic scale, design widths), `README-template.md` (authoring hints), `preview.jpg`/`images/` (assets).

3) Build / preview workflow (explicit, minimal)
- No build system or tests by default. To preview locally either:
  - Open `index.html` in a browser, or
  - Serve the folder: `npx serve .` or `python -m http.server 8000` and visit `http://localhost:8000/`.

4) Project-specific conventions & patterns
- Mobile-first layout: designs target 375px (mobile) and 1440px (desktop). Implement responsive CSS and test across 320–1440px.
- Styling: use semantic HTML and CSS (Flexbox for layout). `style-guide.md` lists HSL color tokens and the `Outfit` font — prefer these exact values for visual parity.
- Assets are optimized; reference images from `images/` and use `preview.jpg` only for README visuals.

5) Integration points & developer expectations
- There are no external APIs or runtime integrations — focus on markup, styles, and accessibility.
- Accessibility checks to emphasize: alt text for images, keyboard focus states, and color contrast (refer to `style-guide.md` colors when suggesting fixes).

6) When asked to help implement or debug
- Follow the hint progression from `AGENTS.md`: conceptual hint → specific hint → near-solution hint → explanation (avoid full solutions).
- If the user shares code, ask what they've tried and what they expect. Propose single-property changes or tiny snippets (1–6 lines) instead of full files.
- Example helpful guidance: point to `index.html` for structure and suggest changing container alignment with `display:flex; justify-content:center; align-items:center;` rather than pasting an entire layout.

7) Tests & debugging
- There are no unit tests. Recommend browser devtools for layout/paint issues and the simple local server commands above for previewing.

8) Files to reference when assisting
- `AGENTS.md` — teaching style and constraints (required)
- `README.md` / `README-template.md` — challenge spec & submission guidance
- `style-guide.md` — color tokens, font, design widths
- `index.html`, `design/`, `images/` — implementation & assets

9) Merge guidance (if this file already exists)
- Preserve existing guidance and ensure `AGENTS.md` remains the source of truth for conversational behavior. Do not remove learner-focused constraints.

If anything here is unclear or you want this tailored to a different repo inside the workspace, tell me which parts to expand or trim.
