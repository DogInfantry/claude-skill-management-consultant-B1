# SQL for PM & Analyst Interviews — Cheat Sheet & PM Lens

A last-mile SQL reference for product/analyst case and interview prep: the high-frequency syntax, the join logic that gets tested, and how SQL maps to PM work. Use with `quantitative-toolkit.md` and `product-management-toolkit.md`.

---

## Part A — Query essentials

```sql
-- Retrieve & filter
SELECT DISTINCT col1, col2 FROM t WHERE condition ORDER BY col1 [ASC|DESC];
SELECT col FROM t WHERE a AND b;   WHERE a OR b;   WHERE NOT a;
SELECT col FROM t WHERE col BETWEEN v1 AND v2;     -- inclusive range
SELECT col FROM t WHERE col LIKE 'A%';             -- pattern match
SELECT col FROM t WHERE col IN (v1, v2, v3);
SELECT col AS alias FROM t AS x;                   -- readable aliases
SELECT TOP 10 col FROM t;                          -- (or LIMIT 10)

-- Modify
INSERT INTO t (c1,c2) VALUES (v1,v2);
UPDATE t SET c1 = v WHERE condition;               -- WHERE is critical
DELETE FROM t WHERE condition;

-- Aggregate
SELECT MIN(c), MAX(c), COUNT(c), SUM(c), AVG(c) FROM t;
SELECT c1, agg(c2) FROM t WHERE cond GROUP BY c1 ORDER BY c1;
SELECT c1, agg(c2) FROM t GROUP BY c1 HAVING agg(c2) > x;   -- filter on aggregates
```

**`WHERE` vs `HAVING`:** `WHERE` filters **rows before** grouping; `HAVING` filters **groups after** aggregation. Mixing these up is a classic interview trip-up.

**Logical order of execution** (not the written order): `FROM → WHERE → GROUP BY → HAVING → SELECT → ORDER BY`. Knowing this explains why you can't reference a `SELECT` alias in `WHERE`.

---

## Part B — Joins (the part interviews love)

```sql
SELECT ... FROM a INNER JOIN b ON a.k = b.k;   -- only matching rows in both
SELECT ... FROM a LEFT  JOIN b ON a.k = b.k;   -- all of A + matches from B
SELECT ... FROM a RIGHT JOIN b ON a.k = b.k;   -- all of B + matches from A
SELECT ... FROM a FULL  JOIN b ON a.k = b.k;   -- all rows, matched where possible
SELECT ... FROM t T1, t T2 WHERE T1.k = T2.mgr;-- self join (table with itself)
```

**The high-frequency question — "which join returns the most / fewest rows?"**
- **Fewest:** `INNER JOIN` — only keys present in *both* tables survive.
- **Most:** `FULL OUTER JOIN` — keeps unmatched rows from *both* sides (`LEFT`/`RIGHT` sit in between).
- With duplicate keys, row count can *multiply* (a key appearing 3× in A and 2× in B yields 6 rows) — mention this; it shows depth.

**Combining result sets:** `UNION` stacks two `SELECT`s and **removes duplicates**; `UNION ALL` keeps duplicates (and is faster).

---

## Part C — Subqueries & conditional logic

```sql
WHERE EXISTS (subquery)                 -- true if subquery returns any row
WHERE col operator ANY (subquery)       -- compare to at least one value
WHERE col operator ALL (subquery)       -- compare to every value
SELECT * INTO newtable FROM src WHERE c;        -- create+fill a new table
INSERT INTO target SELECT * FROM source WHERE c;-- copy rows between tables
CASE WHEN cond1 THEN r1 WHEN cond2 THEN r2 ELSE r3 END  -- stops on first match
```

---

## Part D — SQL through a PM/analyst lens

PMs use SQL to **answer product questions without waiting on an analyst**:
- **Funnel/AARRR analysis:** `COUNT(DISTINCT user_id)` per stage with `GROUP BY` to find the leaky step.
- **Cohorts & retention:** `GROUP BY` signup cohort, join to activity, measure return rates.
- **Segment metrics:** `GROUP BY plan/region/channel` then `HAVING` to surface segments above/below a threshold.
- **Feature adoption:** `LEFT JOIN` users to feature-event table; the unmatched (NULL) rows are non-adopters.
- **North Star / guardrails:** translate each metric into a single, reproducible query so it's monitored consistently.

**Interview tip:** when asked to "find X," say the logical order out loud (filter rows → group → aggregate → filter groups → sort) before writing — it demonstrates you reason about SQL, not just recall syntax.

---

## Usage rules for Claude
1. Default to ANSI SQL; note when a clause is dialect-specific (`TOP` vs `LIMIT`).
2. For "most/fewest rows" join questions, always cover the duplicate-key multiplication case.
3. When a PM data question is posed, propose the *query shape* (which clauses, which join) before full syntax.
