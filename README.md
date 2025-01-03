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
SELECT * 
FROM students
WHERE date_of_birth <= '1994-12-18'
```

### 4. Selezionare tutti i corsi del primo semestre del primo anno di un qualsiasi corso dilaurea (286)

```SQL
SELECT * 
FROM courses
WHERE period = 'I semestre' 
AND year = '1'
```

### 5. Selezionare tutti gli appelli d'esame che avvengono nel pomeriggio (dopo le 14) del 20/06/2020 (21)

```SQL
SELECT * 
FROM exams
WHERE date = '2020/06/20'
AND hour > '13%'
```

### 6. Selezionare tutti i corsi di laurea magistrale (38)

```SQL
SELECT * 
FROM degrees
WHERE level = 'magistrale'
```
### 7. Da quanti dipartimenti è composta l'università? (12)

```SQL
SELECT * 
FROM departments;
```
oppure

```SQL
SELECT count (*) 
FROM departments;
```


### 8. Quanti sono gli insegnanti che non hanno un numero di telefono? (50)

```SQL
SELECT * 
FROM teachers
WHERE phone is NULL
```

### 9. Inserire nella tabella degli studenti un nuovo record con i propri dati (per il campo degree_id, inserire un valore casuale)

```SQL
INSERT INTO students 
VALUE ('5001', '44', 'Andrea', 'Potenza', '1994-01-04','PTNNDR94A04L419A', '2019-09-12', '625033', 'andreapoten3@gmail.com')
```

### 10. Cambiare il numero dell’ufficio del professor Pietro Rizzo in 126

```SQL
UPDATE teachers
SET office_number = '126'
WHERE id = '58'
```

### 11. Eliminare dalla tabella studenti il record creato precedentemente al punto 9

```SQL
DELETE FROM students
WHERE id = '5001'
```