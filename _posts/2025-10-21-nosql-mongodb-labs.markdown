---
layout: posts
title: "NoSQL — MongoDB Labs & Practical Exercises"
date: 2025-10-21 6:00:00 +0200
tags: [MongoDB]
author_profile: true
author: Ahmed Almahey
categories: [work]
highlight_home: false
header:
  overlay_image: "/assets/images/Screenshot 2025-10-21 102750.png"
  teaser: "/assets/images/Screenshot 2025-10-21 102750.png"
description: "A series of hands-on MongoDB labs exploring CRUD operations, data modeling, schema validation, and performance optimization using indexes and aggregation techniques."
---

**NoSQL — MongoDB Labs & Practical Exercises**

This collection of MongoDB labs was completed as part of the ITI database training track.  
The focus was on **mastering core NoSQL concepts** through structured, task-based learning using **MongoDB Compass** and **Robo 3T Studio**.

Although not a full project, these exercises collectively demonstrate practical knowledge in document-based modeling, query building, and performance tuning.

---

###  Lab 1 — Foundational CRUD Operations

- Created a new database named **`ITI_Mongo`** and a collection **`Staff`**.  
- Performed **insertOne** and **insertMany** operations to add staff documents.  
- Executed various **query filters**:
  - Find all documents  
  - Find by gender or age range  
  - Combine multiple conditions using `$and` and `$or`  
- Practiced **updateOne** and **updateMany** to modify records.  
- Experimented with **deleteOne**, **deleteMany**, and full collection deletions.

> 💡 *Outcome:* Gained confidence in performing data manipulation and retrieval in MongoDB’s document model.

---

### ⚙️ Lab 2 — Query Operators, Arrays & Updates

- Used queries with operators like `$exists`, `$all`, `$size`, and comparison filters.  
- Applied update operators such as `$set`, `$unset`, `$currentDate`, `$setOnInsert`, `$inc`, `$min`, `$max`, and `$mul`.  
- Practiced **upsert** behavior for document replacement.  
- Implemented aggregation logic to:
  - Calculate **Total Revenue** per product (`Quantity * Price`)  
  - Compute **Average Salary per Department**  
  - Determine **Max and Min Likes per Title**

> 💡 *Outcome:* Strengthened understanding of update operators and aggregation capabilities in NoSQL contexts.

---

### Lab 3 — Schema Validation & Indexing

- Defined **JSON Schema validation** for the `employees` collection with:
  - Required fields: `name`, `age`, `department`  
  - Age constraint: `>= 18`  
  - Department limited to: `["HR", "Engineering", "Finance"]`  
- Created multiple collections (`trainningCenter1`, `trainningCenter2`) using **insertOne** and **insertMany**.  
- Explored **query plan analysis** with `find().explain()` to observe scanning types.  
- Built indexes:
  - `IX_age` on `age`  
  - `compound` on `firstName` & `lastName`  
- Compared **performance before vs after indexing**.  
- Performed full cleanup with `deleteOne`, `deleteMany`, and `dropDatabase()`.

> 💡 *Outcome:* Learned to optimize query performance and enforce integrity through schema validation.

---

### Skills Demonstrated

- NoSQL data modeling  
- CRUD operations  
- Advanced query filtering  
- Aggregation and computation logic  
- Schema validation and constraints  
- Indexing and query optimization  
- Tool usage: MongoDB Compass & Robo 3T

---

### 🔗 Repository

[MongoDB Tasks at ITI – GitHub](https://github.com/Ahmed-Almahey/Mongo-DB-Tasks_ITI/tree/main)

---
