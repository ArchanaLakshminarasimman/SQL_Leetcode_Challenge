# 182. Duplicate Emails

**Difficulty:** Easy  
🔗 [LeetCode Link](https://leetcode.com/problems/duplicate-emails/)

---

## Problem Statement

**Table:** `Person`

| Column Name | Type    |
|-------------|---------|
| id          | int     |
| email       | varchar |

- `id` is the **primary key** (unique).
- Each row contains one email.
- Emails will **not contain uppercase letters**.
- The `email` field is **guaranteed to be NOT NULL**.

---

Write a solution to **report all duplicate emails** (emails that appear more than once).

Return the result table in **any order**.

---

### Input Example:

**Person table:**

| id | email   |
|----|---------|
| 1  | a@b.com |
| 2  | c@d.com |
| 3  | a@b.com |

---

### Output:

| Email   |
|---------|
| a@b.com |

---

### Explanation:

- `a@b.com` appears twice, so it should be returned.
- Other emails appear only once.

---

## Solution

See [`182_solution.sql`](./182_solution.sql)
