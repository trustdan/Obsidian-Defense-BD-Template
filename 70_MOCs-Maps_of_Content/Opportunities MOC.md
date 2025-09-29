# Opportunities – Pipeline

```dataview
TABLE stage, agency, due_date, value_est, prob_win, priority, next_action
FROM "30_Opportunities"
WHERE type = "opportunity"
GROUP BY stage
SORT due_date asc
```

Example:

|File|stage|agency|due_date|value_est|prob_win|priority|next_action|
|---|---|---|---|---|---|---|---|
|[[OPP – AFRL – SDA Pilot – FY25]]|qualify|USAF / AFRL|2025-11-15|$1.2M|0.35|A|Deliver capabilities brief to [[Alex Nguyen]]|
|[[OPP – Sample Opportunity FY25]]|qualify|Sample Agency|2025-11-30|$1.0M|0.30|A|Send one-pager and schedule demo with [[Sample Person]]|
|[[OPP – L3Harris Teaming – FY25]]|discover|USAF|2025-12-05|$3.5M|0.20|B|Set intro with [[John Doe]] for teaming discussion|

---

