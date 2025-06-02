# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

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
![image](https://github.com/user-attachments/assets/34d070b0-f456-4e19-beba-4184c68479bd)

## RESULT
The program demonstrates dictionary operations and iteration to calculate total marks of each student and identify the student with the highest total (topper). It prints both the total marks and the topper's name along with their score accordingly.
