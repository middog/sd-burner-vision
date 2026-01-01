# Link & Reference Audit ✅

Date: 2026-01-01

## What I Checked

- **Internal links** (within each Hugo site)
- **Cross-site links** between `playa/`, `sdcap/`, and `sdcolab/`
- **External references** (Burning Man, Gathio, Hugo, Discord)
- **Theme navigation** (header/footer/site switcher)

## Findings (Before Fix)

1. **Root-relative markdown links** like `](/how-we-gather/sdcap-path/)` can break when the site is hosted under a subdirectory (e.g. GitHub Pages `/sd-burner-vision/playa/…`), because `/…` resolves to the domain root.
2. **Cross-site relative links** like `../sdcolab/` can break from nested pages (e.g. `/playa/events/`), because `../` depends on the current page depth.

## Fixes Applied

### ✅ Internal links → `relref`

Converted internal root-relative links to Hugo `relref` shortcodes, e.g.

- Before: `[Events](/events/)`
- After:  `[Events]({< relref "events/_index.md" >})`

This makes internal links stable across subdirectory hosting.

### ✅ Cross-site links → `xsite` shortcode

Added a theme shortcode:

- `{< xsite "playa" >}`
- `{< xsite "sdcap" "grants/" >}`

…and replaced cross-site markdown links accordingly, e.g.

- Before: `[SDCAP](../sdcap/)`
- After:  `[SDCAP]({< xsite "sdcap" >})`

The shortcode pipes the configured cross-site base through Hugo’s `relURL`, so it stays correct regardless of page depth.

### ✅ Theme nav: stable URLs + active state

- Header/footer menu links now use `{ .URL | relURL }`
- Site switcher + Fire Triangle buttons now use `| relURL` for stability
- Added active state styling for the current menu item

### ✨ “Looks better” polish

- Improved `.doc-content` styling: blockquotes, code blocks, tables, images, and link underline/hover.

## Change Summary

- Internal link rewrites (relref): 46
- Cross-site link rewrites (xsite): 42
- Home link rewrites (relref): 1

