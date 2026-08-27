# GitHub Profile System Map Design

## Goal

Refresh the GitHub profile README and its system map so the profile communicates the zmzai product matrix as a coherent product system rather than a list of repositories. The map should use the current `@zmzai/theme` visual language and remain readable when rendered by GitHub.

## Direction

Use a sharp editorial composition based on the current theme:

- pure white background;
- near-black ink and quiet gray supporting text;
- fluorescent green accent for active states, key labels, and the brand line;
- MiSans / Noto Serif SC / JetBrains Mono style hierarchy;
- 2px-level sharp geometry and restrained rules;
- no gradients, decorative illustrations, or dense technical arrows.

## Map Composition

The SVG will have four visual zones:

1. Header: `ZMZAI.CLOUD`, a short Chinese descriptor, and the profile's one-line positioning.
2. Product matrix: six product nodes using the existing `牧 / z / m / h / a / i` sequence. Each node shows name, domain, state, and one concise responsibility.
3. System spine: one centered statement showing the primary capability chain: Agent orchestration → Relay model plane → Sandbox / local client execution.
4. Shared foundation: Auth, MongoDB, Bridge + Client, OpenSandbox, and shared packages, shown as a quiet base layer rather than peer products.

The graphic will prioritize the product matrix and the Agent execution spine. Arena and Muzhi remain represented as product-line context, while the detailed repository lists remain in README text for accessibility and linkability.

## README Changes

- Keep the opening brand, links, and image.
- Replace the long duplicated product tables with a short positioning paragraph and a compact "Now / Building" list.
- Add a concise "How the system works" section below the image, describing the Agent → Relay → execution path in plain language.
- Keep repository links in text so the profile remains navigable without reading the SVG.
- Preserve the closing brand line and email contact.

## Compatibility and Verification

- Keep the SVG self-contained with no external font, image, or JavaScript dependency.
- Use explicit `viewBox`, accessible `title`, and `desc`.
- Use only ASCII in SVG attributes and source comments where practical; visible Chinese copy remains because it is part of the profile identity.
- Inspect the rendered SVG dimensions and validate that all text stays inside the viewBox.
- Run a Markdown/SVG reference check and inspect the final diff for unrelated changes.
