# python-subject-wise-topper

## Project Description

This project is a simple Python program that finds the topper of each subject from the marks of three students.

It uses a nested dictionary to store student names and their subject-wise marks. The program uses `for` loops and `if` conditions to find the highest marks in Physics, Chemistry, and Mathematics.

## Students and Marks

| Student | Physics | Chemistry | Mathematics |
|---|---:|---:|---:|
| Jayesh | 83 | 82 | 85 |
| Sumit | 74 | 81 | 87 |
| Pavan | 77 | 84 | 86 |

## Concepts Used

- Python Dictionary
- Nested Dictionary
- For Loop
- If Condition
- Dictionary `items()` Method
- Maximum Marks Comparison

## Source Code

```python
db = {
    "jayesh": {"Phy": 83, "Che": 82, "Mat": 85},
    "sumit": {"Phy": 74, "Che": 81, "Mat": 87},
    "pavan": {"Phy": 77, "Che": 84, "Mat": 86}
}

for sub in ["Phy", "Che", "Mat"]:
    max_marks = 0
    topper = 0

    for student, marks in db.items():
        if marks[sub] > max_marks:
            max_marks = marks[sub]
            topper = student

    print("Topper-", topper, "|", "subject=", sub, max_marks)
```

## Output

```text
Topper- jayesh | subject= Phy 83
Topper- pavan | subject= Che 84
Topper- sumit | subject= Mat 87
```

## How It Works

1. Store student names and marks in a nested dictionary.
2. Select each subject using a `for` loop.
3. Initialize `max_marks` and `topper`.
4. Check each student's marks using another `for` loop.
5. Update the highest marks and topper when higher marks are found.
6. Print the topper of each subject.

## Conclusion

This project demonstrates how to use nested dictionaries, loops, and conditional statements in Python to find subject-wise toppers.

## Author

**Mrudul Pawar**
