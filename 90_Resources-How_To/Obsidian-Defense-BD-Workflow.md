# Obsidian Defense BD Workflow (Cheatsheet)

## Philosophy
- **Folders** keep things clean; **Links** `[[like this]]` create context; **Tags** `#like/this` help filter statuses/tiers.
- Mirror statuses with both a field (e.g., `status: exploring`) and an optional tag (`status/exploring`) if you like quick tag filters.

## Core Plugins
- Dataview, Tasks, Periodic Notes + Calendar, Templater, QuickAdd (optional), Kanban (optional), Advanced URI (optional).

## Capture → Organize
- Quick capture to `00_Inbox`. Promote using Templates into People, Orgs, Opportunities, Ideas.

## Reviews
**Daily (10 min)**: Daily Note (Top 3), tasks due, meetings.  
**Weekly (30–45 min)**: Open **BD Dashboard**, review Pipeline, People next-touches, **Ideas in Flight**, and Account plans.  
**Monthly**: Clean stale opps, archive, update account plans; refresh initiative backlog.

## Useful Queries (Dataview)

### People needing a touch (next 7 days)
```dataview
TABLE org, role, relationship_stage, last_contact, next_touch
FROM "20_People"
WHERE type="person" AND next_touch <= date(today) + dur(7 days)
SORT next_touch asc
```

### People not contacted in 60+ days
```dataview
TABLE org, role, relationship_stage, last_contact, next_touch
FROM "20_People"
WHERE type="person" AND last_contact != null AND (date(today) - date(last_contact)) > dur(60 days)
SORT last_contact asc
```

### Opportunities by due date
```dataview
TABLE stage, agency, due_date, priority, next_action
FROM "30_Opportunities"
WHERE type = "opportunity"
SORT due_date asc
```

### Initiatives & Ideas by status
```dataview
TABLE status, impact, effort, created, next_action
FROM "40_Ideas"
WHERE type="idea" OR contains(tags, "initiative")
GROUP BY status
SORT created desc
```

## Note Naming
- People: `Lastname, Firstname`
- Orgs: `ORG - Account Plan` or just the org name
- Opps: `OPP - Agency - Program - FY25`

## Linking Tips
- In Opportunity notes: link sponsor `[[Jane Smith]]` and customer org.
- In Meeting notes: link every attendee and the related opportunity/account.

## QuickAdd Suggestions
- Create "New Person / Org / Opportunity / Idea" capture macros from templates.
- Add default fields (date, status) and prompt for key fields (name, org, due).
