# PL/SQL Programming Assignments Solutions

## 1. Create GitHub Account and Learn Basic Git Commands

```bash
# Initialize git repository
git init

# Add files
git add .

# Commit files
git commit -m "First Commit"

# Connect GitHub repository
git remote add origin https://github.com/yourusername/repository-name.git

# Push files to GitHub
git push -u origin main
```

---

# 2. Rectangle Area Program

```sql
DECLARE
    length NUMBER := 10;
    width NUMBER := 5;
    area NUMBER;
BEGIN
    area := length * width;
    DBMS_OUTPUT.PUT_LINE('Rectangle Area = ' || area);
END;
/
```

---

# 3. Find the Average of Three Numbers

```sql
DECLARE
    num1 NUMBER := 10;
    num2 NUMBER := 20;
    num3 NUMBER := 30;
    average NUMBER;
BEGIN
    average := (num1 + num2 + num3) / 3;
    DBMS_OUTPUT.PUT_LINE('Average = ' || average);
END;
/
```

---

# 4. Square Area Program

```sql
DECLARE
    side NUMBER := 8;
    area NUMBER;
BEGIN
    area := side * side;
    DBMS_OUTPUT.PUT_LINE('Square Area = ' || area);
END;
/
```

---

# 5. Find the Largest Number among Three Numbers

```sql
DECLARE
    num1 NUMBER := 25;
    num2 NUMBER := 40;
    num3 NUMBER := 15;
BEGIN
    IF num1 >= num2 AND num1 >= num3 THEN
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || num1);
    ELSIF num2 >= num1 AND num2 >= num3 THEN
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || num2);
    ELSE
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || num3);
    END IF;
END;
/
```

---

# 6. Find the Smallest Number among Three Numbers

```sql
DECLARE
    num1 NUMBER := 25;
    num2 NUMBER := 40;
    num3 NUMBER := 15;
BEGIN
    IF num1 <= num2 AND num1 <= num3 THEN
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || num1);
    ELSIF num2 <= num1 AND num2 <= num3 THEN
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || num2);
    ELSE
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || num3);
    END IF;
END;
/
```

---

# 7. Even and Odd Number Program

```sql
DECLARE
    num NUMBER := 12;
BEGIN
    IF MOD(num, 2) = 0 THEN
        DBMS_OUTPUT.PUT_LINE(num || ' is Even');
    ELSE
        DBMS_OUTPUT.PUT_LINE(num || ' is Odd');
    END IF;
END;
/
```

---

# 8. Simple Calculator Program

```sql
DECLARE
    num1 NUMBER := 20;
    num2 NUMBER := 10;
    addition NUMBER;
    subtraction NUMBER;
    multiplication NUMBER;
    division NUMBER;
BEGIN
    addition := num1 + num2;
    subtraction := num1 - num2;
    multiplication := num1 * num2;
    division := num1 / num2;

    DBMS_OUTPUT.PUT_LINE('Addition = ' || addition);
    DBMS_OUTPUT.PUT_LINE('Subtraction = ' || subtraction);
    DBMS_OUTPUT.PUT_LINE('Multiplication = ' || multiplication);
    DBMS_OUTPUT.PUT_LINE('Division = ' || division);
END;
/
```

---

# 9. Celsius to Fahrenheit Conversion Program

```sql
DECLARE
    celsius NUMBER := 30;
    fahrenheit NUMBER;
BEGIN
    fahrenheit := (celsius * 9/5) + 32;
    DBMS_OUTPUT.PUT_LINE('Fahrenheit = ' || fahrenheit);
END;
/
```

---

# 10. Student Grade Calculation Program

```sql
DECLARE
    marks NUMBER := 85;
    grade VARCHAR2(2);
BEGIN
    IF marks >= 90 THEN
        grade := 'A';
    ELSIF marks >= 80 THEN
        grade := 'B';
    ELSIF marks >= 70 THEN
        grade := 'C';
    ELSIF marks >= 60 THEN
        grade := 'D';
    ELSE
        grade := 'F';
    END IF;

    DBMS_OUTPUT.PUT_LINE('Grade = ' || grade);
END;
/
```

---

# 11. Find the Sum from 1 to 100

```sql
DECLARE
    total NUMBER := 0;
    i NUMBER;
BEGIN
    FOR i IN 1..100 LOOP
        total := total + i;
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('Sum = ' || total);
END;
/
```

---

# 12. Find the Factorial of a Number

```sql
DECLARE
    num NUMBER := 5;
    factorial NUMBER := 1;
    i NUMBER;
BEGIN
    FOR i IN 1..num LOOP
        factorial := factorial * i;
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('Factorial = ' || factorial);
END;
/
```

---

# 13. Electricity Bill Calculation Program

```sql
DECLARE
    units NUMBER := 250;
    bill NUMBER;
BEGIN
    IF units <= 100 THEN
        bill := units * 2;
    ELSIF units <= 200 THEN
        bill := (100 * 2) + ((units - 100) * 3);
    ELSE
        bill := (100 * 2) + (100 * 3) + ((units - 200) * 5);
    END IF;

    DBMS_OUTPUT.PUT_LINE('Electricity Bill = ' || bill);
END;
/
```

---

# How to Run PL/SQL Programs

```sql
SET SERVEROUTPUT ON;
```

Then run each program one by one in Oracle SQL Developer or any PL/SQL environment.
