# 10-Day C Programming Curriculum for Non-IT Background Students
## Building Programming Mindset Foundation

**Program Structure:** 1 hour 15 minutes per day (75 minutes) | 10 consecutive days

**Total Investment:** 12.5 hours of focused learning  
**Expected Outcome:** Complete programming mindset, ability to write functional C programs, ready for Java full-stack development

---

## **Day 1: Introduction & Setup - Building the Foundation**

**Time: 75 minutes**  
**Objective:** Understand what programming is, set up environment, write and run first program

### **Content Breakdown (75 min):**

#### **Concept Introduction (15 min):**
- What is programming? (Simple analogy: Recipe for cooking - step-by-step instructions)
- Why learn C? (Foundation for all languages, teaches real programming concepts)
- C in real world (Operating systems, embedded systems, games, databases)
- History and importance of C

#### **Environment Setup (25 min):**

**Option 1 (Recommended for beginners):** Online IDE
- Platform: Replit.com or OnlineGDB.com
- Advantages: No installation, works on any device, browser-based
- Quick start: Sign up → Create project → Start coding

**Option 2:** Install CodeBlocks IDE locally
- Installation time: 10 minutes
- Advantages: Works offline, faster execution
- Steps: Download → Install → Configure compiler

#### **First Program - "Hello World" (25 min):**

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

**Explanation breakdown:**
- `#include <stdio.h>` = Import standard input-output library (like borrowing tools)
- `int main()` = Main function - starting point of program (like opening a book at page 1)
- `printf()` = Print on screen (output command)
- `return 0;` = Program ends successfully (0 = success)
- `\n` = New line character (move to next line)
- Curly braces `{}` = Block of code

#### **Hands-On Practice (10 min):**
- Modify the program to print your name
- Print multiple lines (name, city, country)
- **Confidence Builder:** "You just wrote your first program!"

---

### **Day 1 Practice Questions:**

**Easy:**
1. Write a program that prints your full name
2. Modify "Hello World" to print "Welcome to C Programming"
3. Write a program that prints:
   ```
   C Programming
   Is Fun!
   Let's Learn!
   ```

**Medium:**
4. Write a program that prints your bio:
   ```
   Name: [Your Name]
   City: [Your City]
   Country: [Your Country]
   ```
5. Create a program that prints a simple ASCII art (like a box with stars)
   ```
   ****
   *  *
   *  *
   ****
   ```

**Challenge:**
6. Write a program that prints this pattern:
   ```
   *
   * *
   * * *
   * * * *
   * * * * *
   ```

### **Day 1 Task (Assignment):**
Write a program that prints:
```
========================================
  Welcome to My Programming Journey!
========================================
My name is [Your Name]
I am learning C programming
Today is Day 1 of my 10-day bootcamp
I will become a programmer!
========================================
```

---

## **Day 2: Variables, Data Types & Basic Input/Output**

**Time: 75 minutes**  
**Objective:** Store and use data, take input from user, perform calculations

### **Content Breakdown (75 min):**

#### **Concept Introduction (15 min):**
- Variables = labeled storage boxes for data
- Why different types? Memory efficiency, type safety, proper operations
- Data Types:
  - `int` = integers (whole numbers: 5, -10, 100, 0)
  - `float` = floating-point (decimals: 3.14, 2.5, -0.001)
  - `double` = double precision (more accurate decimals)
  - `char` = single character ('A', 'x', '5', '!')

#### **Variable Declaration & Initialization (15 min):**

```c
#include <stdio.h>

int main() {
    // Declaration
    int age;
    float height;
    char grade;
    
    // Initialization (assignment)
    age = 20;
    height = 5.9;
    grade = 'A';
    
    // Declaration + Initialization
    int marks = 95;
    
    // Multiple variables same type
    int a = 10, b = 20, c = 30;
    
    return 0;
}
```

#### **Output with printf (10 min):**

```c
#include <stdio.h>

int main() {
    int age = 25;
    float height = 5.8;
    char name[] = "Alice";
    
    printf("Name: %s\n", name);
    printf("Age: %d\n", age);
    printf("Height: %f meters\n", height);
    printf("Height: %.2f meters\n", height);  // 2 decimal places
    
    return 0;
}
```

**Format Specifiers:**
- `%d` = integer
- `%f` = float (default 6 decimals)
- `%.2f` = float with 2 decimals
- `%c` = character
- `%s` = string

#### **Taking Input (15 min):**

```c
#include <stdio.h>

int main() {
    int age;
    float height;
    char grade;
    
    printf("Enter your age: ");
    scanf("%d", &age);
    
    printf("Enter your height in meters: ");
    scanf("%f", &height);
    
    printf("Enter your grade: ");
    scanf(" %c", &grade);  // Space before %c important!
    
    printf("\nYou are %d years old, %.2f tall, Grade: %c\n", age, height, grade);
    
    return 0;
}
```

**Key Points:**
- `scanf()` = Take input from keyboard
- `%d`, `%f`, `%c` = Format specifiers
- `&` = Address-of operator (where to store the value)

#### **Basic Calculations (15 min):**

```c
#include <stdio.h>

int main() {
    int num1 = 10;
    int num2 = 5;
    
    printf("Addition: %d + %d = %d\n", num1, num2, num1 + num2);
    printf("Subtraction: %d - %d = %d\n", num1, num2, num1 - num2);
    printf("Multiplication: %d * %d = %d\n", num1, num2, num1 * num2);
    printf("Division: %d / %d = %d\n", num1, num2, num1 / num2);
    printf("Modulus (remainder): %d %% %d = %d\n", num1, num2, num1 % num2);
    
    return 0;
}
```

**Operators:**
- `+` Addition
- `-` Subtraction
- `*` Multiplication
- `/` Division
- `%` Modulus (remainder)

---

### **Day 2 Practice Questions:**

