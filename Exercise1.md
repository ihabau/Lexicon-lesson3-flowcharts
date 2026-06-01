Write a program that asks the user to enter their age.

- If the age is **18 or older**, display: "You are eligible to vote."
- If the age is **less than 18**, display: "You are not eligible to vote."
- End the program.

**Pseudocode**

```
start
input age
if age >= 18
output You are eligible to vote.
else
You are not eligible to vote.
endif
end
```

**Flowchart**

```mermaid
graph TD
A((start)) --> B{Input age}
B --> C[/if age >= 18/]
C -- Yes --> D{You are eligible to vote.}
C -- No --> E{You are not eligible to vote.}
E --> F((end))
D --> F((end))
```
