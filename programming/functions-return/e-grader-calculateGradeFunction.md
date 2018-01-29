#### Exercise : Grader - `calculate_grade` Function

In a previous exercise you wrote a function to print scores (an example solution is given below).
```python
def print_score(name, value):
  print(name, '=' * (value//5))
  
def calculate_grade(project, exam):
  if total_score >= 60 and project >= 25 and exam >= 25:
    return 'A'
  elif (total_score >= 50) and (project >= 25 or exam >= 25):
    return 'B'
  elif total_score >= 40:
    return 'C'
  else:
    return 'D'

project_score = int(input('Enter project score:'))
exam_score = int(input('Enter exam score:'))

total_score = project_score + exam_score
print('Total:', total_score)

grade = calculate_grade(project_score, exam_score)

print_score('Project :', project_score)
print_score('Exam    :', exam_score)
print_score('Total   :', total_score)
print('Grade   :', grade)
```
Add a `calculate_grade` function to the code and replace the following lines,
  
```python
if total >= 60 and project_score >= 25 and exam_score >= 25:
    grade = 'A'
elif (total >= 50) and (project_score >= 25 or exam_score >= 25):
    grade = 'B'
elif total >= 40:
    grade = 'C'
else:
    grade = 'D'
```

with the line,
  
```python
grade = calculate_grade(project_score, exam_score)
```
without changing the external behavior of the program.