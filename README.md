# 🔥 SD Burner Vision

**Three sites. One fire. Zero gatekeeping.**

A demo/prototype for the San Diego Burning Man community web ecosystem.

## Live Demo

- **Landing:** https://middog.github.io/sd-burner-vision/
- **PLAYA:** https://middog.github.io/sd-burner-vision/playa/
- **SDCAP:** https://middog.github.io/sd-burner-vision/sdcap/
- **SDCOLAB:** https://middog.github.io/sd-burner-vision/sdcolab/

## The Fire Triangle

| Site | Element | Purpose |
|------|---------|---------|
| **PLAYA** | 🔴 Heat | Culture, events, community onboarding |
| **SDCAP** | 🔵 Oxygen | Grants, governance, coordination |
| **SDCOLAB** | 🟡 Fuel | Makerspace, tools, resources |

## Quick Start

```bash
# Clone
git clone https://github.com/middog/sd-burner-vision.git
cd sd-burner-vision

# Run locally (requires Hugo)
./scripts/dev.sh

# Sites run at:
# http://localhost:1313 (PLAYA)
# http://localhost:1314 (SDCAP)
# http://localhost:1315 (SDCOLAB)
```

## Linking Conventions

To keep links working when these sites are hosted under a subdirectory (e.g. GitHub Pages), this repo uses:

- **Internal links (within a site):** Hugo `relref`  
  Example: `[Events]({{< relref "events/_index.md" >}})`

- **Cross-site links (between sites):** `xsite` shortcode (defined in the theme)  
  Example: `[Apply for Grants]({{< xsite "sdcap" "grants/" >}})`


## Deployment

Push to `main` branch → GitHub Actions builds → GitHub Pages deploys automatically.

## Structure

```
├── sites/
│   ├── playa/      # Heat - Community site
│   ├── sdcap/      # Oxygen - Governance site
│   └── sdcolab/    # Fuel - Makerspace site
├── themes/
│   └── cerberus/   # Shared tripartite theme
└── .github/
    └── workflows/  # Auto-deploy to GitHub Pages
```

---

*Three heads. One fire. Let's burn.* 🐕🦮🐕‍🦺🔥
