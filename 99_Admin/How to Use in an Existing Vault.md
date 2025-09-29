# Install These Materials in an Existing Obsidian Vault (Quick Guide)

## 1) Unzip and Copy
- Unzip the starter zip.
- Drag the folders you want (e.g., `20_People`, `25_Orgs`, `30_Opportunities`, `40_Ideas`, `00_Dashboards`, `70_MOCs`, `Templates`, `90_Resources`) **into your existing vault**.
- If you already have similarly named folders, you can merge them or rename ours before copying (Obsidian doesn't care about exact folder names).

## 2) Install/Enable Plugins
- **Community Plugins → Browse**: Install and enable
  - **Dataview**
  - **Tasks**
  - **Templater**
  - **Calendar** (optional but recommended)
  - **QuickAdd** (optional for one-keystroke capture)
- Trust these plugins when prompted.

## 3) Configure Templater
- Settings → **Templater** → Template Folder Location: set to your **`Templates`** folder.
- (Optional) Set a hotkey for "Templater: Create new note from template".

## 4) Daily/Weekly Notes (Optional)
- Install **Periodic Notes** or use **Calendar**.
- Point Daily Notes to `Templates/00_Daily_Note.md`.
- Use `Templates/80_Weekly_Review.md` for a weekly reflection.

## 5) Verify Dashboards
- Open `00_Dashboards/BD Dashboard.md` and `70_MOCs/*`.
- If tables are empty, create a couple of **Person**, **Org**, **Opportunity**, and **Idea** notes from the templates; dashboards will auto-populate.

## 6) QuickAdd (Optional Power-Up)
- Create QuickAdd "Capture" actions for:
  - New **Person** (uses `Templates/20_Person.md`)
  - New **Opportunity** (uses `Templates/40_Opportunity.md`)
  - New **Idea/Initiative** (uses `Templates/50_Idea.md`)
- Bind each to a hotkey for instant capture.

## 7) Conventions
- **Links** create your graph of context: always link people ↔ orgs ↔ opportunities ↔ meetings.
- **Tags** are best for status/filters (e.g., `status/active`, `tier/tier1`, `#initiative`). 
- Keep using frontmatter fields (`status`, `last_contact`, `stage`, `due_date`) so dashboards can query them.

You're done. Start in `00_Dashboards/BD Dashboard.md` and use the Templates to add new items.
