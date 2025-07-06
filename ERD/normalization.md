# Database Normalization – Airbnb Clone

## Goal
Ensuring the database schema adheres to Third Normal Form (3NF) to reduce redundancy and improve data integrity.

---

## ✅ First Normal Form (1NF)

- All attributes are atomic (e.g., `first_name`, `email`, `role`)
- Each table has a primary key
- No repeating groups

✔️ Passed

---

## ✅ Second Normal Form (2NF)

- All non-key attributes fully depend on the primary key
- No partial dependencies (no composite primary keys are used)

✔️ Passed

---

## ✅ Third Normal Form (3NF)

- All non-key attributes depend only on the primary key
- No transitive dependencies (e.g., no field depends on another non-key field)

✔️ Passed

---

## 🔄 Optional Improvements

While the current schema satisfies 3NF, the following could be normalized further:

- Extract `role` ENUM into a `Roles` table
- Extract `payment_method` and `status` ENUMs into separate reference tables



## Summary

The current schema is well-designed and adheres to 3NF. It provides a strong foundation for scalable, maintainable relational data in the Airbnb clone project.
