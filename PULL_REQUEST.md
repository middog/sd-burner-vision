# Pull Request: Comprehensive Content Update + How We Gather Section 🐾🔥

## Summary

This PR delivers a complete content refresh across all three sites (PLAYA, SDCAP, SDCoLab) with consistent ELIH-5 (Explain Like I'm a Hippie-5) styling, Fire Triangle theming, and the new "How We Gather" onboarding section.

## What Changed

### ✨ New Section: `/how-we-gather/` (PLAYA)

A comprehensive onboarding section explaining how to engage with the community:

```
sites/playa/content/how-we-gather/
├── _index.md              # Fire Triangle intro, three paths
├── new-pup.md             # Quick-start orientation for newcomers
├── sdcap-path/
│   ├── _index.md          # How to work with the nonprofit (🔵 Oxygen)
│   └── first-ask.md       # Making your first request to SDCAP
├── sdcolab-path/
│   ├── _index.md          # How to work with the makerspace (🟡 Fuel)
│   └── first-build.md     # Making your first thing at CoLab
└── magic-of-3s/
    ├── _index.md          # Philosophy: Fire Triangle, 3S, Growth Path
    ├── yes-and.md         # The "Yes... And!" collaborative culture
    └── fire-party.md      # Understanding Fire Party working sessions
```

### 🔄 Updated: All Existing Content

Every page across all three sites has been updated with:

- Warmer, more welcoming tone
- Fire Triangle context (Heat/Oxygen/Fuel)
- Cross-references between sites
- Consistent formatting and structure
- Pack/dog metaphors where appropriate 🐕

**PLAYA Site Updates:**
- `about/_index.md` — Fire Triangle intro, cross-links
- `community/_index.md` — Pack theme, Discord guidance
- `culture/_index.md` — Expanded 10 Principles table
- `events/_index.md` — Event types table, hosting guidance
- `get-started/_index.md` — Growth Path framework

**SDCAP Site Updates:**
- `about/_index.md` — Oxygen framing, philosophy
- `governance/_index.md` — 3S framework, Yes...And! promise
- `grants/_index.md` — Warmer tone, clear process
- `events/_index.md` — YOUtopia details, cross-links
- `get-started/_index.md` — Full engagement options

**SDCoLab Site Updates:**
- `about/_index.md` — Fuel framing, costs table
- `access/_index.md` — Clear progression path
- `classes/_index.md` — Teaching as gifting
- `space/_index.md` — Pack Code, safety
- `projects/_index.md` — Growth Path, residency

### 🔗 Fixed: Cross-Site Links

All cross-site links now use relative paths (`../sdcap/`, `../sdcolab/`) to work correctly with the GitHub Pages multi-site deployment structure.

## Key Concepts Throughout

### Fire Triangle 🔥
- **Heat (🔴)** = Community, people, energy → PLAYA
- **Oxygen (🔵)** = Enablement, info, process → SDCAP  
- **Fuel (🟡)** = Resources, tools, space → SDCoLab

### Growth Path 📈
```
PROJECT → PARTY → PRACTICE
```

### 3S Framework 🔄
```
SENSE → STABILIZE → STRENGTHEN
```

### Yes... And! 🎭
Never just "no" — acknowledge, explain, enable, connect, offer.

## 🐕 Easter Eggs

- Pack/dog metaphors throughout
- "Good dog" encouragements
- Fetch-stick philosophy for 3S
- Paw prints (🐾) as section markers
- Three-dog emoji clusters (🐕🐕🐕)
- "New Pup Orientation" page title
- "Sniffing around" for the sensing stage

---

## Commit Message

```
feat: comprehensive content update with ELIH-5 styling

- Add How We Gather section (9 new pages for onboarding)
- Update all existing pages with Fire Triangle theming
- Apply consistent warm tone across all three sites
- Fix cross-site links for GitHub Pages deployment
- Add Growth Path and 3S framework documentation
- Include Yes...And! culture explanation

Content derived from sdcap-governance repo patterns.
Pack metaphors and dog easter eggs included. 🐾

🔥 Three heads, one fire. Good dog.
```

---

## Files Changed

### New Files (9)
- `sites/playa/content/how-we-gather/_index.md`
- `sites/playa/content/how-we-gather/new-pup.md`
- `sites/playa/content/how-we-gather/sdcap-path/_index.md`
- `sites/playa/content/how-we-gather/sdcap-path/first-ask.md`
- `sites/playa/content/how-we-gather/sdcolab-path/_index.md`
- `sites/playa/content/how-we-gather/sdcolab-path/first-build.md`
- `sites/playa/content/how-we-gather/magic-of-3s/_index.md`
- `sites/playa/content/how-we-gather/magic-of-3s/yes-and.md`
- `sites/playa/content/how-we-gather/magic-of-3s/fire-party.md`

### Modified Files (15)
- `sites/playa/content/about/_index.md`
- `sites/playa/content/community/_index.md`
- `sites/playa/content/culture/_index.md`
- `sites/playa/content/events/_index.md`
- `sites/playa/content/get-started/_index.md`
- `sites/sdcap/content/about/_index.md`
- `sites/sdcap/content/governance/_index.md`
- `sites/sdcap/content/grants/_index.md`
- `sites/sdcap/content/events/_index.md`
- `sites/sdcap/content/get-started/_index.md`
- `sites/sdcolab/content/about/_index.md`
- `sites/sdcolab/content/access/_index.md`
- `sites/sdcolab/content/classes/_index.md`
- `sites/sdcolab/content/space/_index.md`
- `sites/sdcolab/content/projects/_index.md`

---

## Checklist

- [x] All content uses consistent ELIH-5 tone
- [x] Fire Triangle correctly represented across sites
- [x] 3S and Growth Path frameworks explained
- [x] Cross-site links use relative paths (`../`)
- [x] Internal links verified
- [x] Hugo frontmatter complete with weights
- [x] Dog easter eggs included 🐕
- [x] No gatekeeping language
- [x] Yes... And! philosophy embedded

---

*Three heads, one fire, good dog.* 🐕🔥
