### 1. Selezionare tutti gli studenti nati nel 1990 (160)

```SQL
SELECT *
FROM students
WHERE date_of_birth LIKE '1990-%'
```

### 2. Selezionare tutti i corsi che valgono più di 10 crediti (479)

```SQL
SELECT * 
FROM courses
WHERE cfu > '10'
```