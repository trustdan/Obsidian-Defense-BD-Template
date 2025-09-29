---
type: org
sector: government
hq_location: Anywhere, USA
website: https://example.org
tags: [crm/org, #government]
---

# Sample Org

## Summary
- Pilot-friendly; clear buying center.

## Key People (auto)
```dataview
TABLE role, relationship_stage, last_contact, next_touch
FROM "20_People"
WHERE type = "person" AND org = this.file.link
SORT relationship_stage asc, next_touch asc
```
