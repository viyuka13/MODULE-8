# 🏆 Hackerrank:Runner-Up Score Finder in Python

## 🎯 AIM:
To write a Python program that takes a list of scores from participants and finds the **runner-up score** (i.e., the second-highest score), eliminating any duplicates.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a variable `n` and get its value from the user (number of participants)
3. Read the list of `n` scores from the user using `input().split()` and convert them to integers
4. Store the scores in a list
5. Use `set()` to remove any duplicate scores
6. Convert the set back to a list and sort it in ascending order
7. Print the second-last element of the sorted list (i.e., the runner-up score)
8. **Stop**

---

## 💻 PROGRAM:
    student_marks = {
        "Alice": [85, 90, 78, 92, 88],
        "Bob": [75, 80, 70, 85, 90],
        "Charlie": [95, 85, 82, 87, 91],
        "David": [65, 70, 60, 75, 68]
    }
    
    total_marks = {}
    
    for student, marks in student_marks.items():
        total_marks[student] = sum(marks)
    
    topper = max(total_marks, key=total_marks.get)
    
    print("Total Marks of Each Student:", total_marks)
    print("Topper:", topper, "with a score of", total_marks[topper])
## OUTPUT
![image](https://github.com/user-attachments/assets/b1af693c-7190-4a7a-a6f2-3e2c0447c596)

## RESULT
The program demonstrates dictionary operations and iteration to calculate total marks of each student and identify the student with the highest total (topper). It prints both the total marks and the topper's name along with their score accordingly.