**Easy:**
1. Write a program that takes two numbers and prints their sum
2. Create a program that takes length and width, calculates area of rectangle
3. Write a program that converts Fahrenheit to Celsius (C = (F - 32) * 5/9)

**Medium:**
4. Take marks in 3 subjects as input, calculate average:
   ```
   Enter marks in Math: 85
   Enter marks in Science: 90
   Enter marks in English: 78
   Average: 84.33
   ```

5. Create a simple interest calculator:
   - Principal, rate, time as input
   - Formula: SI = (P * R * T) / 100
   - Print simple interest

**Challenge:**
6. BMI (Body Mass Index) calculator:
   - Take weight (kg) and height (m) as input
   - BMI = weight / (height * height)
   - Print category: Underweight (<18.5), Normal (18.5-24.9), Overweight (25-29.9), Obese (>30)

### **Day 2 Task (Assignment):**
Create a program that:
1. Takes user's name as input
2. Takes marks in 3 subjects (Math, Science, English)
3. Calculates total and average
4. Prints:
   ```
   Name: [Name]
   Math: [marks]
   Science: [marks]
   English: [marks]
   Total: [total]
   Average: [average]
   ```

---

## **Day 3: Decision Making - If/Else Statements**

**Time: 75 minutes**  
**Objective:** Make programs that make decisions using conditional logic

### **Content Breakdown (75 min):**

#### **Concept Introduction (10 min):**
- Decisions in programming = if-else statements
- Real-life example: "If it's raining, take umbrella. Else, don't."
- Computers make decisions based on conditions (true/false)

#### **Comparison Operators (10 min):**
- `==` Equal to (5 == 5 is true)
- `!=` Not equal to (5 != 3 is true)
- `>` Greater than (10 > 5 is true)
- `<` Less than (5 < 10 is true)
- `>=` Greater than or equal to
- `<=` Less than or equal to

#### **If Statement (15 min):**

```c
#include <stdio.h>

int main() {
    int age = 20;
    
    if (age >= 18) {
        printf("You are an adult\n");
    }
    
    return 0;
}
```

**Logic:** If condition is TRUE, execute code inside braces

#### **If-Else Statement (15 min):**

```c
#include <stdio.h>

int main() {
    int marks = 45;
    
    if (marks >= 50) {
        printf("Pass\n");
    } else {
        printf("Fail\n");
    }
    
    return 0;
}
```

**Logic:** If TRUE, execute first block; else execute second block

#### **If-Else If-Else (Multiple Conditions) (15 min):**

```c
#include <stdio.h>

int main() {
    int marks = 75;
    
    if (marks >= 90) {
        printf("Grade: A\n");
    } else if (marks >= 75) {
        printf("Grade: B\n");
    } else if (marks >= 50) {
        printf("Grade: C\n");
    } else {
        printf("Grade: F - Fail\n");
    }
    
    return 0;
}
```

#### **Logical Operators (10 min):**

```c
// AND (&&) - both conditions must be true
if (age >= 18 && age <= 60) {
    printf("Working age\n");
}

// OR (||) - at least one condition must be true
if (marks >= 75 || attendance >= 80) {
    printf("Eligible for exam\n");
}

// NOT (!) - reverses condition
if (!(marks < 50)) {
    printf("Pass\n");
}
```

---

### **Day 3 Practice Questions:**

**Easy:**
1. Check if a number is positive or negative
2. Check if a person can vote (age >= 18)
3. Check if a number is even or odd (number % 2 == 0)

**Medium:**
4. Grade calculator based on marks:
   - 90-100: A
   - 75-89: B
   - 50-74: C
   - <50: F
   
5. Age category classifier:
   ```
   <13: Child
   13-19: Teenager
   20-60: Adult
   >60: Senior
   ```

**Challenge:**
6. Triangle validator:
   - Take 3 sides as input
   - Check if it forms a valid triangle (sum of any 2 sides > 3rd side)
   - If valid, check if equilateral (all sides equal), isosceles (2 sides equal), or scalene (all different)

### **Day 3 Task (Assignment):**
Create a program that:
1. Takes a student's marks as input
2. Assigns grade: A (90+), B (75-89), C (50-74), F (<50)
3. Takes attendance percentage as input
4. Prints:
   ```
   Marks: [X]
   Grade: [X]
   Attendance: [X]%
   Status: [Eligible/Ineligible for exam]
   ```
   (Eligible only if marks >= 50 AND attendance >= 75%)

---

## **Day 4: Loops - Repeating Code**

**Time: 75 minutes**  
**Objective:** Repeat code without rewriting using loops

### **Content Breakdown (75 min):**

#### **Why Loops? (10 min):**
- Without loop: Print numbers 1-100 needs 100 printf statements
- With loop: Repeat code 100 times automatically
- Saves time, reduces errors, makes code clean

#### **For Loop (20 min):**

```c
#include <stdio.h>

int main() {
    // Print numbers 1 to 10
    for (int i = 1; i <= 10; i++) {
        printf("%d\n", i);
    }
    
    return 0;
}
```

**Breaking down for loop:**
- `int i = 1` = Initialization (starting value)
- `i <= 10` = Condition (keep looping while true)
- `i++` = Increment (increase i by 1 after each iteration)
- Loop executes: 1, 2, 3, ..., 10 (stops when i > 10)

#### **While Loop (15 min):**

```c
#include <stdio.h>

int main() {
    int i = 1;
    
    while (i <= 10) {
        printf("%d\n", i);
        i++;  // Very important - increment to avoid infinite loop!
    }
    
    return 0;
}
```

**Key Difference:**
- For loop: When you know exact number of iterations
- While loop: When you loop based on condition

#### **Do-While Loop (10 min):**

```c
#include <stdio.h>

int main() {
    int i = 1;
    
    do {
        printf("%d\n", i);
        i++;
    } while (i <= 10);
    
    return 0;
}
```

