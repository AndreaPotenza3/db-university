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

### 3. Selezionare tutti gli studenti che hanno più di 30 anni
```SQL

```

### 4. Selezionare tutti i corsi del primo semestre del primo anno di un qualsiasi corso dilaurea (286)

```SQL
SELECT * 
FROM courses
WHERE period = 'I semestre' 
AND year = '1'
```