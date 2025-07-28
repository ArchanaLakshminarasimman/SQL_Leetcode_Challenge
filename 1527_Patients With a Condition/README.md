# 1527. Patients With a Condition

**Difficulty:** Easy  
🔗 [LeetCode Link](https://leetcode.com/problems/patients-with-a-condition/)

---

## 🧩 Problem Statement

**Table:** `Patients`

| Column Name  | Type    |
|--------------|---------|
| patient_id   | int     |
| patient_name | varchar |
| conditions   | varchar |

- `patient_id` is the **primary key** (unique).
- `conditions` contains **0 or more codes** separated by spaces.
- This table stores information about **patients** in the hospital.

---

Write a solution to find the `patient_id`, `patient_name`, and `conditions` of patients who have **Type I Diabetes**.

> Type I Diabetes always starts with the prefix **`DIAB1`** in the `conditions` column.

---

### 📥 Input Example:

**Patients table:**

| patient_id | patient_name | conditions   |
|------------|--------------|--------------|
| 1          | Daniel       | YFEV COUGH   |
| 2          | Alice        |              |
| 3          | Bob          | DIAB100 MYOP |
| 4          | George       | ACNE DIAB100 |
| 5          | Alain        | DIAB201      |

---

### 📤 Output:

| patient_id | patient_name | conditions   |
|------------|--------------|--------------|
| 3          | Bob          | DIAB100 MYOP |
| 4          | George       | ACNE DIAB100 |

---

### 🧠 Explanation:

- **Bob** has a condition `DIAB100` which starts with `DIAB1`.
- **George** also has a condition that includes `DIAB100`.
- **Alain** has `DIAB201` → does **not** match since it doesn't start with `DIAB1`.

---

## ✅ Solution

See [`1527_solution.sql`](./1527_solution.sql)