**Key Difference:** Do-while executes at least once, even if condition is false

#### **Loop Control - Break & Continue (10 min):**

```c
// Break - exits loop immediately
for (int i = 1; i <= 10; i++) {
    if (i == 5) break;  // Stop when i reaches 5
    printf("%d ", i);   // Prints: 1 2 3 4
}

// Continue - skip current iteration
for (int i = 1; i <= 10; i++) {
    if (i % 2 == 0) continue;  // Skip even numbers
    printf("%d ", i);   // Prints: 1 3 5 7 9
}
```

#### **Nested Loops (10 min):**

```c
#include <stdio.h>

int main() {
    // Print multiplication table
    for (int i = 1; i <= 3; i++) {
        for (int j = 1; j <= 3; j++) {
            printf("%d ", i * j);
        }
        printf("\n");
    }
    
    // Output:
    // 1 2 3
    // 2 4 6
    // 3 6 9
    
    return 0;
}
```

---

### **Day 4 Practice Questions:**

**Easy:**
1. Print numbers 1-50
2. Print first 10 even numbers (2, 4, 6, ...)
3. Print first 10 odd numbers (1, 3, 5, ...)
4. Print multiplication table of any number

**Medium:**
5. Print sum of first N natural numbers:
   ```
   Enter N: 5
   Sum of 1+2+3+4+5 = 15
   ```

6. Count down from 10 to 1
7. Print Fibonacci series (0, 1, 1, 2, 3, 5, 8, ...)

**Challenge:**
8. Print pattern:
   ```
   *
   * *
   * * *
   * * * *
   * * * * *
   ```

9. Print this pattern:
   ```
   1
   1 2
   1 2 3
   1 2 3 4
   1 2 3 4 5
   ```

10. Find factorial of a number (5! = 5 * 4 * 3 * 2 * 1 = 120)

### **Day 4 Task (Assignment):**
Create a program that:
1. Takes a number as input
2. Prints multiplication table (1 to 10)
3. Prints sum of all multiples
4. Example:
   ```
   Enter number: 5
   5 x 1 = 5
   5 x 2 = 10
   ...
   5 x 10 = 50
   Sum of all multiples: 275
   ```

---

## **Day 5: Functions - Breaking Code into Reusable Pieces**

**Time: 75 minutes**  
**Objective:** Create reusable code blocks and understand function structure

### **Content Breakdown (75 min):**

