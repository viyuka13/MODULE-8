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
    n = int(input())
    students = []
    
    for _ in range(n):
        name = input()
        grade = float(input())
        students.append([name, grade])
    
    grades = sorted(set([grade for name, grade in students]))
    second_lowest = grades[1]
    
    second_lowest_students = [name for name, grade in students if grade == second_lowest]
    second_lowest_students.sort()
    
    for student in second_lowest_students:
        print(student)

## Output
![image](https://github.com/user-attachments/assets/d30ee282-2365-436a-81e3-c8b568dc6164)

## Result
The program reads student names and grades, identifies the second lowest grade, and prints all student names who have that grade in alphabetical order, each on a new line, demonstrating list handling, sorting, and filtering operations.

