# Project Koios Color Palette
The Project Koios palette should feel like a technical notebook, old engineering manual, academic archive, or Unix documentation.  
  
It should not feel like an AI startup, edtech platform, creator brand, finance newsletter, or corporate consulting deck.  
  
Use the core palette for most of the site. Use the secondary palette only when the content needs contrast, status, code emphasis, or a different technical register.
## Core Palette

<table>
  <thead>
    <tr>
      <th>Role</th>
      <th>Name</th>
      <th>Hex</th>
      <th>Swatch</th>
      <th>Use</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Background</td>
      <td>Paper</td>
      <td><code>#F4F1E8</code></td>
      <td><div style="width:80px;height:32px;background:#F4F1E8;border:1px solid #999;"></div></td>
      <td>Main page background</td>
    </tr>
    <tr>
      <td>Text</td>
      <td>Ink</td>
      <td><code>#171717</code></td>
      <td><div style="width:80px;height:32px;background:#171717;border:1px solid #999;"></div></td>
      <td>Primary text</td>
    </tr>
    <tr>
      <td>Muted Text</td>
      <td>Graphite</td>
      <td><code>#5F6368</code></td>
      <td><div style="width:80px;height:32px;background:#5F6368;border:1px solid #999;"></div></td>
      <td>Secondary text, captions</td>
    </tr>
    <tr>
      <td>Border</td>
      <td>Rule Line</td>
      <td><code>#D8D1C4</code></td>
      <td><div style="width:80px;height:32px;background:#D8D1C4;border:1px solid #999;"></div></td>
      <td>Dividers, cards, subtle outlines</td>
    </tr>
    <tr>
      <td>Panel</td>
      <td>Warm Panel</td>
      <td><code>#FFF9ED</code></td>
      <td><div style="width:80px;height:32px;background:#FFF9ED;border:1px solid #999;"></div></td>
      <td>Cards, callout backgrounds</td>
    </tr>
    <tr>
      <td>Accent</td>
      <td>Deep Technical Blue</td>
      <td><code>#1F4E5F</code></td>
      <td><div style="width:80px;height:32px;background:#1F4E5F;border:1px solid #999;"></div></td>
      <td>Links, section markers, small emphasis</td>
    </tr>
  </tbody>
</table>

## Secondary Palette

<table>
  <thead>
    <tr>
      <th>Role</th>
      <th>Name</th>
      <th>Hex</th>
      <th>Swatch</th>
      <th>Use</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Dark Background</td>
      <td>Charcoal</td>
      <td><code>#111418</code></td>
      <td><div style="width:80px;height:32px;background:#111418;border:1px solid #999;"></div></td>
      <td>Optional dark sections</td>
    </tr>
    <tr>
      <td>Dark Panel</td>
      <td>Slate</td>
      <td><code>#1B2229</code></td>
      <td><div style="width:80px;height:32px;background:#1B2229;border:1px solid #999;"></div></td>
      <td>Dark cards or code regions</td>
    </tr>
    <tr>
      <td>Code Background</td>
      <td>Terminal Black</td>
      <td><code>#0B0D10</code></td>
      <td><div style="width:80px;height:32px;background:#0B0D10;border:1px solid #999;"></div></td>
      <td>Code blocks</td>
    </tr>
    <tr>
      <td>Code Text</td>
      <td>Pale Blue</td>
      <td><code>#D6E4FF</code></td>
      <td><div style="width:80px;height:32px;background:#D6E4FF;border:1px solid #999;"></div></td>
      <td>Code text</td>
    </tr>
    <tr>
      <td>Warning Accent</td>
      <td>Oxide</td>
      <td><code>#9A4A2F</code></td>
      <td><div style="width:80px;height:32px;background:#9A4A2F;border:1px solid #999;"></div></td>
      <td>Rare warning or emphasis</td>
    </tr>
    <tr>
      <td>Success Accent</td>
      <td>Muted Green</td>
      <td><code>#3E6B50</code></td>
      <td><div style="width:80px;height:32px;background:#3E6B50;border:1px solid #999;"></div></td>
      <td>Rare positive/status emphasis</td>
    </tr>
  </tbody>
