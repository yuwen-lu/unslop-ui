# unslop-ui

A coding agent skill that enforces clean UI/UX design and prevents common AI-generated anti-patterns when writing frontend code.

Based on this post: [Anti-Slop UI Rules for AI Code Generation](https://x.com/yuwen_lu_/status/2041187936738447565)

## What it prevents

- Homogenous color goo (everything the same hue at different saturations)
- Icon-in-rounded-square filler
- Emojis as visual assets
- Default serif hero headlines (Instrument Serif, Playfair Display, etc.)
- Gratuitous glassmorphism
- Gradient and colored shadow overuse
- Cards nested in cards nested in cards
- Slow entrance animations on everything

## What it encourages

Solid neutral backgrounds, clean sans-serif typography, whitespace as a design tool, flat minimal icons only where they aid understanding, and nothing decorative that doesn't earn its place.

Reference sites for good taste: Linear, Vercel, Stripe, Raycast, Arc Browser, Cursor.

## Install

### Claude Code (marketplace)

```sh
claude /plugin marketplace add yuwen-lu/unslop-ui
claude /plugin install unslop-ui@unslop-ui
```

### Claude Code (manual)

Copy the `skills/unslop-ui/` directory into your project:

```sh
cp -r skills/unslop-ui/ your-project/.claude/skills/unslop-ui/
```

Or for user-level (all projects):

```sh
cp -r skills/unslop-ui/ ~/.claude/skills/unslop-ui/
```

### Cursor

```sh
cp -r skills/unslop-ui/ your-project/.cursor/skills/unslop-ui/
```

### OpenAI Codex

```sh
cp -r skills/unslop-ui/ your-project/.agents/skills/unslop-ui/
```

### Gemini CLI

```sh
cp -r skills/unslop-ui/ your-project/.gemini/skills/unslop-ui/
```

### Trae

```sh
cp -r skills/unslop-ui/ your-project/.trae/skills/unslop-ui/
```

### Kiro

```sh
cp -r skills/unslop-ui/ your-project/.kiro/skills/unslop-ui/
```

## Examples

The `examples/` directory contains reference screenshots showing good and bad design patterns:

| File | Shows |
|------|-------|
| `bad-homogenous-color.png` | Colors mushed together into one blob |
| `bad-icon-rounded-square.png` | Decorative icons in colored boxes |
| `bad-glassmorphism.png` | Frosted glass cards over gradients |
| `bad-gradient-shadow.png` | Gradients and colored shadows everywhere |
| `bad-button-shadow.png` | Glowing colored button shadows |
| `good-cursor-color.png` | Clean color usage (Cursor) |
| `bad-excessive-hero-serif.png` | Serif typography overuse |

## License

[MIT](LICENSE)
