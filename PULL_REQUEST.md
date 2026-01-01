# Pull Request: Complete Content Update with Fixed Links 🐾🔥

## Summary

Complete content refresh with ELIH-5 styling, Fire Triangle theming, and **verified cross-site links**.

## Link Structure (VERIFIED)

```
/sd-burner-vision/
├── playa/           ← PLAYA content lives here
│   ├── how-we-gather/
│   ├── culture/
│   ├── events/
│   └── ...
├── sdcap/           ← SDCAP content lives here
│   ├── grants/
│   ├── governance/
│   └── ...
└── sdcolab/         ← SDCoLab content lives here
    ├── access/
    ├── classes/
    └── ...
```

### Cross-Site Link Pattern
- Cross-site links: use `xsite` shortcode (stable regardless of page depth)
  - Example: `]({{< xsite "playa" "how-we-gather/sdcap-path/" >}})`
- From SDCoLab → PLAYA: `](../playa/how-we-gather/sdcolab-path/)`
- From PLAYA → SDCAP: `](../sdcap/)`
- From PLAYA → SDCoLab: `](../sdcolab/)`

### Internal Link Pattern
- Within same site: use Hugo `relref` (stable under subdirectory hosting)
  - Example: `]({{< relref "grants/_index.md" >}})`
  - Example: `]({{< relref "how-we-gather/_index.md" >}})`

## Discoverability Added

Each site's home page now prominently features:

**PLAYA (`/`):**
- Quick Links table with How We Gather as top option
- Fire Triangle explanation with links to all three sites
- "New Here?" section pointing to engagement guide

**SDCAP (`/`):**
- Quick Links table with "How to Engage with SDCAP" as top option
- Direct link to `../playa/how-we-gather/sdcap-path/`
- "New Here?" section

**SDCoLab (`/`):**
- Quick Links table with "How to Engage with SDCoLab" as top option
- Direct link to `../playa/how-we-gather/sdcolab-path/`
- "New Here?" section with link to First Build guide

## Files Changed

### Home Pages Updated (3)
- `sites/playa/content/_index.md` — Full navigation hub
- `sites/sdcap/content/_index.md` — Engagement-first navigation
- `sites/sdcolab/content/_index.md` — Engagement-first navigation

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

### Updated Files (15)
All existing content pages refreshed with Fire Triangle context and verified links.

## Commit Message

```
feat: complete content update with verified cross-site links

- Add How We Gather section (9 pages) on PLAYA
- Update all home pages with engagement-first navigation
- Fix all cross-site links (../playa/, ../sdcap/, ../sdcolab/)
- Add Fire Triangle context across all sites
- Verify all link targets exist

🔥 Three heads, one fire. Good dog. 🐾
```

---

*Links verified. Navigation added. Good dog.* 🐕🔥
