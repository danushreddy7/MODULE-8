# 🎓 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---

## 🎯 Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## 🧠 Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

## 💻  Program
```
students = [
    ("Alice", 85),
    ("Bob", 75),
    ("Charlie", 90),
    ("David", 75),
    ("Eva", 80),
    ("Frank", 85)
]
grades = [grade for name, grade in students]
unique_grades = sorted(set(grades))  # Remove duplicates and sort the grades
second_lowest_grade = unique_grades[1]  
students_with_second_lowest = [name for name, grade in students if grade == second_lowest_grade]
students_with_second_lowest.sort()
print("Students with the second lowest grade:")
for student in students_with_second_lowest:
    print(student)

```
## Output:
```
Input                                Result
 [("Alice", 85),
    ("Bob", 75),
    ("Charlie", 90),              [("Alice", 85), ("Bob", 75), ("Charlie", 90), ("David", 75), ("Eva", 80), ("Frank", 85)]
    ("David", 75),
    ("Eva", 80),
    ("Frank", 85)]
```
## Result:
The program was successful.

