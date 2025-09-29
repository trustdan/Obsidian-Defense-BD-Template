# 🚀 Business Development Dashboard

## 🎯 Open Action Items
```dataview
TASK
WHERE !completed
GROUP BY file.link
```

## 📈 Active Opportunities Pipeline
```dataview
TABLE stage as "Stage", value_est as "Est. Value", sponsor as "POC", due_date as "Due"
FROM "30_Opportunities"
WHERE type = "opportunity" AND stage != "awarded" AND stage != "lost"
SORT due_date asc
```

## 💡 Initiatives & Ideas
```dataview
TABLE status, impact, effort, created, next_action
FROM "40_Ideas"
WHERE type = "idea" OR contains(tags, "initiative")
GROUP BY status
SORT created desc
```

## 👥 People to (Re)Contact (>60 days)
```dataview
TABLE org, role, relationship_stage, last_contact, next_touch
FROM "20_People"
WHERE type = "person" AND last_contact != null AND (date(today) - date(last_contact)) > dur(60 days)
SORT last_contact asc
```

## 🗓️ Recent Meetings
```dataview
LIST
FROM "10_Meetings"
SORT file.mtime DESC
LIMIT 15
```
