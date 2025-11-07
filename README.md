# Java_JPA_Hibernate-lab-02_Case1_Solved

## Exercise

Identity of entity definition

Goal

Learn how to define simple and composite identity of entity in terms of Java Persistence API. 

Subject

There is a Department entity (with fields: companyName, name and description) and 3 cases to defined identity for it:

1.	Single identity

2.	Composite with identity as separate class (using @EmbeddedId)

3.	Composite with identity fields inside the entity class (using @IdClass)

You need to implement all three cases.

Description

Single identity

1.	Open module jpa-lab-02

2.	Open class edu.jpa.entity.Department_1

3.	Specify class-level annotation @Entity. This lets JPA runtime to know that this particular class should be treated as an entity.

4.	Specify field-level annotation @Id for id field. This lets JPA runtime to know that this fields is used as key

5.	Specify field-level annotation @GeneratedValue for id field. This applies particular identity generation strategy for this field (here the default one will be applied).

## Solution

```
SHOW DATABASES LIKE 'JPA_DB_02';

USE JPA_DB_02;

SHOW TABLES;

SHOW CREATE TABLE Department_1;

SELECT id, companyName, departmentName, description FROM Department_1;

SELECT COUNT(*) FROM Department_1;
```

<img width="1919" height="762" alt="image" src="https://github.com/user-attachments/assets/c55f0619-e09c-419f-82a0-19c0d68365ae" />

