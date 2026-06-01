#### Exercise 3: Simple Password Check

Write a program that:

1. Asks the user to enter a password.
2. Compares it with a stored password (e.g., "12345").
3. If they match, display: "Access Granted."
4. If they don't match, display: "Access Denied."
5. End the program.

**Pseudocode:**

```
Start
Input password
if password == 12345
  output Access Granted.
else output Access Denied.
End

```

**Flowchart**

```mermaid
graph TD
A((start)) --> B[/Input password/]
C(12345( <-- D{if B = C}
D -- Yes --> E[/Access Granted./] --> G((End))
D -- No --> F[/Access Denied./] --> G
```