</table>

## Typography
## Typography

Typography should be Obsidian-readable first.

Most Project Koios material begins as Markdown notes, lecture drafts, research notes, or working documents. The source files should remain readable in Obsidian, VS Code, GitHub, and Quarto without depending on custom fonts or website-specific styling.

The website can improve the presentation, but it should not make the source format ugly or fragile.

## Typography

Typography should be Obsidian-readable first.

Most Project Koios material begins as Markdown notes, lecture drafts, research notes, or working documents. The source files should remain readable in Obsidian, VS Code, GitHub, and Quarto without depending on custom fonts or website-specific styling.

The website can improve the presentation, but it should not make the source format ugly or fragile.

| Type | Primary Use | Notes |
|---|---|---|
| Sans-serif | Default body text, notes, UI, navigation, metadata, labels | Best default because it feels closest to Obsidian, GitHub, and technical documentation. |
| Serif | Optional long-form essays and polished article pages | Use selectively when a page should feel more like a published essay. Do not make it the default. |
| Monospace | Code, file paths, shell commands, constants, tags, short technical identifiers | Use only when monospace has a job. Do not use it as decoration. |

## Sample Technical Note Rendering

### Finite-Difference Hamiltonian

This is normal prose. It should feel like a readable technical note, not a marketing page.

The one-dimensional Hamiltonian is
$$
\hat{H}
=
-\frac{\hbar^2}{2m}
\frac{\mathrm{d}^2}{\mathrm{d}x^2}
+
V(x).
$$

After discretization, the operator becomes a matrix eigenvalue problem,

$$
H\psi = E\psi.
$$

Use `np.linalg.eigh(H)` for dense Hermitian matrices. For larger sparse systems, use `scipy.sparse.linalg.eigsh`.

The implementation might live in:

```text
src/projectkoios/quantum/hamiltonian.py
```

A note can carry metadata:

```yaml
type: working-note
status: draft
area: computational-physics
updated: 2026-05-17
```

The point is not to hide the math. The point is to make the structure readable.

## Font Variables

```css
:root {
  --font-body: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  --font-reading: ui-serif, Georgia, Cambria, "Times New Roman", Times, serif;
  --font-mono: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace;
}
```

| Type | Primary Use | Notes |
|---|---|---|
| Sans-serif | Default body text, notes, UI, navigation, metadata, labels | Best default because it feels closest to Obsidian, GitHub, and technical documentation. |
| Serif | Optional long-form essays and polished article pages | Use selectively when a page should feel more like a published essay. Do not make it the default. |
| Monospace | Code, file paths, shell commands, constants, tags, short technical identifiers | Use only when monospace has a job. Do not use it as decoration. |

## Font Variables

```css
:root {
  --font-body: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  --font-reading: ui-serif, Georgia, Cambria, "Times New Roman", Times, serif;
  --font-mono: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace;
}
```

## Mathematics

Math  is treated as normal technical prose, not decoration.
- support inline math with `$...$`
- Display math with `$$...$$`. This matches my Obsidian, and workflow.
- Display equations should be visually quiet. Use spacing, Most equations do not need boxes, shadows, gradients, or special treatment.

### Semantic blocks
The block should explain why the equation matters. It should not exist just to make the page look designed.
- Definition
- Model
- Assumption
- Result
- Derivation Step


Math blocks must remain horizontally scrollable on small screens. Broken equations on mobile are unacceptable.

The preferred style is:

- readable
- copyable
- minimally styled
- compatible with Markdown/Quarto sources
- consistent with technical notes and textbooks

The math should look like it belongs in a serious set of notes, not a product landing page.