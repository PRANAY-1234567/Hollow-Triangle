📘 Hollow Pyramid Star Pattern in Python

📌 Overview

This Python program prints a Hollow Pyramid Star (*) Pattern using nested loops and conditional statements.

Unlike a filled pyramid, this pattern prints stars only at the boundaries of the pyramid and leaves spaces inside, creating a hollow structure.

This example demonstrates important programming concepts such as nested loops, conditional logic, and pattern formatting.

⚙️ Source Code

n = 4

for i in range(1, n+1):
    print(" " * (n - i), end=" ")

    for j in range(1, 2*i):
        if j == 1 or j == 2*i - 1 or i == n:
            print("*", end=" ")
        else:
            print(" ", end=" ")

    print()
🧠 How It Works
1️⃣ Define Number of Rows
n = 4

This variable controls the height of the pyramid.

2️⃣ Outer Loop – Controls Rows
for i in range(1, n+1):

Iterates from 1 to n

Each iteration prints one row of the pyramid.

3️⃣ Print Leading Spaces
print(" " * (n - i), end=" ")

Adds spaces before the stars

Keeps the pyramid center aligned.

4️⃣ Inner Loop – Controls Columns
for j in range(1, 2*i):

Prints elements across the row

Total positions follow the formula:

2*i - 1

This ensures the pyramid expands symmetrically.

5️⃣ Boundary Condition
if j == 1 or j == 2*i - 1 or i == n:

Stars are printed when:

j == 1 → Left edge of pyramid

j == 2*i - 1 → Right edge of pyramid

i == n → Last row (completely filled)

Otherwise, spaces are printed to create the hollow interior.

▶️ Sample Output
    * 
   * * 
  *   * 
 * * * * * * *
🔑 Key Concepts Demonstrated

Nested loops

Conditional statements (if-else)

Pattern design using mathematics

String multiplication

Console formatting

⏱️ Time Complexity

O(n²)
Each row contains multiple column operations.

🚀 Customization

You can increase the pyramid size by modifying:

n = 6

Example larger pyramid:

     *
    * *
   *   *
  *     *
 *       *
* * * * * * * * *
📚 Learning Outcomes

After studying this program, you will understand:

How to create hollow geometric patterns

How to combine loops with conditional logic

How to control alignment and spacing in console output

How mathematical formulas help design patterns
