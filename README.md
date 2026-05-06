# Mortals+ — Chronicles of Darkness Character Sheet Builder

Mortals+ is a browser-based character builder and live play aid for Chronicles of Darkness (Second Edition). One of the Chronicles of Darkness core rulebooks is required to use this app.

**[Open the app →](https://bonewolf22.github.io/Mortals-A-Chronicles-of-Darkness-Character-Builder/)**

---

## Supported splats

**Main splats**
- Mortal (Chronicles of Darkness core)
- Beast: The Primordial †
- Changeling: The Lost
- Demon: The Descent
- Deviant: The Renegades
- Geist: The Sin-Eaters
- Hunter: The Vigil
- Mage: The Awakening
- Mummy: The Curse †
- Promethean: The Created †
- Vampire: The Requiem
- Werewolf: The Forsaken
- Ephemeral Entities (Spirits, Ghosts, Angels, Demons, Goetia, Supernal Beings)

† These splats have no default library entries (Atavisms, Nightmares, Transmutations, Utterances, etc.). The sheet structure is complete but the ability dropdowns will show only a placeholder entry until you add content from the rulebook. Use the in-app **Library Editor** or see [CUSTOMISATION_GUIDE.md](CUSTOMISATION_GUIDE.md) for the format.

**Half-splats**
- Ghoul
- Proximi
- Wolf-Blooded

**Other**
- Mage: The Ascension (via the Mage Translation Guide)
- Horrors (Chronicles of Darkness core / Hunter: The Vigil antagonists)

---

## Features

### Character sheet

- **Attributes** — 9 attributes across Mental, Physical, Social, displayed as clickable dots with Power/Finesse/Resistance row labels. Cycle between 5-dot, 10-dot, and 15-dot display; an overflow indicator (`+N`) appears when a value exceeds the current dot max. Show numeric values toggle also available
- **Skills** — 24 skills across Mental, Physical, Social (rated 0–5), with rote checkbox and specialty field. Skill names are editable inline
- **Health track** — typed damage (Bashing / Lethal / Aggravated); click any box to cycle; auto-resizes when Stamina or Size changes
- **Willpower** — dot and box tracker with adjustable maximum
- **Derived traits** — Defense, Initiative, Speed; auto-calculated from stats with manual override. When armor is equipped, an Armor row shows per-location general/ballistic ratings (Head, Torso, Arms, Legs) summed across all equipped pieces
- **Beats / Experience** — 5 Beats auto-awards 1 XP; fully data-driven (splat-specific beat trackers can be added in `data.json` without code changes)
- **Tilts and Conditions** — searchable library with custom entry support
- **Aspirations** — simple line list
- **Merits** — searchable library, 5-dot or 10-dot max toggle
- **Weapons** — melee and ranged cards with full stat fields; Equipped toggle applies Initiative modifier to derived traits
- **Armor** — cards with full stat fields; Equipped toggle applies Defense and Speed penalties; per-location coverage checkboxes (Head, Torso, Arms, Legs)
- **Equipment** — cards with dice bonus, durability, size, structure
- **Notes** — free-text field with markdown support

### Splat sections

Apply a preset from the **Sheet Configuration** panel to enable all sections for a given splat. Sections can also be toggled individually. Each splat adds its own sections on top of the standard sheet:

- **Beast** — Legend/Life/Concept/Family/Hunger/Soul header, Lair (10-dot track), Satiety (10-dot track), Satiety Condition, Atavisms, Nightmares, Family Ties
- **Changeling** — Needle/Thread/Seeming/Court/Kith header, Wyrd, Clarity (dot-square track), Glamour, Favored Regalia, Frailties, Touchstones, Goblin Debt, Contracts, Pledges, Seeming Blessing/Curse, Kith Blessing
- **Demon** — Incarnation/Agenda/Catalyst header, Cover Rating, Primum, Aether, Demonic Form, Embeds, Exploits, Cipher (interactive gear diagram), Covers (identity cards with per-cover Merits), Cover Beats tracker
- **Deviant** — Origin/Clade/Forms header, Stability (dot-square track), Acclimation, Flux, Touchstones, Variations (rated by Magnitude), Scars (rated by Magnitude), Adaptations, Origins
- **Geist** — Geist/Burden/Root/Bloom/Krewe header, Synergy (labeled track with per-level labels), Plasm, Keys, Haunts, Remembrance Traits
- **Hunter** — Compact/Conspiracy header, Endowments, Tactics, Touchstones, The Code, Group Beats tracker
- **Mage** — Path/Order/Legacy/Cabal header, Arcana block (10 Arcana rated 0–5), Gnosis, Wisdom, Mana, Obsessions, Inured Spells, Rotes, Praxes, Arcana Attainments, Legacy Attainments, Arcane Beats tracker, Nimbus, Yantras, Magical Tools
- **Mummy** — Guild/Decree/Burden/Balance/Judge/Meret Name header, Sekhem (dot-square track ×10), Memory (dot-square track ×10), Pillars block (Ab/Ba/Ka/Ren/Sheut — each with permanent dots and temporary squares), Reminisce Beats tracker, Affinities, Touchstones, Utterances (rated-list)
- **Promethean** — Elpis/Torment/Lineage/Refinement/Role header, Pilgrimage, Azoth, Pyros, Transmutations, Bestowment, Refinement Condition, Fixed Alembics, Milestones, Mastered Roles, Vitriol Beats tracker
- **Vampire** — Clan/Covenant/Bloodline header, Blood Potency, Humanity, Vitae, Banes, Disciplines, Devotions, Vampire Rites
- **Werewolf** — Auspice/Tribe/Lodge/Pack header, Primal Urge, Harmony, Essence, Renown block (5 renown types), Flesh/Spirit Touchstones, live Forms reference table (calculated stats per form), Gifts, Rites
- **Ephemeral Entity** — Type/Rank/Concept header, Power/Finesse/Resistance attributes (5/10/15-dot display), Corpus track, Willpower, Essence, derived stats, Numina, Manifestations, Influences, Ban, Bane. Ghost variant adds Anchors; Supernal variant adds Arcana

**Half-splats** layer onto the standard mortal sheet and share relevant sections with their parent splat:

- **Ghoul** — Regnant's Clan/Covenant/Family identity, Disciplines (shared with Vampire), Vitae (shared with Vampire)
- **Wolf-Blooded** — Tribe/Pack identity, Tells, Tension Pool
- **Proximi** — Dynasty/Heritage Path identity, Blessings (draws from Rotes library), Mana (shared with Mage), Curse

**Other presets** are available for non-standard play:

- **Mage (Ascension)** — Uses the Mage: the Ascension Translation Guide. Replaces Awakening sections with Ascension equivalents: Spheres (10 Arcana, same dots), Arete (Gnosis), Practices (Yantras), Foci (Magical Tools), Resonance (Nimbus), Sphere Attainments. Adds a Quintessence & Paradox wheel: a circular 20-square track where Quintessence fills clockwise and Paradox counter-clockwise; increasing Paradox decrements Quintessence automatically. Avatar Essence/Affiliation/Sect identity header. Wisdom, Praxes, Obsessions, and Inured Spells off by default.
- **Horror** — For Chronicles of Darkness antagonists. Standard mortal sheet with Horror Identity (Type, Concept), Potency (dot-track), and Dread Powers (named-list)
- **Minor NPC** — Lightweight GM stat block. Enables Name/Concept/Virtue/Vice, Attributes, Other Traits, and two dice pool sections (General and Combat). All other sections hidden. Intended for quick NPC builds.

### Generation

- **Generate Mortal** — distributes dots using standard Chronicles of Darkness creation spreads (Attributes 5/4/3, Skills 11/7/4), picks a random name. Respects the preset currently selected in Sheet Configuration — generate a Hunter, Mage, or any other splat directly
- **Generate Ephemeral Entity** — generates a stat block scaled to the selected Rank, sampling Numina, Manifestations, Influences, Ban, and Bane from the library. Applies the Ephemeral Entity preset automatically
- **New blank sheet** — all attributes at 1, all skills at 0. Respects the selected preset

### Description formatting

Description fields support lightweight markdown:

| Syntax | Result |
|---|---|
| `**text**` | **bold** |
| `*text*` | *italic* |
| `***text***` | ***bold italic*** |

Press Enter for line breaks. Fields show rendered text by default — click to edit, click away to save. In `data.json`, use `\n` for line breaks in JSON strings.

### Layout

Section titles are drag handles — drag any section to reorder it or move it between columns. Layout is saved per character. Use **Reset layout to defaults** to restore the original positions. Use **Lock layout** to prevent accidental drags during play.

### Collapsible sections

Click any section header to collapse it. Collapsed state is preserved across page refreshes.

### Print / Save as PDF

Click **Print / Save as PDF** in the toolbar. Use your browser's **Save as PDF** destination with **Letter** paper size.

- **Chrome is the recommended browser** for printing. Firefox does not reliably handle page breaks at the attributes/columns boundary
- Before printing, sections are automatically compacted into a space-efficient layout — attributes, skills, arcana, renown, pillars, merits, ability lists, gear, covers, and the Werewolf forms table all switch to compact renderers. The live sheet is fully restored after the print dialog closes
- Tilts and Conditions always print with at least 3 rows (filled entries plus blank ruled lines) for pencil use at the table
- All collapsed sections and closed item cards are automatically expanded before printing, then restored afterwards
- Consumable tracks (health, willpower, resource tracks, dot tracks) print empty so they can be filled in pencil at the table
- Beats trackers do not print — they are live-play tools only
- The PDF filename defaults to the character's name (Chrome)

### Mobile and tablet

On touch devices the desktop sidebar is replaced by a floating button that opens a bottom drawer with the same Save, Configure, Sheet, and Library panels. Section drag-and-drop and textarea resize handles are touch-compatible.

---

## Saving characters

Characters are saved in your **browser's local storage** — no account or server required. This means:

- Saves are local to your device and browser
- To move a character between browsers or devices, use **Export sheet** (downloads a `.json` file) and **Import sheet** on the destination browser
- Clearing browser data will delete your saves — export important characters regularly

### Organising saved characters

The Saves panel supports two organisational tools:

- **Tags** — attach freeform labels to any character (e.g. `PC`, `NPC`, `active`). The filter bar searches by both name and tag. Tags are added and removed directly on each save-item row.
- **Folders** — group characters into named folders for broader organisation (e.g. by chronicle or faction). Folders are collapsible and appear in the Saves panel, the tablet drawer, and the Storyteller Mode "Add to Scene" sidebar. Characters not assigned to a folder appear in an ungrouped section at the bottom. Create folders via the input at the bottom of the Saves panel; rename or delete via the buttons that appear on hover.

Tags and folders are complementary — use folders for broad grouping and tags for cross-cutting labels that span folders.

---

## Storyteller Mode

Storyteller Mode is a desktop-only GM overlay for running live scenes with multiple characters. Access it via the **⚔ Storyteller Mode** button in the sidebar. It is hidden on touch devices.

The scene workspace shows all active characters as compact cards. Each card displays:

- **Health / Corpus track** — click boxes to deal damage, same as the main sheet
- **Willpower track** — spend and recover dots during play
- **Resource tracks** — all enabled resource sections (Vitae, Essence, Mana, etc.) rendered automatically for any splat
- **Derived stats** — Defense, Initiative, Speed, with wound penalty highlighted when the last three health boxes are filled
- **Armor coverage** — aggregate Head/Torso/Arms/Legs ratings from all equipped armor pieces
- **Equipped gear, conditions, tilts, pinned traits, and instance notes** — all visible at a glance in the card header

Expand a card with the **▶ arrow** to access the full character reference, equip or unequip gear, add conditions and tilts, pin abilities to the card header, and edit instance notes.

Changes made in Storyteller Mode (damage, conditions, equipped gear, notes) exist only in the scene and **never affect the original saved character sheet**.

### Initiative tracker

The scene panel includes a built-in **Initiative Tracker**, accessible via the **Init** button in the Storyteller Mode toolbar. The tracker:

- Lists all scene instances ordered by Initiative value (highest first)
- Supports ad-hoc entries for minor NPCs not in the scene proper
- Tracks acted/unacted status per character per round with a single click
- Shows a round counter; advance with **Next Round** (resets all acted markers)
- Rolls Initiative for all unrolled instances at once via **Roll All**
- Persists across scene reloads

### Adding characters and managing the scene

Use **Add to Scene** in the sidebar to bring saved characters into play. Characters are shown grouped by folder if folders are set up. Each character you add becomes an independent **instance** — you can add multiple instances of the same character for groups of identical NPCs.

Use the **− Columns +** control in the toolbar to organise cards across up to five columns. Drag cards by their title bar to move them between columns. Use **New Scene** to clear the scene and start fresh (with confirmation).

---

## Data library editor

The **Library Editor** (accessible via the Data Library panel in the sidebar or drawer) lets you extend the built-in ability lists with your own entries — merits from a supplement, homebrew abilities, weapons from the rulebook, and so on.

### How it works

The library editor maintains a **supplement** layer stored in your browser alongside your characters. At startup, supplement entries are merged with the base library — entries with the same name as a base entry **override** the base entry rather than duplicating it. The base library (`data.json`) is never modified; clearing your supplement always restores the original entries.

### Adding and editing entries

Select a section type from the dropdown (Merits, Disciplines, Weapons, etc.). The editor shows your supplement entries first, then the full base library below. For each section type, the editor presents the appropriate fields:

- **Weapons** — name, type (melee/ranged/thrown), damage, initiative modifier, strength requirement, size, availability, ranges, clip, notes
- **Armor** — name, general/ballistic armor, defense/speed penalty, strength requirement, availability, coverage checkboxes, notes
- **Equipment** — name, dice bonus, durability, size, structure, availability, description
- **Rated ability lists** (Merits, Disciplines, Gifts, etc.) — name, rating, description
- **Named ability lists** (Tilts, Conditions, Contracts, etc.) — name, description

Use **Override** on any base library entry to pre-fill the add form with that entry's values — edit what you need and save to create a supplement entry that replaces the base.

Use the **search bar** to filter entries by name across both supplement and base sections. Use the **A–Z / Recent** sort toggle to sort your supplement entries alphabetically or by most recently added.

### Adding sheet entries to the library

Any item on a character sheet that isn't already in the library shows a small **+ lib** button in its header row. Clicking it saves that entry to your supplement immediately — useful for weapons, armor, merits, or abilities you've typed in from a rulebook. The button disappears once the entry is in the library.

### Backup and sharing

Use **Export** in the library editor to download your supplement as a `supplement.json` file. Use **Import** to merge entries from a file (existing same-name entries are kept; duplicates are skipped). Export regularly — clearing your browser data will erase your supplement.

---

## Contributing

Everything that can be customised lives in **`data.json`** — no code changes are needed for most additions. See [CUSTOMISATION_GUIDE.md](CUSTOMISATION_GUIDE.md) for a full walkthrough, from adding a single merit to building a complete new splat.

For code contributions, the entire frontend lives in two files with no build step or external dependencies:

- `index.html` — all HTML, CSS, and JavaScript
- `data.json` — all configuration and content

Run locally using the **Live Server** VS Code extension (`Go Live` button). Do not open `index.html` directly via `file://` — the `fetch('./data.json')` call will be blocked by browser security.

---

## License

Fan tool. Chronicles of Darkness is a trademark of Paradox Interactive AB. Not affiliated with or endorsed by Paradox Interactive. Forks are welcome provided they are not used for commercial gain.

Skull images are from https://mrgone.rocksolidshells.com/
