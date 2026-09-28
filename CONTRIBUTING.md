# Contributing

Issues and pull requests are welcome.

## Reporting a problem

Open an issue with your Obsidian version, operating system, light or dark mode, and a
screenshot. If a plugin or a CSS snippet is involved, name it.

## Working on the theme

1. Clone the repository and link it into a test vault:
   `ln -s "$PWD" "<vault>/.obsidian/themes/Borozdov Wire"`
2. Choose Borozdov Wire under Settings → Appearance → Themes. After editing
   `theme.css`, run **Reload app without saving** from the command palette.
3. Lint with the rules the community directory applies: `npm install`, then
   `npm run lint`.
4. After a visible change, rerender the screenshots: `npm run screenshots`. It needs
   macOS with Obsidian and Google Chrome installed, and Pillow for Python. The theme is
   laid over Obsidian's own stylesheet, extracted from the installed app at run time;
   `screenshots/` is rewritten.

House rules:

- Obsidian's CSS variables first, plain selectors after; no `!important`, no `:has()`.
- Colors come from the palette in section 1 of `theme.css`; nothing else holds a color
  literal.
- Cool cloud paper, navy ink for headings and the main button, seafoam for code and data,
  one signal orange for the checked task and a peach wash for the highlighter; cards float
  on a soft layered shadow. The only embedded font is Wire Mono, a subset of Source Code
  Pro (code, inline code, property names and table headers): `fonts/*.woff2` are written
  into `theme.css` by `npm run fonts`.
- The release ships `dist/theme.css` from `npm run build`: the same file without
  comments. The build fails on any lint problem.

## Releasing

1. Bump `version` in `manifest.json` and add the same version to `versions.json`, mapped
   to the minimum Obsidian version it needs.
2. Commit, then push an annotated tag named with the bare version:
   `git tag -a 1.0.1 -m "1.0.1: …"` and `git push origin 1.0.1`.
3. The release workflow lints and builds the theme, checks the tag against
   `manifest.json` and `versions.json`, attests `manifest.json` and `dist/theme.css`, and
   publishes the GitHub release with both files attached. The tag message becomes the
   release notes.
4. Never delete a published release: the community directory keeps its own record of
   every version it has reviewed.
