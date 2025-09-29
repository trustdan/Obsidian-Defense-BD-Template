# People – Index

```dataview
TABLE role, org, relationship_stage, last_contact, next_touch
FROM "20_People"
WHERE type = "person"
SORT relationship_stage asc, next_touch asc
```

Example:

| File             | role            | org           | relationship_stage | last_contact | next_touch |
| ---------------- | --------------- | ------------- | ------------------ | ------------ | ---------- |
| [[Smith, Jane]]  | Program Manager | [[USAF AFRL]] | warm               | 2025-09-19   | 2025-10-06 |
| [[Nguyen, Alex]] | Tech Lead       | [[USAF AFRL]] | champion           | 2025-09-20   | 2025-10-03 |
| [[Doe, John]]    | Capture Manager | [[L3Harris]]  | lead               | 2025-08-15   | 2025-10-05 |

---

