# 1667. Fix Names in a Table

**Difficulty:** Easy  
🔗 [LeetCode Link](https://leetcode.com/problems/fix-names-in-a-table/)

---

## Problem Statement

**Table:** `Users`

| Column Name | Type    |
|-------------|---------|
| user_id     | int     |
| name        | varchar |

- `user_id` is the primary key (unique).
- This table contains the ID and **name of the user**.
- The `name` column may contain only **lowercase and uppercase** characters.

---

Write a SQL solution to **fix the names** so that:

- Only the **first character** is uppercase
- The **rest of the characters** are lowercase

Return the result table ordered by `user_id`.

---

### Input Example:

**Users table:**

| user_id | name  |
|---------|-------|
| 1       | aLice |
| 2       | bOB   |

---

### Output:

| user_id | name  |
|---------|-------|
| 1       | Alice |
| 2       | Bob   |

---

## Solution

See [`1667_solution.sql`](./1667_solution.sql)
