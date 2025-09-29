# Accounts – Overview

```dataview
TABLE current_status, owner, fy_targets
FROM "50_Accounts"
WHERE type = "account"
SORT current_status, file.name
```



Example:

| File                         | current_status | owner | fy_targets                |
| ---------------------------- | -------------- | ----- | ------------------------- |
| [[USAF AFRL – Account Plan]] | prospect       | me    | ["SDA Pilot","Edge Demo"] |
| [[Sample Account – Plan]]    | prospect       | me    | ["Pilot","Phase II"]      |
| [[L3Harris – Account Plan]]  | active         | me    | ["Teaming","Phase III"]   |

---

