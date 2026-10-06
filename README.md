# Borozdov Wire

A theme from the Borozdov collection. Two faces — light **Seaglass**, a deep navy ledger
under cool dawn, and dark **Fathom**, the same ledger in deep sea water. Navy ink on cloud
white, seafoam code, soft layered cards and one signal orange for what stands out.

![Borozdov Wire in light mode](https://raw.githubusercontent.com/borozdov-obsidian-themes/wire/main/screenshots/light.png)

![Borozdov Wire in dark mode](https://raw.githubusercontent.com/borozdov-obsidian-themes/wire/main/screenshots/dark.png)

## Principles

- **Navy is the structure.** Headings, the title, the main button and the open file are
  indigo navy; the text is a cool charcoal, never black.
- **Seafoam means code.** Inline code is seafoam on a seafoam wash and strings in code
  blocks are seafoam; Wire Mono sets code, property names and table headers.
- **Cards that float.** Callouts sit on a soft five-layer shadow, code blocks on a hairline
  with a whisper of shadow; 8px corners everywhere, pills only for tags.
- **One signal orange.** Orange marks a checked task and a peach wash is the highlighter. By
  night seafoam takes over the buttons and sky cyan the links.

## Features

- Light and dark modes, following Settings → Appearance → Base color scheme
- Callouts as floating cards with the title in the type's colour; the plain note on a sky
  wash
- Code blocks as white cards, inline code in seafoam, table headers in small mono capitals
- Tags as mono pills on a sky wash
- Quiet editing: no focus ring around the note, its title or form fields while you type;
  property names read as labels, not boxed fields
- Text colours meet WCAG contrast on both faces
- The phone layout keeps the same colours and shapes
- No `!important`: every rule can be overridden with a CSS snippet

## Installation

**From the community directory, as a variant:** this theme ships inside **Borozdov
Utility**. Install Borozdov Utility under Settings → Appearance → Themes → Manage, then
the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin, and
choose **Wire** under Style Settings → Borozdov Utility → Variant. The variant brings this
theme's palette, type and corners; its own layout, and its embedded font if it has one,
come with the full theme below.

**The full theme, by hand:** download `manifest.json` and `theme.css` from the [latest
release](https://github.com/borozdov-obsidian-themes/wire/releases/latest) into
`<vault>/.obsidian/themes/Borozdov Wire/`, then choose Borozdov Wire under Settings →
Appearance → Themes.

## Font

Wire Mono is embedded in `theme.css` as base64 WOFF2 under the SIL Open Font License 1.1 —
see [`fonts/OFL.txt`](fonts/OFL.txt). It is a Latin and Cyrillic subset of Source Code Pro
(© 2010, 2012 Adobe Systems Incorporated), renamed because a modified copy may not use the
original's Reserved Font Name. One weight, for code, inline code, property names and table
headers.

## License

MIT — see [LICENSE](LICENSE).

---

**По-русски.** Тема из коллекции Borozdov. Два лика: светлый «Морское стекло» — тёмно-синий
гроссбух в прохладном рассвете, и тёмный «Глубина» — тот же гроссбух в глубокой морской
воде. Тёмно-синие чернила на облачно-белом, код цвета морской пены (моноширинный Wire Mono
на основе Source Code Pro), мягкие парящие карточки и один сигнальный оранжевый.
В каталоге тема живёт вариантом Borozdov Utility: установите Borozdov Utility и плагин Style Settings, затем выберите Wire в Style Settings → Borozdov Utility → Variant. Целиком, со своей вёрсткой, тема ставится вручную из последнего релиза репозитория.
