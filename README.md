# Defense BD Obsidian – Comprehensive README

_Last updated: 2025-09-29_

This README is your quick-start and power-user guide for running Business Development in the defense sector with Obsidian.

---

## 1) Folder Map (high level)

- **00_Dashboards** – Command center dashboards (Dataview tables).
- **00_Inbox** – Quick capture. Process into People/Orgs/Opportunities/Ideas.
- **06_Attachments** – Files/assets you link or embed.
- **10_Meetings** – One note per meeting; end with commitments + next touch.
- **20_People** – Lightweight CRM (one note per key person).
- **25_Orgs** – One note per organization (agency/prime/sub/lab/partner).
- **30_Opportunities** – Each RFI/RFP/teaming lead as a note.
- **35_Pipeline** – Optional Kanban boards (if you use the Kanban plugin).
- **40_Ideas** – “Ideas in Flight” backlog and initiative notes.
- **45_Projects** – Internal initiatives (distinct from external opportunities).
- **50_Accounts** – Account plans for priority orgs.
- **60_Intel** – Knowledge base (Acronyms, Competitors, Programs/Tech).
- **65_Events** – Conferences with goals/targets/meetings and outcomes.
- **70_MOCs-Maps_of_Content** – Dashboards/MOCs for People, Orgs, Opps, Ideas, Accounts.
- **90_Resources-How_To** – Cheatsheets, how-tos, common queries.
- **99_Admin** – Meta docs, changelogs.
- **Templates** – All note templates (mapped to folders).

---

## 2) Plugins You’ll Want

- **Dataview** – renders dashboards/tables from your notes.
- **Tasks** – cross-vault task queries and due dates.
- **Templater** – create notes _from_ templates and auto-fill frontmatter.
- **QuickAdd** (optional) – single-keystroke capture flows.
- **Calendar** (optional) – daily note navigation.
- **Kanban** (optional) – if you prefer a board for pipeline/ideas.

> Enable Community Plugins, then install the ones you want. Trust plugin authors when prompted.

---

## 3) Using Templates (three solid methods)

### A) Core “Templates” plugin (built-in; simple)
1. **Settings → Core plugins → enable “Templates.”**
2. **Settings → Templates → Template folder location:** `Templates/`
3. Create/open a blank note where you want it.
4. Press **Ctrl/Cmd+P → _Templates: Insert template_ → pick one** (e.g., `20_Person`).
5. (Optional) **Hotkey:** Settings → Hotkeys → set a key for “Templates: Insert template.”

**When to use:** You already created the note and just want to insert the structure.

---

### B) Templater plugin (power move; one-step creation)
1. **Install/enable “Templater.”**
2. **Settings → Templater → Template folder location:** `Templates/`
3. Run **Ctrl/Cmd+P → _Templater: Create new note from template_**, choose a template.
4. Templater prompts for a **title** and **save location** → creates the file **and** inserts the template in one go.
5. **Folder templates (recommended):** Templater → “Folder templates”  
   - Map `20_People` → `20_Person.md`, `30_Opportunities` → `30_Opportunity.md`, etc.  
   - **Result:** Any new note created inside that folder auto-applies the right template.

**When to use:** Fastest, most consistent way to create new notes straight into the right folder.

---

### C) QuickAdd (blazing capture via hotkey)
1. Install **QuickAdd**.
2. Create a **Capture**:
   - **Name:** “New Person”
   - **Template:** `Templates/20_Person.md`
   - **Destination:** `20_People/`
   - **File name:** `{VALUE}` (you’ll type “Lastname, Firstname”)
3. Assign a **Hotkey** (e.g., `Alt+P`).
4. Repeat for **New Opportunity** (Alt+O), **New Idea** (Alt+I), etc.

**When to use:** In the flow—create fully formed notes in 1–2 seconds.

---

## 4) Field Conventions (to keep dashboards working)

Use consistent **frontmatter keys**:
- `type` (person, org, opportunity, meeting, idea, project, account, intel, event)
- `status` (for ideas/projects), `stage` (for opportunities)
- `org` (in Person), `customer` (in Opportunity), `sponsor`/`key_stakeholders`
- `last_contact`, `next_touch`, `due_date`
- `value_est`, `prob_win`, `priority` (Opps)

**Tags (optional but helpful):**
- `tier/tier1`, `tier/tier2`, `status/exploring`, `initiative`, `account/plan`, `event/conference`

**Link everything:** People ↔ Orgs ↔ Opportunities ↔ Meetings ↔ Accounts.

---

## 5) MOCs (Maps of Content) – What they look like

<img width="973" height="1087" alt="image" src="https://github.com/user-attachments/assets/2b433e4f-5f4a-47cc-9a3c-f154e1d556de" />


> In **Reading view** with **Dataview** enabled, these render as tables.

**People MOC (example render)**  
| File             | role            | org           | relationship_stage | last_contact | next_touch |
| ---------------- | --------------- | ------------- | ------------------ | ------------ | ---------- |
| [[Smith, Jane]]  | Program Manager | [[USAF AFRL]] | warm               | 2025-09-19   | 2025-10-06 |
| [[Nguyen, Alex]] | Tech Lead       | [[USAF AFRL]] | champion           | 2025-09-20   | 2025-10-03 |
| [[Doe, John]]    | Capture Manager | [[L3Harris]]  | lead               | 2025-08-15   | 2025-10-05 |

