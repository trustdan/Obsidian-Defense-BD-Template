# ✈️ Ideas in Flight

```dataview
TABLE status, impact, effort, created, next_action
FROM "40_Ideas"
WHERE type = "idea" OR contains(tags, "initiative")
GROUP BY status
SORT created desc
```

Example:

|File|status|impact|effort|created|next_action|
|---|---|---|---|---|---|
|[[LinkedIn Newsletter – SAMPLE]]|exploring|H|M|2025-09-29|Draft outline and cadence|
|[[Sales Navigator – SAMPLE]]|backlog|H|S|2025-09-29|Define ICP filters and save lead lists|
|[[Capabilities One-Pager Refresh]]|doing|M|M|2025-09-20|Circulate draft for approvals|

---

