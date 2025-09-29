---
type: org
sector: government # government | prime | sub | lab | VC | partner | university
type_tag: #government  # #prime | #subcontractor | #government | #partner
parent: 
hq_location: 
website: 
duns: 
cage: 
naics: []
intel_tags: []
tags: [crm/org]
---

# {{title}}

## Summary
- Mission/charter: 
- Buying centers: 
- Relevant tech interests: 

## Key People (auto)
```dataview
TABLE role, relationship_stage, last_contact, next_touch
FROM "20_People"
WHERE type = "person" AND org = this.file.link
SORT relationship_stage asc, next_touch asc
```

## Active Opportunities
- 

## Notes
- 