**Accounts MOC (example render)**  
| File                         | current_status | owner | fy_targets                 |
| --------------------------- | -------------- | ----- | -------------------------- |
| [[USAF AFRL – Account Plan]]| prospect       | me    | ["SDA Pilot","Edge Demo"]  |
| [[Sample Account – Plan]]    | prospect       | me    | ["Pilot","Phase II"]       |

**Ideas MOC / Ideas in Flight (example render)**  
| File                               | status     | impact | effort | created     | next_action                             |
| ---------------------------------- | ---------- | ------ | ------ | ----------- | --------------------------------------- |
| [[LinkedIn Newsletter – SAMPLE]]   | exploring  | H      | M      | 2025-09-29  | Draft outline and cadence               |
| [[Sales Navigator – SAMPLE]]       | backlog    | H      | S      | 2025-09-29  | Define ICP filters and save lead lists  |

**Opportunities – Pipeline MOC (example render)**  
| File                              | stage    | agency      | due_date   | value_est | prob_win | priority | next_action                                   |
| --------------------------------- | -------- | ----------- | ---------- | --------- | -------- | -------- | --------------------------------------------- |
| [[OPP – AFRL – SDA Pilot – FY25]] | qualify  | USAF/AFRL   | 2025-11-15 | $1.2M     | 0.35     | A        | Deliver capabilities brief to [[Alex Nguyen]] |

**Orgs MOC (example render)**  
| File           | sector     | hq_location              |
| -------------- | ---------- | ------------------------ |
| [[USAF AFRL]]  | government | Wright-Patterson AFB, OH |
| [[L3Harris]]   | prime      | Melbourne, FL            |

> Tip: In each Org note, add a local Dataview that auto-lists its People:
```
```dataview
TABLE role, relationship_stage, last_contact, next_touch
FROM "20_People"
WHERE type = "person" AND org = this.file.link
SORT relationship_stage asc, next_touch asc
```
```

---

## 6) Daily/Weekly Operating Rhythm

**Daily (10 min)**  
- Open **Daily Note** → set Top 3 → check tasks due.  
- Convert Inbox captures into People/Org/Opp/Idea notes using Templates.  
- Log quick bullets in today’s note.

**Weekly (30–45 min)**  
- **BD Dashboard:** clear overdue tasks.  
- **Pipeline (Opportunities MOC):** update stages, due dates, next actions.  
- **People MOC:** schedule next touches for champions/prospects.  
- **Ideas in Flight:** pick one idea to progress.  
- **One Account Plan:** update stakeholders/plays/risks.

---

## 7) Command Palette & Hotkeys (cheat sheet)

**Universal**
- **Ctrl/Cmd+P** – Open Command Palette
- **Ctrl/Cmd+O** – Quick Switcher (jump to any note)
- **Ctrl/Cmd+N** – New note
- **Ctrl/Cmd+E** – Toggle Edit/Reading view
- **Ctrl/Cmd+F** – Find in note
- **Ctrl/Cmd+Shift+F** – Global search
- **Alt+Click** on a link – Open in new pane
- **Ctrl/Cmd+Left/Right** – Navigate back/forward

**Templates & Templater**
- **Templates: Insert template** (bind a hotkey)
- **Templater: Create new note from template**
- **Templater: Replace templates in the active file**

**QuickAdd (if installed)**
- Run your captures: “New Person / Opportunity / Idea” (assign hotkeys like **Alt+P**, **Alt+O**, **Alt+I**).

**Dataview**
- No hotkey by default—just ensure the plugin is enabled; switch to **Reading view** to render queries.

**Calendar / Periodic Notes**
- Click a date to open its daily note (bind a hotkey for “Open today’s note” if desired).

---

## 8) Troubleshooting

- **Dataview not rendering?**  
  Enable Dataview; switch to **Reading view**; check frontmatter keys (`type`, `status`, `stage`, etc.).
- **Tables empty?**  
  Create real notes in the target folders using the templates; the MOCs will auto-populate.
- **Links not resolving?**  
  Make sure you’re using `[[WikiLinks]]` and consistent names (`Lastname, Firstname` for People).

---

## 9) Naming Conventions (recommended)

- **People:** `Lastname, Firstname` (e.g., `Smith, Jane`)
- **Orgs:** just the org name (e.g., `USAF AFRL`)
- **Opportunities:** `OPP – Agency – Program – FY25`
- **Accounts:** `Org – Account Plan`
- **Meetings:** `YYYY-MM-DD – Topic / Counterparty`
- **Events:** `CONFERENCE YYYY – City`

---

## 10) Pro Tips

- Use **folder templates** (Templater) so the right template auto-applies by folder.
- Save **searches/filters** you use frequently (e.g., next touches due this week).
- Keep **`next_action`** populated everywhere—MOCs become action dashboards.
- Keep **`last_contact`** and **`next_touch`** fresh in People for follow-up queries.
- Consider **aliasing** common org/person name variations in frontmatter `aliases: []`.
