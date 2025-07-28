# 1407. Top Travellers

**Difficulty:** Easy  
🔗 [LeetCode Link](https://leetcode.com/problems/top-travellers/)

## Problem Statement

Table: `Users`

| Column Name | Type    |
|-------------|---------|
| id          | int     |
| name        | varchar |

- `id` is the column with unique values for this table.
- `name` is the name of the user.

Table: `Rides`

| Column Name | Type    |
|-------------|---------|
| id          | int     |
| user_id     | int     |
| distance    | int     |

- `id` is the column with unique values for this table.
- `user_id` is the id of the user who traveled the distance `distance`.

Write a solution to report the distance traveled by each user.

Return the result table ordered by `travelled_distance` in **descending order**, and if two or more users traveled the same distance, **order them by their name in ascending order**.

---

## Example

**Input:**

Users table:

| id | name     |
|----|----------|
| 1  | Alice    |
| 2  | Bob      |
| 3  | Alex     |
| 4  | Donald   |
| 7  | Lee      |
| 13 | Jonathan |
| 19 | Elvis    |

Rides table:

| id | user_id | distance |
|----|---------|----------|
| 1  | 1       | 120      |
| 2  | 2       | 317      |
| 3  | 3       | 222      |
| 4  | 7       | 100      |
| 5  | 13      | 312      |
| 6  | 19      | 50       |
| 7  | 7       | 120      |
| 8  | 19      | 400      |
| 9  | 7       | 230      |

**Output:**

| name     | travelled_distance |
|----------|--------------------|
| Elvis    | 450                |
| Lee      | 450                |
| Bob      | 317                |
| Jonathan | 312                |
| Alex     | 222                |
| Alice    | 120                |
| Donald   | 0                  |

**Explanation:**
- Elvis and Lee both traveled 450 miles.
- Elvis comes first as his name is alphabetically smaller than Lee.
- Donald did not take any rides, so his distance is 0.

---

## Solution

See [`solution.sql`](./solution.sql)
