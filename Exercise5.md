#### Exercise 5: Smart Parking Fee Calculator

Write a program that calculates the parking fee for a city garage:

1. Ask the user for the **number of hours** parked (e.g., 4).
2. If the time is **1 hour or less**, the fee is **0 kr** (Free).
3. If the time is **between 1 and 3 hours**, the fee is a flat **50 kr**.
4. If the time is **more than 3 hours**, calculate the fee as: **50 kr + (40 kr for every hour beyond the 3rd hour)**.
5. If the calculated fee is **greater than 250 kr**, set the fee to **250 kr** (Maximum Daily Rate).
6. Ask if the user has a **"Loyalty Card"**. If **Yes**, subtract **20%** from the fee.
7. Display the **Final Fee** and end the program.

**Pseudocode:**

```
Start
input parkedHoures
if parkedHoures <= 1
 fee = 0
elseIf parkedHoures >= 1 && parkedHoures < 3
 fee = 50
else
 fee = (parkedHoures - 3) * 40 + 50
endIf
if fee > 250
 fee = 250
endIf
input loyalCard
if loyalCard
 fee * 0.8
endIf
End
```

**Flowchart**

```mermaid
graph TD
S((Start)) --> input[/pt = park time/]
input -->pt0{if pt <= 1} -- Yes --> res1(result == 0(
pt0 -- No --> pt1{if pt <= 3} -- Yes --> res2(result == 50(
pt1 -- No --> pt2{pt > 3} --> pt3{if result > 250} -- No --> res3[ result = (pt - 3) * 50 + 40 ]
pt3 -- Yes --> res4(result == 250(
res1 --> out[/final fee/] --> E((End))
res2 --> out[/final fee/] --> E((End))
res3 --> out[/final fee/] --> E((End))
res4 --> out[/final fee/] --> E((End))
```
