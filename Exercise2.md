### Write a program that takes a student's marks (out of 100) as input and determines their grade

- **90 or above:** "Grade A"
- **75 to 89:** "Grade B"
- **50 to 74:** "Grade C"
- **Below 50:** "Fail"
- End the program.

**Pseudocode:**

```
Start
input marks
if grade >= 90
  output Grade A
elseIf grade > 75 and marks < 89
  output Grade B
elseIf grade > 50 and marks < 74
  output Grade C
else grade < 50
  output Grade FAil
EndIf
End

```

**Flowchart**

```mermaid
graph TD
A((start)) --> B[/grade = Input: grade/]
B --> C{if grade >= 90} -- Yes ---> D[/output: Grade A/] --> K((End))
C -- No --> E{ if grade > 75 && grade < 89} -- Yes --> F[/output: Grade B/] --> K((End))
E -- No --> G{ if grade > 50 && grade < 74} -- Yes --> H[/output: Grade C/] --> K((End))
G -- No ---> J[/output: Fail/] --> K((End))
```