#### **Why Functions? (10 min):**
- Real-world analogy: Recipe for making tea
- Write once, use 100 times (DRY principle - Don't Repeat Yourself)
- Code becomes organized, reusable, maintainable, testable
- Large programs broken into manageable chunks

#### **Function Structure (15 min):**

```c
#include <stdio.h>

// Function declaration (prototype)
int add(int a, int b);

int main() {
    // Function call
    int result = add(5, 3);
    printf("Sum: %d\n", result);
    return 0;
}

// Function definition
int add(int a, int b) {
    return a + b;
}
```

**Parts:**
- **Return type:** `int` (what function returns)
- **Function name:** `add`
- **Parameters:** `(int a, int b)` (inputs)
- **Function body:** Code inside braces
- **Return statement:** Send result back

#### **Multiple Functions (15 min):**

```c
#include <stdio.h>

int multiply(int x, int y) {
    return x * y;
}

float divide(float x, float y) {
    if (y != 0)
        return x / y;
    else
        return 0;
}

int main() {
    printf("Multiply: %d\n", multiply(5, 4));      // 20
    printf("Divide: %f\n", divide(20.0, 4.0));     // 5.0
    return 0;
}
```

#### **Void Functions (No Return Value) (15 min):**

```c
#include <stdio.h>

// Function that doesn't return anything
void greet(char name[]) {
    printf("Hello, %s!\n", name);
}

void printLine() {
    printf("========================\n");
}

int main() {
    printLine();
    greet("Alice");
    greet("Bob");
    printLine();
    return 0;
}
```

#### **Local vs Global Variables (10 min):**

```c
#include <stdio.h>

int globalVar = 100;  // Global - accessible everywhere

int main() {
    int localVar = 50;  // Local - only in main()
    
    printf("Global: %d\n", globalVar);  // Works
    printf("Local: %d\n", localVar);    // Works
    
    return 0;
}

void someFunction() {
    printf("%d\n", globalVar);  // Works
    printf("%d\n", localVar);   // ERROR - localVar doesn't exist here
}
```

#### **Function with Multiple Parameters (10 min):**

```c
#include <stdio.h>

// Calculate area of rectangle
int rectangleArea(int length, int width) {
    return length * width;
}

// Calculate area of circle
float circleArea(float radius) {
    return 3.14 * radius * radius;
}

int main() {
    printf("Rectangle area: %d\n", rectangleArea(5, 3));    // 15
    printf("Circle area: %f\n", circleArea(5.0));           // 78.5
    return 0;
}
```

---

### **Day 5 Practice Questions:**

**Easy:**
1. Create function to calculate square of a number
2. Create function to check if number is even or odd
3. Create function that prints "Welcome" 5 times

**Medium:**
4. Create function to calculate power (2^5 = 32)
   ```c
   int power(int base, int exponent)
   ```

5. Create function to check if number is prime
   ```c
   int isPrime(int n)
   ```

6. Create functions for basic arithmetic:
   ```c
   int add(int a, int b)
   int subtract(int a, int b)
   int multiply(int a, int b)
   float divide(float a, float b)
   ```

**Challenge:**
7. Create function to calculate factorial of a number
   ```c
   int factorial(int n)
   ```

8. Create function to print Fibonacci series
   ```c
   void fibonacci(int count)
   ```

### **Day 5 Task (Assignment):**
Create a program with these functions:
1. `int factorial(int n)` - Calculate factorial
2. `int isPrime(int n)` - Check if prime (return 1 if prime, 0 if not)
3. `int sumOfDigits(int n)` - Calculate sum of digits (123 → 1+2+3 = 6)
4. Call all functions from main() with user inputs

Example output:
```
Enter number: 5
Factorial of 5: 120
Is 5 prime? Yes
Sum of digits in 5: 5
```

---

## **Day 6: Arrays - Storing Multiple Values**

**Time: 75 minutes**  
**Objective:** Store and manipulate multiple values of same type

### **Content Breakdown (75 min):**

#### **Why Arrays? (10 min):**
- Store 100 marks? Create 100 variables? NO!
- Use 1 array: `int marks[100]`
- Arrays organize data efficiently

#### **Array Declaration & Initialization (15 min):**

```c
#include <stdio.h>

int main() {
    // Declaration with initialization
    int numbers[5] = {10, 20, 30, 40, 50};
    
    // Access elements (indexing starts at 0!)
    printf("First element: %d\n", numbers[0]);   // 10
    printf("Third element: %d\n", numbers[2]);   // 30
    printf("Last element: %d\n", numbers[4]);    // 50
    
    // Modify element
    numbers[2] = 99;
    printf("After modification: %d\n", numbers[2]);  // 99
    
    return 0;
}
```

**Important:** Array indexing starts at 0!
- Index 0 = first element
- Index 4 = fifth element
- Index [n-1] = last element

#### **Array with Loop (20 min):**

```c
#include <stdio.h>

int main() {
    int marks[5];
    
    // Input marks
    printf("Enter 5 marks:\n");
    for (int i = 0; i < 5; i++) {
        printf("Enter mark %d: ", i + 1);
        scanf("%d", &marks[i]);
    }
    
    // Print marks
    printf("\nYour marks:\n");
    for (int i = 0; i < 5; i++) {
        printf("Mark %d: %d\n", i + 1, marks[i]);
    }
    
    return 0;
}
```

#### **Calculate Statistics from Array (15 min):**

```c
#include <stdio.h>

int main() {
    int marks[5] = {85, 90, 78, 92, 88};
    int sum = 0;
    int max = marks[0];
    int min = marks[0];
    
    // Calculate sum
    for (int i = 0; i < 5; i++) {
        sum = sum + marks[i];
    }
    
    // Find max and min
    for (int i = 0; i < 5; i++) {
        if (marks[i] > max) max = marks[i];
        if (marks[i] < min) min = marks[i];
    }
    
    float average = sum / 5.0;
    
    printf("Sum: %d\n", sum);
    printf("Average: %f\n", average);
    printf("Maximum: %d\n", max);
    printf("Minimum: %d\n", min);
    
    return 0;
}
```

#### **2D Arrays (Multi-dimensional) (15 min):**

```c
#include <stdio.h>

int main() {
    // 3x3 matrix
    int matrix[3][3] = {
        {1, 2, 3},
        {4, 5, 6},
        {7, 8, 9}
    };
    
    // Access elements
    printf("%d\n", matrix[0][0]);  // 1
    printf("%d\n", matrix[1][1]);  // 5
    printf("%d\n", matrix[2][2]);  // 9
    
    // Print entire matrix
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            printf("%d ", matrix[i][j]);
        }
        printf("\n");
    }
    
    return 0;
}
```

---

### **Day 6 Practice Questions:**

**Easy:**
1. Take 5 numbers, print them in reverse order
2. Find sum and average of array
3. Find maximum and minimum in array

**Medium:**
4. Count how many numbers are greater than 50 in an array
5. Find second largest number in array
6. Swap elements: array[0] ↔ array[4], array[1] ↔ array[3]

**Challenge:**
7. Linear search: Search for a number in array
8. Bubble sort: Sort array in ascending order
9. Find duplicate elements in array
10. Array rotation: Rotate array by k positions

### **Day 6 Task (Assignment):**
Create a program that:
1. Takes 5 numbers as input
2. Finds maximum, minimum, average
3. Counts numbers > 50
4. Prints results:
   ```
   Numbers: 45 78 92 33 67
   Maximum: 92
   Minimum: 33
   Average: 63.0
   Count > 50: 3
   ```

---

## **Day 7: Strings - Working with Text**

**Time: 75 minutes**  
**Objective:** Store and manipulate text data

### **Content Breakdown (75 min):**

#### **What is String? (10 min):**
- String = array of characters
- Each character occupies 1 position
- String ends with special character '\0' (null terminator)
- Example: "Hello" stored as ['H','e','l','l','o','\0']

#### **String Declaration (15 min):**

```c
#include <stdio.h>

int main() {
    // String declaration
    char name[50] = "Alice";
    char city[50];  // Empty string
    
    // Print string
    printf("Name: %s\n", name);  // %s for string
    
    // Access individual characters
    printf("First character: %c\n", name[0]);   // A
    printf("Second character: %c\n", name[1]);  // l
    printf("Third character: %c\n", name[2]);   // i
    
    return 0;
}
```

#### **Taking String Input (20 min):**

```c
#include <stdio.h>

int main() {
    char name[50];
    char city[50];
    
    printf("Enter your name: ");
    scanf("%s", name);  // Note: No & for strings!
    
    printf("Enter your city: ");
    scanf("%s", city);
    
    printf("Hello, %s from %s!\n", name, city);
    
    return 0;
}
```

**Important:** For strings, `scanf("%s", name)` NOT `scanf("%s", &name)`

#### **String Functions (20 min):**

```c
#include <stdio.h>
#include <string.h>  // String library

int main() {
    char str1[50] = "Hello";
    char str2[50] = "World";
    char str3[50];
    
    // Length of string
    printf("Length of 'Hello': %lu\n", strlen(str1));  // 5
    
    // Copy string
    strcpy(str3, str1);
    printf("After copy: %s\n", str3);  // Hello
    
    // Compare strings
    if (strcmp("abc", "abc") == 0) {
        printf("Strings are equal\n");
    }
    
    // Concatenate strings
    strcat(str3, " ");
    strcat(str3, str2);
    printf("Concatenated: %s\n", str3);  // Hello World
    
    return 0;
}
```

**String Functions:**
- `strlen()` - Get length
- `strcpy()` - Copy string
- `strcat()` - Concatenate (join)
- `strcmp()` - Compare strings (0 = equal)
- `strrev()` - Reverse string

#### **Working with Individual Characters (10 min):**

```c
#include <stdio.h>
#include <string.h>

int main() {
    char str[50] = "Programming";
    int len = strlen(str);
    
    // Print each character
    printf("Characters: ");
    for (int i = 0; i < len; i++) {
        printf("%c ", str[i]);
    }
    printf("\n");
    
    // Print string in reverse
    printf("Reverse: ");
    for (int i = len - 1; i >= 0; i--) {
        printf("%c", str[i]);
    }
    printf("\n");
    
    return 0;
}
```

---

### **Day 7 Practice Questions:**

**Easy:**
1. Take a string, print its length
2. Print each character on new line
3. Check if two strings are equal
4. Copy one string to another

**Medium:**
5. Check if string is palindrome ("racecar" = yes, "hello" = no)
6. Count vowels in a string
7. Convert string to uppercase (or lowercase)
8. Concatenate two strings with a space

**Challenge:**
9. Count occurrences of a character in string
10. Check if string contains only digits
11. Remove spaces from string
12. Find longest word in a sentence

### **Day 7 Task (Assignment):**
Create a program that:
1. Takes a string (sentence) as input
2. Prints string length
3. Prints each character on new line
4. Prints string in reverse
5. Counts vowels (a, e, i, o, u)
6. Example:
   ```
   Enter string: Hello
   Length: 5
   Characters: H e l l o
   Reverse: olleH
   Vowels: 2
   ```

---

## **Day 8: Switch Statement & Complex Logic**

**Time: 75 minutes**  
**Objective:** Use switch for multiple conditions and solve real-world problems

### **Content Breakdown (75 min):**

#### **Switch vs If-Else (10 min):**

**If-Else approach (verbose):**
```c
int day = 3;
if (day == 1) printf("Monday");
else if (day == 2) printf("Tuesday");
else if (day == 3) printf("Wednesday");
else if (day == 4) printf("Thursday");
else printf("Other day");
```

**Switch approach (cleaner):**
```c
int day = 3;
switch(day) {
    case 1:
        printf("Monday");
        break;
    case 2:
        printf("Tuesday");
        break;
    // ... more cases
}
```

#### **Switch Statement Structure (15 min):**

```c
#include <stdio.h>

int main() {
    int day = 3;
    
    switch(day) {
        case 1:
            printf("Monday\n");
            break;  // Important - exit switch
        case 2:
            printf("Tuesday\n");
            break;
        case 3:
            printf("Wednesday\n");
            break;
        case 4:
            printf("Thursday\n");
            break;
        case 5:
            printf("Friday\n");
            break;
        case 6:
            printf("Saturday\n");
            break;
        case 7:
            printf("Sunday\n");
            break;
        default:
            printf("Invalid day\n");
    }
    
    return 0;
}
```

**Key Points:**
- `switch(variable)` - Check variable value
- `case value:` - If variable equals this value
- `break;` - Exit switch (IMPORTANT!)
- `default:` - If no case matches (like else)

#### **Calculator Program (20 min):**

```c
#include <stdio.h>

int main() {
    float num1, num2;
    char operator;
    
    printf("Enter first number: ");
    scanf("%f", &num1);
    
    printf("Enter operator (+, -, *, /): ");
    scanf(" %c", &operator);
    
    printf("Enter second number: ");
    scanf("%f", &num2);
    
    switch(operator) {
        case '+':
            printf("Result: %f\n", num1 + num2);
            break;
        case '-':
            printf("Result: %f\n", num1 - num2);
            break;
        case '*':
            printf("Result: %f\n", num1 * num2);
            break;
        case '/':
            if (num2 != 0)
                printf("Result: %f\n", num1 / num2);
            else
                printf("Cannot divide by zero\n");
            break;
        default:
            printf("Invalid operator\n");
    }
    
    return 0;
}
```

#### **Menu-Driven Program (20 min):**

```c
#include <stdio.h>

int main() {
    int choice;
    
    printf("===== Simple Menu =====\n");
    printf("1. Add two numbers\n");
    printf("2. Subtract two numbers\n");
    printf("3. Multiply two numbers\n");
    printf("4. Exit\n");
    printf("Enter your choice: ");
    scanf("%d", &choice);
    
    switch(choice) {
        case 1: {
            int a, b;
            printf("Enter two numbers: ");
            scanf("%d %d", &a, &b);
            printf("Sum: %d\n", a + b);
            break;
        }
        case 2: {
            int a, b;
            printf("Enter two numbers: ");
            scanf("%d %d", &a, &b);
            printf("Difference: %d\n", a - b);
            break;
        }
        case 3: {
            int a, b;
            printf("Enter two numbers: ");
            scanf("%d %d", &a, &b);
            printf("Product: %d\n", a * b);
            break;
        }
        case 4:
            printf("Exiting...\n");
            break;
        default:
            printf("Invalid choice\n");
    }
    
    return 0;
}
```

#### **Combining with Loops (10 min):**

```c
#include <stdio.h>

int main() {
    int choice;
    
    while(1) {
        printf("\n===== Menu =====\n");
        printf("1. Play\n");
        printf("2. Settings\n");
        printf("3. Quit\n");
        printf("Enter choice: ");
        scanf("%d", &choice);
        
        switch(choice) {
            case 1:
                printf("Starting game...\n");
                break;
            case 2:
                printf("Adjusting settings...\n");
                break;
            case 3:
                printf("Thanks for playing!\n");
                return 0;  // Exit program
            default:
                printf("Invalid choice\n");
        }
    }
    
    return 0;
}
```

---

### **Day 8 Practice Questions:**

**Easy:**
1. Simple calculator with switch (add, subtract, multiply, divide)
2. Day of week converter (1-7 to Monday-Sunday)
3. Grade printer (A, B, C, D, F)

**Medium:**
4. Simple ATM menu:
   ```
   1. Withdraw
   2. Deposit
   3. Check Balance
   4. Exit
   ```

5. Menu for shape area calculator:
   ```
   1. Circle
   2. Rectangle
   3. Triangle
   4. Exit
   ```

**Challenge:**
6. Build a menu-driven quiz application
7. Create a game menu with options to play, view rules, settings, quit

### **Day 8 Task (Assignment):**
Create a menu-driven program that:
1. Shows menu:
   ```
   1. Check even/odd
   2. Check positive/negative
   3. Check prime
   4. Exit
   ```
2. For choice 1-3, take a number and perform operation
3. Repeat menu until user selects exit
4. Example:
   ```
   ===== Menu =====
   1. Check even/odd
   2. Check positive/negative
   3. Check prime
   4. Exit
   Enter choice: 1
   Enter number: 10
   10 is even
   
   (menu repeats...)
   ```

---

## **Day 9: Putting It All Together - Mini Project**

**Time: 75 minutes**  
**Objective:** Combine all concepts in a complete working program

### **Project: Student Grade Management System**

**Features:**
1. Add student records (name, marks in 3 subjects)
2. Display all students with grades
3. Calculate class average
4. Find topper (highest average)
5. Menu-driven interface
6. Loop until user exits

### **Complete Code:**

```c
#include <stdio.h>
#include <string.h>

struct Student {
    char name[50];
    int marks[3];
    float average;
    char grade;
};

void calculateGrade(struct Student *student) {
    int sum = 0;
    for (int i = 0; i < 3; i++) {
        sum = sum + student->marks[i];
    }
    student->average = sum / 3.0;
    
    if (student->average >= 90) student->grade = 'A';
    else if (student->average >= 75) student->grade = 'B';
    else if (student->average >= 50) student->grade = 'C';
    else student->grade = 'F';
}

int main() {
    struct Student students[100];
    int totalStudents = 0;
    int choice;
    
    while (1) {
        printf("\n========================================\n");
        printf("  Student Grade Management System\n");
        printf("========================================\n");
        printf("1. Add Student\n");
        printf("2. Display All Students\n");
        printf("3. Calculate Class Average\n");
        printf("4. Find Topper\n");
        printf("5. Exit\n");
        printf("========================================\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);
        
        switch(choice) {
            case 1: {
                if (totalStudents >= 100) {
                    printf("Maximum students reached!\n");
                    break;
                }
                printf("\n--- Add New Student ---\n");
                printf("Enter student name: ");
                scanf("%s", students[totalStudents].name);
                
                printf("Enter marks in Math: ");
                scanf("%d", &students[totalStudents].marks[0]);
                printf("Enter marks in Science: ");
                scanf("%d", &students[totalStudents].marks[1]);
                printf("Enter marks in English: ");
                scanf("%d", &students[totalStudents].marks[2]);
                
                calculateGrade(&students[totalStudents]);
                totalStudents++;
                printf("Student added successfully!\n");
                break;
            }
            
            case 2: {
                if (totalStudents == 0) {
                    printf("No students added yet!\n");
                    break;
                }
                printf("\n========== All Students ==========\n");
                printf("%-20s %-10s %-10s\n", "Name", "Average", "Grade");
                printf("==================================\n");
                for (int i = 0; i < totalStudents; i++) {
                    printf("%-20s %-10.2f %-10c\n",
                           students[i].name,
                           students[i].average,
                           students[i].grade);
                }
                printf("==================================\n");
                break;
            }
            
            case 3: {
                if (totalStudents == 0) {
                    printf("No students added yet!\n");
                    break;
                }
                float totalAverage = 0;
                for (int i = 0; i < totalStudents; i++) {
                    totalAverage = totalAverage + students[i].average;
                }
                float classAverage = totalAverage / totalStudents;
                printf("\nClass Average: %.2f\n", classAverage);
                break;
            }
            
            case 4: {
                if (totalStudents == 0) {
                    printf("No students added yet!\n");
                    break;
                }
                int topperIndex = 0;
                for (int i = 1; i < totalStudents; i++) {
                    if (students[i].average > students[topperIndex].average) {
                        topperIndex = i;
                    }
                }
                printf("\n========== Topper ==========\n");
                printf("Name: %s\n", students[topperIndex].name);
                printf("Average: %.2f\n", students[topperIndex].average);
                printf("Grade: %c\n", students[topperIndex].grade);
                printf("============================\n");
                break;
            }
            
            case 5:
                printf("\nThank you for using Student Management System!\n");
                printf("Exiting...\n");
                return 0;
            
            default:
                printf("Invalid choice! Please try again.\n");
        }
    }
    
    return 0;
}
```

### **What Student Learns:**

✅ Structures (grouping related data)  
✅ Functions with parameters and pointers  
✅ Arrays of structures  
✅ Loops within loops  
✅ Menu-driven interface design  
✅ Real problem-solving approach  
✅ **Programming mindset: "I can build real applications!"**

### **Day 9 Practice Questions:**

**Enhancements to the project:**

1. **Search functionality:** Find student by name
2. **Sort functionality:** Display students sorted by average (highest to lowest)
3. **Delete functionality:** Remove a student by name
4. **Update functionality:** Edit student marks
5. **Statistics:** Show pass/fail count, highest marks, lowest marks
6. **Save/Load:** Save student data to file, load on program start

### **Day 9 Task (Assignment):**

**Extension Challenge:**
Add these features to Student Management System:

1. Search function to find student by name and display their details
2. Display students sorted by average (highest first)
3. Count and display number of students with each grade (A, B, C, F)

Example output:
```
Grade Distribution:
Grade A: 5 students
Grade B: 3 students
Grade C: 2 students
Grade F: 0 students
```

---

## **Day 10: Recap, Pointers Introduction & Final Project**

**Time: 75 minutes**  
**Objective:** Review all concepts, introduce pointers, celebrate completion

### **Content Breakdown (75 min):**

#### **Quick Recap (15 min):**

| Topic | What You Learned | Used For |
|-------|-----------------|----------|
| **Variables & Data Types** | Store different kinds of data | Storing numbers, text, single characters |
| **Input/Output** | Take input, print output | Communicate with user |
| **Conditionals** | Make decisions (if-else, switch) | Choose different code paths |
| **Loops** | Repeat code (for, while) | Process multiple items |
| **Functions** | Reusable code blocks | Organize code, prevent repetition |
| **Arrays** | Store multiple values | Handle collections of data |
| **Strings** | Work with text | Process text data |
| **Structures** | Group related data | Create complex data types |

#### **Pointers - Introduction (20 min):**

**Memory Address:**
```c
#include <stdio.h>

int main() {
    int age = 25;
    
    printf("Value: %d\n", age);      // 25
    printf("Address: %p\n", &age);   // 0x7fff5fbff8ac (example)
    
    return 0;
}
```

**Pointer Basics:**
```c
#include <stdio.h>

int main() {
    int age = 25;
    int *ptr;  // Declare pointer to int
    
    ptr = &age;  // ptr holds address of age
    
    printf("Value of age: %d\n", age);        // 25
    printf("Address of age: %p\n", &age);     // 0x7fff...
    printf("Value in ptr: %p\n", ptr);        // 0x7fff...
    printf("Value pointed to by ptr: %d\n", *ptr);  // 25
    
    return 0;
}
```

**Key Symbols:**
- `&` = Address-of operator (get address)
- `*` = Dereference operator (get value at address)

**Why Pointers Matter:**
- ✅ Used in arrays and strings
- ✅ Pass variables by reference to functions
- ✅ Create dynamic memory
- ✅ Build complex data structures
- **Don't worry about full details yet!** You'll master this later.

#### **Pointers in Functions (15 min):**

```c
#include <stdio.h>

// Function that modifies original variable
void increment(int *num) {
    *num = *num + 1;  // Dereference and modify
}

int main() {
    int value = 10;
    
    printf("Before: %d\n", value);  // 10
    increment(&value);  // Pass address
    printf("After: %d\n", value);   // 11
    
    return 0;
}
```

#### **Final Project - Quiz Game (25 min):**

### **Project: Interactive Quiz Game**

```c
#include <stdio.h>
#include <string.h>

int main() {
    // Quiz questions and options
    char questions[5][100] = {
        "What is the capital of India?",
        "What is 2 + 2?",
        "Who wrote Harry Potter?",
        "What is the largest planet in our solar system?",
        "In what year did World War II end?"
    };
    
    char options[5][4][50] = {
        {"A) Delhi", "B) Mumbai", "C) Bangalore", "D) Kolkata"},
        {"A) 3", "B) 4", "C) 5", "D) 6"},
        {"A) JK Rowling", "B) George RR Martin", "C) Stephen King", "D) Tolkien"},
        {"A) Mars", "B) Jupiter", "C) Saturn", "D) Venus"},
        {"A) 1943", "B) 1944", "C) 1945", "D) 1946"}
    };
    
    int answers[5] = {0, 1, 0, 1, 2};  // Index of correct answers (A=0, B=1, C=2, D=3)
    
    int score = 0;
    char userAnswer;
    
    printf("\n");
    printf("========================================\n");
    printf("    Welcome to C Programming Quiz!\n");
    printf("========================================\n");
    printf("You will answer 5 questions.\n");
    printf("Choose your answer: A, B, C, or D\n");
    printf("Good luck!\n");
    printf("========================================\n\n");
    
    // Loop through all questions
    for (int i = 0; i < 5; i++) {
        printf("Question %d: %s\n", i + 1, questions[i]);
        
        // Print all options
        for (int j = 0; j < 4; j++) {
            printf("%s\n", options[i][j]);
        }
        
        printf("Your answer (A/B/C/D): ");
        scanf(" %c", &userAnswer);
        
        // Convert answer to index (A->0, B->1, C->2, D->3)
        int userChoice = userAnswer - 'A';
        
        // Check answer
        if (userChoice >= 0 && userChoice <= 3) {
            if (userChoice == answers[i]) {
                printf("✓ Correct!\n");
                score++;
            } else {
                printf("✗ Wrong! Correct answer: %c\n", 'A' + answers[i]);
            }
        } else {
            printf("Invalid input!\n");
        }
        
        printf("\n");
    }
    
    // Calculate percentage
    float percentage = (score / 5.0) * 100;
    
    printf("========================================\n");
    printf("         Quiz Complete!\n");
    printf("========================================\n");
    printf("Your Score: %d / 5\n", score);
    printf("Percentage: %.1f%%\n", percentage);
    printf("========================================\n\n");
    
    // Feedback based on score
    if (score >= 5) {
        printf("🌟 Excellent! Perfect score!\n");
        printf("You're absolutely ready for Java!\n");
    } else if (score >= 4) {
        printf("🎉 Great! You understand concepts well!\n");
        printf("You're ready for Java full-stack development!\n");
    } else if (score >= 3) {
        printf("👍 Good effort! Keep practicing!\n");
        printf("Review concepts and practice more before Java.\n");
    } else if (score >= 2) {
        printf("📚 You need more practice!\n");
        printf("Review the fundamentals again.\n");
    } else {
        printf("⚠️  Revisit all concepts and practice daily!\n");
    }
    
    printf("\n========================================\n");
    printf("  Thank you for completing this bootcamp!\n");
    printf("========================================\n\n");
    
    return 0;
}
```

### **What This Project Teaches:**

✅ 2D arrays (questions, options)  
✅ Loops within loops  
✅ Character arithmetic (A→0)  
✅ Conditional logic (validate input)  
✅ Score calculation  
✅ User feedback based on performance  
✅ Complete standalone application

### **Day 10 Practice Questions:**

**Enhancements to Quiz Game:**

1. **Difficulty Levels:** Add easy, medium, hard questions
2. **Timer:** Add time limit per question
3. **Leaderboard:** Track highest scores
4. **Category-based:** Quiz on different topics
5. **Randomize:** Shuffle questions randomly

### **Day 10 Task (Assignment):**

**Final Challenge:**

1. Run the Quiz game successfully
2. Play through all 5 questions
3. Get your final score
4. **Extension:** Add these features:
   - Add 5 more questions (C programming specific)
   - Display time per question
   - Show which questions were wrong

---

## **By Day 11 - Programming Mindset Achieved ✅**

### **What They Now Understand:**

**Problem-Solving Mindset:**
1. **Break Complex Problems:** Divide into smaller functions
2. **Store Data Wisely:** Use appropriate data types and structures
3. **Automate Repetition:** Use loops instead of rewriting
4. **Make Decisions:** Use conditionals for logic
5. **Reuse Code:** Functions prevent duplication
6. **Debug Systematically:** Test each part independently
7. **Think in abstractions:** Structures, functions, modules

**Key Insights:**
- ✅ Programming is **logical thinking**, not magic
- ✅ **Practice > Theory** - Real programs beat tutorials
- ✅ **Errors are learning opportunities** - Debugging teaches most
- ✅ **Small steps lead to big projects** - Compound learning
- ✅ **C teaches fundamentals** - Everything else builds on this

### **Ready for Next Steps:**

- ✅ Can understand object-oriented concepts (Java)
- ✅ Can work with frameworks (Spring Boot)
- ✅ Can build complete applications
- ✅ Can learn any programming language faster
- ✅ **Employment-ready mindset developed!**
- ✅ Confident to tackle Java, microservices, full-stack development

---

## **Teaching Tips for Trainer:**

### **For Non-IT Background Students:**

1. **Use Analogies:**
   - "Function = Recipe" (write once, use many times)
   - "Array = Row of boxes" (each box holds a value)
   - "Loop = Washing machine cycle" (repeat action)
   - "Pointer = Address to a house" (get/use address)

2. **Hands-On First:**
   - Theory → Practice → Complex Problems
   - Show working code first
   - Explain mechanics second

3. **Celebrate Small Wins:**
   - "You compiled your first program! That's huge!"
   - "Your calculator works! You're a programmer!"
   - Create momentum and confidence

4. **Relate to Real World:**
   - Variables = bank accounts
   - Loops = daily routines
   - Functions = appliances/tools
   - Arrays = phone contacts list

5. **Don't Rush:**
   - 75 minutes is optimal for one topic
   - Mastery > Speed
   - Better to go deep in one concept than shallow in many

6. **Practice Problems First:**
   - Show working program
   - Explain mechanics
   - Let them modify

7. **Encourage Experimentation:**
   - "What if you change this number? Try it!"
   - "Break it intentionally and fix it"
   - Learning through mistakes

8. **Group Learning:**
   - Pair programming (2 students, 1 computer)
   - Builds confidence
   - Collaborative problem-solving

9. **Show Error Messages:**
   - "This error means... Let's fix it together"
   - Error messages are **not** scary
   - They're instructions on what to fix

10. **End Each Day with Real Code:**
    - Students should have working code, not just notes
    - Runnable programs for portfolio
    - They can show it to others

---

## **Success Metrics - By Day 11:**

| Metric | Status |
|--------|--------|
| Write basic C programs independently | ✅ |
| Understand loops, functions, arrays | ✅ |
| Debug simple errors | ✅ |
| Combine multiple concepts in one program | ✅ |
| Think like a programmer systematically | ✅ |
| Confidence to learn Java | ✅ |
| Ready for portfolio projects | ✅ |
| Build a complete working application | ✅ |
| Problem-solving mindset developed | ✅ |
| Foundations for industry-ready skills | ✅ |

---

## **Next Steps After Day 10:**

### **Transition to Java:**

1. **OOP Concepts:** Classes, objects, inheritance (transfers from C structures)
2. **Spring Framework:** Build REST APIs
3. **Database:** SQL, JDBC, Hibernate
4. **Frontend:** React or Angular
5. **Microservices:** Spring Boot microservices
6. **Deployment:** Docker, Kubernetes, Cloud platforms

### **Recommended Timeline:**

- **Week 1-2:** Java basics (4-6 hours)
- **Week 3-4:** OOP in Java (4-6 hours)
- **Week 5-6:** Spring Boot (6-8 hours)
- **Week 7-8:** Database & REST APIs (6-8 hours)
- **Week 9-10:** Full-stack with React/Angular (8-10 hours)
- **Week 11-12:** Microservices architecture (8-10 hours)
- **Week 13+:** Deploy to cloud and build portfolio (ongoing)

**Total:** 6 months to industry-ready full-stack developer

---

## **Final Notes:**

This 10-day curriculum is designed to **transform non-IT students into programmers** with:

✅ **Foundational Understanding:** Variables, loops, functions, arrays, strings  
✅ **Problem-Solving Skills:** Break problems, think logically, code systematically  
✅ **Real Code Experience:** Working programs, not just theory  
✅ **Confidence Boost:** "I can build applications!"  
✅ **Ready for Advanced Learning:** Java, frameworks, microservices

The key is **practice, practice, practice**. By Day 11, students won't just know programming concepts—they'll **think like programmers**.

Good luck! 🚀

