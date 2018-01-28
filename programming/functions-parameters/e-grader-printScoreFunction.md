#### Exercise : Grader - `print_score` Function

The code below prints the grade based on exam and project score, somewhat similar to <trigger trigger="click" for="modal:printScoreFunction-gradeAnalyzer">a previous exercise you did</trigger>.
```python
project_score = int(input('Enter project score:'))
exam_score = int(input('Enter exam score:'))
total = project_score + exam_score
print('Total:', total)

if total >= 60 and project_score >= 25 and exam_score >= 25:
    grade = 'A'
elif (total >= 50) and (project_score >= 25 or exam_score >= 25):
    grade = 'B'
elif total >= 40:
    grade = 'C'
else:
    grade = 'D'

print('Project :', '=' * (project_score//5))
print('Exam    :', '=' * (exam_score//5))
print('Total   :', '=' * (total//5))
print('Grade   :', grade)
```
Add a `print_score` function to the code and replace the following three lines,
  
```python
print('Project :', '=' * (project_score//5))
print('Exam    :', '=' * (exam_score//5))
print('Total   :', '=' * (total//5))
```

with these three lines
  
```python
print_score('Project :', project_score)
print_score('Exam    :', exam_score)
print_score('Total   :', total)
```
without changing the external behavior of the program.

<modal large title="" id="modal:printScoreFunction-gradeAnalyzer">
  <include src="../if/e-grades.md"/>
</modal>