# DSA456-Notes
Comprehensive notes on data structures and algorithms

### Algorithms Analysis

#### What is Algorithms Analysis?

When you write a program (which is like giving instructions to a computer), you should think about how much time and space (memory) your program needs. These are two important resources:

1. **Time**: How long it takes for your program to finish running.
2. **Memory**: How much space it takes up in the computer's memory.

Sometimes, you might need to choose between using more time or more memory. It depends on what you need your program to do and what kind of computer you have. 

- **Example**: If you need your program to be very fast because it has to finish quickly, you might use more memory. If your computer doesn't have much memory, you might use more time but less memory.

#### Understanding Resource Needs

The resources (time and memory) your program uses often depend on how much data you have. If you have more data:

- You need more space to store it.
- It takes more time to process it.

#### Key Idea

When we talk about "Algorithms Analysis," we're not just asking "How much resource is used for a certain amount of data?" Instead, we're asking:

- **How does the resource usage change when we add a little more data?**

So, we're interested in how quickly the resource needs grow as the data gets bigger.

#### Example to Understand Growth Rate

Think of it like this: If you have one block, you need a small box to store it. If you get one more block, do you need a box that's just a little bit bigger, or do you need a much bigger box? This is what we mean by looking at the growth rate.

### Summary

- **Algorithms Analysis** helps us understand how much more time or memory we need as we get more data.
- We care about how quickly the needs grow, not just how much is used for a specific amount of data.

### Measuring Resource Consumption

#### Analysis of Algorithms

When we look at how much of something (like time or memory) a program uses as it works with more and more data, we call this "analysis of algorithms." Let's break this down:

1. **Resources**: Things that we have a limited amount of. The most common ones are:
   - **Time**: How long the program takes to run.
   - **Memory**: How much space the program uses.

#### Time Resource

Every little action your program does, like adding two numbers or saving a result, takes a bit of time. If you do more actions, it takes more time. One way to figure out how much time a program needs is to count how many actions (or operations) it performs.

- **Example**: If your program does 10 actions, it takes less time than if it does 100 actions.

We pretend that every action takes the same amount of time to keep things simple. In real life, some actions take longer than others, but for our analysis, we pretend they all take the same time.

#### Memory Resource

The other big resource is memory. Memory is like the space you need to store things. Unlike counting operations for time, memory usage depends on things like:
- How many variables you create.
- How much space those variables take up.

#### Measuring Resources

To figure out how much of a resource (time or memory) a program uses, we create a math expression. This expression shows how the resource usage changes as we use more data.

- **Example**: If you have 1 toy, you need a small box. If you have 100 toys, you need a much bigger box.

The expression helps us see how much more time or memory we need as we get more data. It's not just a single number; it's a formula that changes based on how much data we have.

### Summary

- **Time Resource**: We count how many actions the program does. More actions mean more time.
- **Memory Resource**: We look at how much space the variables and data take up. More data means more memory.

We use math expressions to understand how the needs for these resources grow as we get more data. This helps us know what to expect when our program works with more data.

### Growth Rates

When we talk about growth rates in algorithms, we're trying to understand how much more time or memory a program needs as we add more data. Let's look at different types of growth rates one by one, with simple examples.

#### Constant

Imagine you have a magic box. No matter how many toys you put inside—1 toy or 1 million toys—it always takes the same time to close the box. This is a **constant growth rate**.

- **Graph**: It's a straight, flat line because it never changes no matter how much data you add.

#### Logarithmic

Now, imagine you have a book with magical pages. Every time you double the number of pages, you only need a little more time to read it. This is a **logarithmic growth rate**.

- **Graph**: Starts steep but gets flatter and flatter. It never gets completely flat, but it gets close.

#### Linear

Think of a line of people where you shake each person’s hand. If you have 1 person, it takes a short time. If you have 10 people, it takes 10 times longer. This is a **linear growth rate**.

- **Graph**: A straight line going up evenly because the time increases directly with the number of people.

#### Loglinear

Imagine you have a special kind of party where for each new guest, you need to do a little more work than before, but not too much. This is a **loglinear growth rate**.

- **Graph**: It's a line that curves a little bit, getting less curved as you have more guests.

#### Quadratic

Imagine a birthday party where each new kid needs more and more balloons. If you have 1 kid, you need 1 balloon. For 2 kids, you need 4 balloons. For 3 kids, you need 9 balloons. This is a **quadratic growth rate**.

- **Graph**: Looks like a big U-shaped curve that gets steep quickly.

#### Cubic

Imagine the same birthday party, but now, if you have 1 kid, you need 1 toy. For 2 kids, you need 8 toys. For 3 kids, you need 27 toys. This is a **cubic growth rate**.

- **Graph**: Similar to quadratic but gets steep even faster.

#### Exponential

Imagine you have a magical plant that doubles in size every day. On the first day, it’s small. On the second day, it’s twice as big. By the fifth day, it's huge! This is an **exponential growth rate**.

- **Graph**: Starts flat but suddenly shoots up very steeply, almost like a wall.

### Summary

- **Constant**: Never changes, always the same.
- **Logarithmic**: Grows slowly, getting flatter.
- **Linear**: Grows evenly, like a straight line.
- **Loglinear**: Slightly curved line, gets less curved over time.
- **Quadratic**: Grows faster, like a steep U-shape.
- **Cubic**: Grows even faster than quadratic.
- **Exponential**: Grows very, very fast, like a rocket.

Each type of growth rate shows how the needs for resources (like time or memory) change as we add more data. Understanding these helps us pick the best algorithm for our needs.

### Asymptotic Notation

Asymptotic notation is a way to describe how much time or memory an algorithm needs as the amount of data grows. Let's break down each type of notation with simple, kid-friendly explanations.

### Big-O (O)

#### What it is:
- **Big-O (O)** tells us the upper limit of time or memory an algorithm will need as the data grows.

#### Example:
- Imagine you are cleaning your room. If it takes you no more than 1 hour to clean any mess, no matter how messy it gets, that's Big-O. The time it takes to clean is bounded by 1 hour.

### Little-o (o)

#### What it is:
- **Little-o (o)** tells us an upper limit that's not tight. It says the algorithm uses less than a certain amount of time or memory, but doesn't reach that amount.

#### Example:
- If cleaning your room always takes less than 1 hour, even if it sometimes takes much less, that's little-o. You know it won't take 1 hour, but you're not sure exactly how much less.

### Omega (Ω)

#### What it is:
- **Omega (Ω)** tells us the lower limit of time or memory an algorithm needs as the data grows.

#### Example:
- Imagine you have a favorite book you read before bed. You know it takes at least 10 minutes to read a chapter, no matter what. That's Omega. It never takes less than 10 minutes.

### Theta (Θ)

#### What it is:
- **Theta (Θ)** tells us the exact bound of time or memory an algorithm needs. It’s both the upper and lower limit.

#### Example:
- If every time you clean your room, it always takes exactly 30 minutes, that's Theta. The time is consistently 30 minutes, not more and not less.

### Putting it Together with Examples

- **O(f(n))**: If your chore (like cleaning) takes no more than \( f(n) \) minutes, no matter how messy your room is, that’s Big-O.
- **Ω(f(n))**: If your chore takes at least \( f(n) \) minutes, no matter what, that’s Omega.
- **Θ(f(n))**: If your chore always takes exactly \( f(n) \) minutes, that’s Theta.
- **o(f(n))**: If your chore takes less than \( f(n) \) minutes, but you don't know exactly how much less, that’s little-o.

### Worst Case, Best Case, Average Case

- **Worst Case**: How much time it takes at most, like cleaning the messiest room ever.
- **Best Case**: How much time it takes at least, like cleaning a nearly clean room.
- **Average Case**: How much time it takes on average, like cleaning a normally messy room.

### Rating System for Algorithms

Imagine movie ratings (like G, PG, etc.). They tell you what to expect without watching the movie. Asymptotic notation does the same for algorithms. It tells you what to expect in terms of resource usage (time or memory) as your data grows. From the least to the most resource usage, the ratings are:

- **O(1)**: Constant time, like a magic box that closes instantly, no matter how many toys.
- **O(log n)**: Logarithmic time, like a book that takes a bit more time as it gets thicker.
- **O(n)**: Linear time, like shaking hands with each person in a line.
- **O(n log n)**: Loglinear time, like sorting toys where the effort grows slightly faster than just adding more toys.
- **O(n^2)**: Quadratic time, like needing more and more balloons for each kid at a party.
- **O(n^3)**: Cubic time, like needing even more toys for each extra kid at a party.
- **O(2^n)**: Exponential time, like a magical plant that doubles in size every day.

### A Closer Look at Big-O

#### Formal Definition

- **T(n) is O(f(n))** if for some constants \( c \) and \( n_0 \), \( T(n) \leq cf(n) \) for all \( n \geq n_0 \).

#### Breaking It Down

1. **Constants \( c \) and \( n_0 \)**:
   - These are fixed numbers. They don’t change with the size of the data \( n \).
   - \( c \) is like a multiplier, and \( n_0 \) is a starting point where the rule starts to apply.

2. **T(n) \leq cf(n)**:
   - This means that our algorithm's resource use \( T(n) \) is less than or equal to a scaled version of \( f(n) \) after a certain point \( n_0 \).

3. **For all \( n \geq n_0 \)**:
   - This rule starts applying after a certain amount of data \( n_0 \), and continues for all larger amounts of data.

### Summary

- Asymptotic notation helps us understand how algorithms will behave as data grows, without needing to look at every detail of the code.
- It gives us a "rating" for resource usage, helping us predict performance and choose the best algorithm for our needs.

### What is Linear Search?
Imagine you have a box of toys, and you want to find your favorite toy. You start looking at the first toy, then the second toy, and so on, until you find your favorite one. This is exactly how linear search works. You look at each item in a list one by one until you find what you are looking for or reach the end of the list.

### The Linear Search Function
Here's a simple version of the linear search written in Python:

```python
def linear_search(my_list, key):
    for i in range(0, len(my_list)):
        if my_list[i] == key:
            return i
    return -1
```

- **my_list**: This is your box of toys (the list of items).
- **key**: This is your favorite toy that you're trying to find.
- **for i in range(0, len(my_list))**: This loop goes through each toy in the box.
- **if my_list[i] == key**: This checks if the current toy is your favorite toy.
- **return i**: If it finds the toy, it tells you the position (index) of the toy.
- **return -1**: If it doesn't find the toy after checking all toys, it tells you that the toy isn't there by returning -1.

### Analyzing How Long It Takes
When we talk about how long it takes to find your toy, we're looking at two things:
1. **Best Case**: This is the quickest way to find your toy. Maybe it's the first toy you look at.
2. **Worst Case**: This is the longest it could take. Maybe your toy is the last one you look at or it's not there at all.

#### Unsuccessful Search
Let's start by thinking about the worst case where your toy is not in the box.

- You look at each toy one by one until you reach the end of the box.
- For each toy, you do one check to see if it’s your favorite toy.

If there are `n` toys in the box, you do this check `n` times.

Here's the step-by-step counting of the work done by the function:
- The loop runs `n` times.
- Inside the loop, it does one check each time (`my_list[i] == key`).

So, we can say the total work done (number of operations) is:
\[ T(n) = n \]
where `T(n)` is the number of operations needed for a list of size `n`.

#### Successful Search
Now, let's think about the best case where you find your toy right away:
- If the toy is the first one, the loop runs only once and finds it immediately.

But on average, if the toy could be anywhere:
- You might find it after looking at about half of the toys in the box.

So, on average, it would look at `n/2` toys:
\[ T(n) = n/2 \]

### Simplifying for Big-O Notation
When we talk about Big-O notation, we care about what happens as the number of toys (`n`) gets very large. We simplify by focusing on the biggest term and ignoring smaller constants.

For our linear search:
- In the worst case, we said:
\[ T(n) = n \]
- Even if we added small constants (like counting other tiny operations), as `n` gets very large, those don't matter much.

So, in Big-O notation, we say:
\[ T(n) = O(n) \]
This means that the time it takes to do the search grows linearly with the number of toys.

### Why We Use Big-O
Big-O notation helps us understand and compare how efficient different algorithms are without worrying about the exact time they take. It’s like saying how many steps are on a staircase without needing to know the height of each step.

### Recap
1. **Linear Search**: Look at each toy one by one until you find your toy or reach the end.
2. **Worst Case**: Look through all the toys (n times).
3. **Best Case**: Find your toy immediately (1 time).
4. **Average Case**: Look through about half the toys (n/2 times).
5. **Big-O Notation**: Helps us describe the efficiency of the search. For linear search, it’s `O(n)`, meaning the time grows linearly with the number of items.

So, just like finding your toy in a box, linear search takes more time the more toys you have, and that’s why it’s `O(n)`.


### What is Binary Search?
Imagine you have a big book of words, and it's sorted alphabetically. You want to find a specific word in the book. Instead of starting from the first page and looking at each word one by one, you can be smarter. You can open the book in the middle, see if your word is before or after the middle, and then repeat the process with the half of the book that might contain your word. This is how binary search works.

### The Binary Search Function
Here's a simple version of binary search written in Python:

```python
def binary_search(my_list, key):
    rc = -1
    low = 0
    high = len(my_list) - 1

    while rc == -1 and low <= high:
        mid = (low + high) // 2
        if key < my_list[mid]:
            high = mid - 1
        elif key > my_list[mid]:
            low = mid + 1
        else:
            rc = mid

    return rc
```

- **my_list**: This is your sorted book of words (the list of items).
- **key**: This is the word you're trying to find.
- **low**: This is the start of the section you're searching.
- **high**: This is the end of the section you're searching.
- **mid**: This is the middle of the section you're searching.

The binary search starts by checking the middle word. If your word is before the middle word, it looks in the first half; if it's after, it looks in the second half. It keeps doing this until it finds the word or runs out of places to look.

### Analyzing How Long It Takes
When we talk about how long it takes to find your word, we're looking at the worst case, which is not finding the word at all.

#### Unsuccessful Search
Let's think about the worst case where your word is not in the book.

1. **Initial Setup**
   - **rc = -1**: Setting up a return code, just 1 operation.
   - **low = 0**: Starting index, 1 operation.
   - **high = len(my_list) - 1**: Ending index, 3 operations (1 function call to get the length, 1 subtraction, and 1 assignment).

2. **While Loop**
   - The loop keeps running until `low` is greater than `high`.

Each time the loop runs, it does a few things:
   - **Checking Conditions**: `rc == -1 and low <= high` is checked, which takes 3 operations each time.
   - **Finding the Middle**: `mid = (low + high) // 2` takes 3 operations each time.
   - **Comparisons and Updates**: It checks if `key` is less than, greater than, or equal to the middle element. The most operations happen when it checks both less than and greater than:
     - `if key < my_list[mid]`: 1 operation.
     - `elif key > my_list[mid]`: 1 operation.
     - `low = mid + 1`: 2 operations if the key is greater.

So, each iteration of the loop involves about 10 operations.

### Number of Loop Iterations
The key part of binary search is that it eliminates half of the remaining elements each time. 

- **First Iteration**: `n` elements.
- **Second Iteration**: `n/2` elements.
- **Third Iteration**: `n/4` elements.
- **Fourth Iteration**: `n/8` elements.
- And so on...

This continues until we're down to 1 element. If we write this as a pattern, it looks like:

- 1st iteration: \( n / 2^0 \)
- 2nd iteration: \( n / 2^1 \)
- 3rd iteration: \( n / 2^2 \)
- \( k \)-th iteration: \( n / 2^{k-1} \)

When we get down to just 1 element, we can say:

\[ \frac{n}{2^k} = 1 \]

By solving for \( k \), we get:

\[ k = \log_2{n} \]

So, the loop runs about \( \log_2{n} \) times.

### Putting It All Together
Now let's add up the operations:

1. **Initial Setup**: 1 + 1 + 3 = 5 operations.
2. **Loop Operations**: Each iteration is about 10 operations.

Since the loop runs \( \log_2{n} \) times, the total operations for the loop are:

\[ 10 \cdot \log_2{n} \]

Adding the initial setup:

\[ T(n) = 10 \cdot \log_2{n} + 5 \]

### Simplifying for Big-O Notation
When we use Big-O notation, we focus on the largest term as the number of items (`n`) gets very large. Small constants become less important.

For binary search:
\[ T(n) = 10 \cdot \log_2{n} + 5 \]

As `n` gets very large, the 5 becomes insignificant compared to the \( 10 \cdot \log_2{n} \).

So, in Big-O notation, we say:
\[ T(n) = O(\log n) \]

### Recap
1. **Binary Search**: Start in the middle, eliminate half the elements each time.
2. **Worst Case**: Not finding the word, checking about \( \log_2{n} \) times.
3. **Big-O Notation**: Focuses on the largest term, which is \( \log n \).

Binary search is much faster than linear search, especially for large lists, because it cuts the number of items to check in half each time, making it \( O(\log n) \).

let's break down **the steps for analyzing code performance** in a way that's easy to understand.

### Step 0: Show Your Code

First, you put your code so everyone can see it. It's like showing your homework before you start explaining it.

```python
def factorial(number):
    rc = 1
    for i in range(2, number + 1):
        rc = rc * i
    return rc
```

This code calculates the factorial of a number. A factorial is when you multiply a number by all the numbers below it. For example, factorial of 5 (written as 5!) is 5 * 4 * 3 * 2 * 1.

### Step 1: Explain What Variables and Functions Mean

Next, we explain what the variables and functions mean in the code. Think of it as labeling the parts of a puzzle before putting it together.

- Let **n** be the number we're finding the factorial for.
- Let **T(n)** be the number of steps (operations) our code takes to find the factorial of n.

### Step 2: Count the Steps (Operations)

Now, we count every little step the code takes to do its job. Imagine counting the number of moves you make to solve a puzzle.

1. **Setting up `rc`**: 
   ```python
   rc = 1  # 1 operation
   ```

2. **Setting up the loop**: 
   ```python
   for i in range(2, number + 1):  # (n-1) iterations + 1 for the + operator + 1 for range call
   ```

3. **Multiplying inside the loop**:
   ```python
   rc = rc * i  # 2 operations (multiplication and assignment), (n-1) times
   ```

4. **Returning the result**:
   ```python
   return rc  # 1 operation
   ```

So, let's write this with the counts:

```python
def factorial(number):
    rc = 1  # 1 operation

    for i in range(2, number + 1):  # (n-1) + 1 + 1 = (n-1) + 2
        rc = rc * i  # 2 * (n-1)
    
    return rc  # 1 operation
```

### Step 3: Add Up the Steps

Now, we add up all the steps we counted:

- **Setting up `rc`**: 1 step.
- **Loop setup**: (n-1) + 2 steps.
- **Inside the loop**: 2 * (n-1) steps.
- **Returning the result**: 1 step.

So, the total steps are:

\[ T(n) = 1 + ((n-1) + 2) + (2 \cdot (n-1)) + 1 \]

### Step 4: Simplify the Steps

We simplify the total steps by adding and combining like terms. It’s like tidying up your puzzle pieces.

\[ T(n) = 1 + (n-1) + 2 + 2(n-1) + 1 \]

\[ T(n) = 1 + n - 1 + 2 + 2n - 2 + 1 \]

Combine the terms:

\[ T(n) = 3n + 1 \]

### Step 5: Find the Dominating Term

Finally, we look for the biggest term because as the puzzle (or number n) gets bigger, the smaller pieces don’t matter much.

In \( T(n) = 3n + 1 \), as n becomes very large, the "+1" part doesn’t matter much compared to "3n".

So, we say \( T(n) \) is \( O(n) \).

### Summary

1. **Show the Code**: Display the code you’re analyzing.
2. **Explain Variables**: Define the variables and functions.
3. **Count Steps**: Count the operations in the code.
4. **Add Up Steps**: Combine all the counts into one expression.
5. **Find Dominating Term**: Simplify to find the term that matters most as n gets very large.

This tells us how the code will perform as the size of the input (n) increases. For the factorial function, the steps grow linearly with n, which is called \( O(n) \) in Big-O notation.

When analyzing loop iterations in terms of time complexity, the terms \( n \), \( n+1 \), and \( n-1 \) refer to different scenarios depending on the specific behavior of the loop and the starting/ending conditions. Here’s a detailed explanation:

### Loop Iterations

1. **\( n \) Iterations:**
   - This is the straightforward case where the loop runs exactly \( n \) times.
   - **Example:**
     ```python
     for i in range(n):
         # loop body
     ```
   - **Explanation:** The loop starts at 0 and ends at \( n-1 \), making a total of \( n \) iterations.

2. **\( n+1 \) Iterations:**
   - This occurs when the loop runs one extra iteration, often due to the inclusive nature of the loop’s end condition.
   - **Example:**
     ```python
     for i in range(n+1):
         # loop body
     ```
   - **Explanation:** The loop starts at 0 and ends at \( n \), making a total of \( n+1 \) iterations.

3. **\( n-1 \) Iterations:**
   - This occurs when the loop runs one fewer iteration, often due to the exclusive nature of the loop’s start or end condition.
   - **Example:**
     ```python
     for i in range(1, n):
         # loop body
     ```
   - **Explanation:** The loop starts at 1 and ends at \( n-1 \), making a total of \( n-1 \) iterations.

### Use Cases

- **Using \( n \) Iterations:**
  - When the loop condition is straightforward, such as `for i in range(n)`, and you want the loop to execute exactly \( n \) times.
  - **Example:**
    ```python
    for i in range(10):  # Runs 10 times
        print(i)
    ```

- **Using \( n+1 \) Iterations:**
  - When you need the loop to run one extra iteration beyond \( n \).
  - This could be for inclusive ranges or when a boundary condition requires one extra step.
  - **Example:**
    ```python
    for i in range(n+1):  # Runs 11 times if n is 10
        print(i)
    ```
  - **Real-world scenario:**
    - Checking conditions up to and including the \( n \)-th element.

- **Using \( n-1 \) Iterations:**
  - When the loop needs to start from 1 instead of 0, or when it should run up to \( n-1 \) elements.
  - **Example:**
    ```python
    for i in range(1, n):  # Runs 9 times if n is 10
        print(i)
    ```
  - **Real-world scenario:**
    - When calculating differences between consecutive elements, you often iterate from the second element to the last.

### Examples in Context

1. **\( n \) Iterations:**
   - **Function:**
     ```python
     def print_numbers(n):
         for i in range(n):
             print(i)
     ```
   - **Explanation:** Prints numbers from 0 to \( n-1 \).

2. **\( n+1 \) Iterations:**
   - **Function:**
     ```python
     def print_numbers_inclusive(n):
         for i in range(n+1):
             print(i)
     ```
   - **Explanation:** Prints numbers from 0 to \( n \), including \( n \).

3. **\( n-1 \) Iterations:**
   - **Function:**
     ```python
     def print_numbers_exclusive(n):
         for i in range(1, n):
             print(i)
     ```
   - **Explanation:** Prints numbers from 1 to \( n-1 \), excluding 0.

### Summary

- **\( n \):** Use when you want the loop to run exactly \( n \) times.
- **\( n+1 \):** Use when you need one extra iteration, often for inclusive conditions.
- **\( n-1 \):** Use when you start from 1 or need one fewer iteration, often for exclusive conditions. 

Understanding when to use \( n \), \( n+1 \), or \( n-1 \) helps in accurately counting loop iterations and analyzing the time complexity of algorithms.

### Introduction to Recursion

**What is Recursion?**

Recursion is like when you ask yourself the same question over and over again until you find an answer. In programming, recursion is when a function calls itself to solve a problem.

**Why is Recursion Important?**

Sometimes, problems are easier to solve if you can break them down into smaller parts. Recursion helps to do that. Some algorithms (ways to solve problems) are easier to write and understand using recursion.

**Why Should You Learn Recursion?**

- Some problems are best solved with recursion.
- Textbooks and resources often show recursive solutions.
- Understanding recursion helps you understand these solutions better.

### The Run-time Stack

**What is the Run-time Stack?**

Imagine a stack of plates. The run-time stack works in a similar way for your programs. It's where your program keeps track of what it's doing and what variables it’s using.

**How Does It Work?**

1. **Function Calls**: When a function (a piece of code that does a specific job) is called, it’s like adding a new plate to the stack.
2. **Local Variables**: Each function has its own variables (like plates with food on them). These variables only exist on the current plate.
3. **Function Ends**: When a function finishes, the plate is removed from the stack, and you go back to the previous plate.

**Why is the Run-time Stack Important for Recursion?**

When a function calls itself (recursion), it adds a new plate to the stack each time. This helps keep track of where you are in solving the problem. When each "plate" (function call) finishes, it’s removed from the stack until you get back to the first plate (the original function call).

### Example

Let's say you have a problem like this: 

**How to Find a Factorial (like 5!) Using Recursion**

1. **What is Factorial?**: The factorial of 5 (written as 5!) is 5 * 4 * 3 * 2 * 1.
2. **Using Recursion**: You can solve this by multiplying 5 by the factorial of 4 (which is 4 * 3 * 2 * 1), and so on.

Here's a simple function to find the factorial:

```python
def factorial(n):
    if n == 1:  # Base case
        return 1
    else:
        return n * factorial(n - 1)  # Recursive call
```

**How Does It Work?**

1. `factorial(5)` calls `factorial(4)`, which calls `factorial(3)`, and so on, adding plates to the stack.
2. When it reaches `factorial(1)`, it knows the answer is 1 (this is the base case, like finding the bottom plate).
3. It then multiplies back up the stack: 1 * 2, then 2 * 3, then 6 * 4, and finally 24 * 5 to get 120.

Each function call adds a "plate" to the stack until it reaches the base case, then it removes each plate one by one, multiplying the values as it goes back up.

**Lists**

### What is a List?
Imagine you have a row of toy boxes, and each toy box has a number on it, like Box 1, Box 2, Box 3, and so on. Each box can hold one toy. This row of boxes with numbers is what we call a list.

### Properties of a List
- **Ordered**: The boxes have a specific order. There is a "first" box, a "second" box, and so on.
- **Sorted or Unsorted**: The toys inside the boxes can be arranged in a specific way (like all the cars together, all the dolls together) which is sorted, or they can just be put in randomly, which is unsorted.
- **Duplicates or Unique**: You can have more than one of the same toy (duplicates), or you can have all different toys (unique).

### List Operations
These are some things you can do with your row of toy boxes:

1. **Initialize**: This means getting your row of empty toy boxes ready to start putting toys in.
2. **Add an Item**: Put a new toy in one of the boxes.
3. **Remove an Item**: Take a toy out of a box.
4. **Search**: Look through the boxes to find a specific toy.
5. **Sort**: Arrange the toys in a specific order (like all the cars together, all the dolls together).
6. **Iterate Through All Items**: Go through each box one by one to see what toy is inside.

### Different Ways to Make a List
There are two main ways to set up your row of toy boxes:

1. **Array Method**: This is like having a long bench with fixed spaces for each box. Each space always has a box, and you can't move the spaces around. If you want to add a new box, you have to put it at the end or move everything to make space.

2. **Linked List Method**: This is like having a line of friends holding hands. Each friend (box) can hold a toy and also point to the next friend in line. If you want to add a new friend in the middle, you just break the chain and link hands with the new friend.

### Summary
A list is just a fancy name for a row of toy boxes where each box has an important place in line. You can do lots of things with this row of boxes, like adding new toys, taking toys out, or finding a specific toy. And there are two main ways to set up your boxes: all in fixed spaces or like friends holding hands.

### What is a Linked List?
A linked list is like a chain of friends holding hands. Each friend has a toy, and they hold hands to show the next friend in line. This makes a long chain where each friend can point to the next friend.

### Parts of a Linked List
- **Node**: This is each friend in the chain. Each node (friend) has two things:
  1. A toy (data object).
  2. A pointer (hand) to the next friend (node) in the line.

- **Pointer to First Node**: The linked list itself keeps track of the first friend in the chain. By following the pointers (hands) from the first friend, you can visit all the other friends.

### Example of Linked List
Imagine you want to store 5 numbers. Here’s what it looks like in a linked list:

1. Friend 1 holds number 10 and points to Friend 2.
2. Friend 2 holds number 20 and points to Friend 3.
3. Friend 3 holds number 30 and points to Friend 4.
4. Friend 4 holds number 40 and points to Friend 5.
5. Friend 5 holds number 50 and points to nothing (end of the chain).

### How is it Different from an Array?
An array is like a long bench with numbered spots, and you can directly go to any spot on the bench. So, if you want the 5th spot, you just jump straight to it.

But in a linked list, you have to start from the first friend and follow the pointers (hands) one by one to reach the 5th friend. This means you have to walk through the line of friends to get to any specific one.

### Operations on a Linked List
Here are some things you can do with your chain of friends:

1. **push_front**: Add a new friend at the beginning of the line.
2. **push_back**: Add a new friend at the end of the line.
3. **pop_front**: Remove the first friend in the line.
4. **pop_back**: Remove the last friend in the line.
5. **insert**: Add a new friend at a specific place in the line.
6. **erase**: Remove a specific friend from the line.
7. **erase(a,b)**: Remove all friends between friend a and friend b.
8. **traversals**: Do something with each friend in the line, like checking their toys.

### Special Points
- It's really quick to find the first friend.
- To find any other friend, you have to start at the beginning and follow the pointers.
- This is unlike an array where you can quickly jump to any spot.

### Enhancements
Sometimes, to make things easier, we add more features to our linked list. We will learn about these when we talk about how to actually make a linked list.

### Summary
A linked list is like a line of friends holding hands, where each friend has a toy and points to the next friend. You can add or remove friends and follow the line to find a specific friend. It's different from an array because you have to follow the pointers to move through the line.

### List Implementation
Think of two ways to store your toys: in a long box (array) or with friends holding hands (linked list). Each way has its own set of cool tricks and challenges.

### Array-Based Implementation
Imagine you have a big toy box with numbered slots. Each slot can hold one toy.

#### Advantages:
1. **Easy Access**: You can quickly grab any toy from any slot. If you want the toy in slot 3, you just look at slot 3.
2. **Fast Searching**: If the toys are in order, you can quickly find any toy using a trick called binary search.

#### Drawbacks:
1. **Wasted Space**: Sometimes you have more slots than toys, so some slots stay empty.
2. **Hard to Add Toys in the Middle**: If you want to add a toy in the middle, you have to shift all the toys after it to make space.
3. **Hard to Remove Toys**: If you want to take out a toy from the middle, you have to shift all the toys after it to fill the gap.
4. **Growing Pains**: If your toy box gets full, you need to get a bigger one and move all your toys, which takes time.

### Linked List Implementation
Now imagine your toys are with friends standing in a line. Each friend has a toy and points to the next friend.

#### Advantages:
1. **Easy to Grow and Shrink**: You can easily add or remove friends. If you want to add a new friend, you just link them in without moving others.
2. **Efficient Use of Space**: No wasted slots. Each friend only holds a toy if there’s one to hold.
3. **Flexible Memory**: Friends can stand anywhere, so you don’t need a big space for all of them together.

#### Drawbacks:
1. **Extra Space for Pointers**: Each friend needs to remember who they point to, which takes extra space.
2. **Slower Search**: You can’t quickly jump to a specific friend. You have to start at the first friend and follow the line.
3. **No Caching**: Since friends can be anywhere, you can’t use special tricks to speed up looking at all the toys.

### Memory Requirements
- **Arrays**: Imagine your toy box has extra slots for future toys. When full, you get a bigger box and move all toys to the new box.
- **Linked Lists**: Each toy gets a new friend, and you never have extra friends without toys. But each friend needs to remember the next friend, which uses a bit more space.

### Summary
Arrays are like a neat toy box with numbered slots, great for quick access and searching but not so good for adding or removing toys in the middle. Linked lists are like a chain of friends holding toys, great for adding and removing toys easily but slower to search and needing more space for each friend’s pointer.

### Nodes
Imagine each of your friends is holding a toy and has a string to point to the next friend. This friend with a toy and a string is called a **node**.

- **Singly Linked List**: Each friend has one string pointing to the next friend.
- **Doubly Linked List**: Each friend has two strings, one pointing to the next friend and one pointing to the previous friend.

### Iterators
Think of an iterator like a magic pointer that helps you go through the line of friends without worrying about how they’re connected. This magic pointer can do a few things:

1. **First**: Point to the first friend in line.
2. **Next**: Move to the next friend in line.
3. **IsDone**: Check if the pointer has reached the end of the line.
4. **CurrentItem**: Show the toy the current friend is holding.

### Linked List
The linked list is like the master plan that knows where the first friend (node) is. This helps you follow the strings from one friend to another to see all the toys.

### Summary
- **Nodes** are friends holding toys with strings to other friends.
- **Singly Linked List**: Each friend has one string pointing to the next friend.
- **Doubly Linked List**: Each friend has two strings, one pointing to the next and one to the previous friend.
- **Iterators** are magic pointers that help you visit each friend one by one without worrying about the strings.
- **Linked List** is the master plan that knows where the first friend is, helping you follow the line and see all the toys.

### Linked List Overview
Imagine you have a magic toy box called **DList** (Doubly Linked List). This magic toy box doesn’t hold toys directly but knows where the first and last toy are.

### How We Make Our Linked List

#### Step 1: Creating the Magic Toy Box (DList)
First, we need a magic toy box that can remember where the first and last toys are:

```python
class LinkedList:
    def __init__(self):
        self.front = None  # Pointer to the first toy
        self.back = None   # Pointer to the last toy
```

- **front**: This is like a pointer that shows us where the first toy is.
- **back**: This is another pointer that shows us where the last toy is.

#### Step 2: Creating Nodes (Friends with Toys)
Now, let’s create friends who hold the toys and have strings to point to the next and previous friends:

```python
class LinkedList:
    class Node:
        def __init__(self, data, next=None, prev=None):
            self.data = data  # The toy
            self.next = next  # String pointing to the next friend
            self.prev = prev  # String pointing to the previous friend

    def __init__(self):
        self.front = None  # Pointer to the first friend
        self.back = None   # Pointer to the last friend
```

- **data**: The toy the friend is holding.
- **next**: The string pointing to the next friend in line.
- **prev**: The string pointing to the previous friend in line.

### How Nodes and Pointers Work
- If there are no toys yet, **front** and **back** both point to **None** (nothing).
- When we add a toy, we make a new friend (Node) and update the **front** and **back** pointers to point to this new friend.

### Example of Adding Toys
1. **First Toy**: When you add the first toy, **front** and **back** both point to this new friend.
2. **Second Toy**: When you add a second toy, the first friend points to the second friend, and the second friend points back to the first friend. Update **back** to point to the second friend.

### Special Value: None
- **None**: It’s like saying there’s no friend or toy. If a pointer points to **None**, it means it’s not pointing to any friend.

### Checking for None
To see if there is no toy or friend, we check if a pointer is **None**:

```python
ref = None
if(ref):
    print("reference refers to something")
else:
    print("reference refers to nothing (None)")
```

In this example, because `ref` is **None**, it prints “reference refers to nothing (None).”

### Summary
1. **DList**: A magic toy box that knows where the first and last toys are.
2. **Node**: Friends holding toys with strings pointing to the next and previous friends.
3. **None**: Means there is no toy or friend.

### Adding a Toy to the Front (push_front)

Imagine you have a toy box, and you want to add a new toy to the very front. Here’s how we do it:

#### Step 1: Create a New Friend Holding the Toy
First, you make a new friend who will hold the new toy and point to the friend currently at the front of the line.

```python
nn = self.Node(data, self.front)
```

- `nn` is the new friend holding the new toy.
- `self.front` is the current front friend.

#### Step 2: Link the Current Front Friend Back to the New Friend
Next, if there’s already a friend at the front, you need to make sure they point back to the new friend.

```python
if self.front is None:
    self.back = nn
else:
    self.front.prev = nn
```

- If there are no friends yet (`self.front` is `None`), make the new friend also the last friend.
- If there is a friend at the front, link them back to the new friend.

#### Step 3: Move the Front Pointer to the New Friend
Finally, update the front pointer to the new friend.

```python
self.front = nn
```

- Now, the new friend is at the front of the line.

### Full push_front Code
Putting all these steps together, here’s the full function to add a toy to the front:

```python
def push_front(self, data):
    nn = self.Node(data, self.front)
    if self.front is None:
        self.back = nn
    else:
        self.front.prev = nn
    self.front = nn
```

### Removing a Toy from the Front (pop_front)

Now, let’s remove the toy from the front of the toy box.

#### Step 1: Check if the Toy Box is Empty
First, check if there are any toys in the box. If it’s empty, do nothing.

```python
if self.front is not None:
```

- If there’s no friend at the front, we don’t need to do anything.

#### Step 2: Hold the Front Friend
Hold the front friend so we don’t lose them.

```python
rm = self.front
```

- `rm` is the front friend holding the toy we want to remove.

#### Step 3: Move the Front Pointer to the Next Friend
Move the front pointer to the second friend in line.

```python
self.front = self.front.next
```

- Now, the second friend becomes the first friend.

#### Step 4: Fix the Previous Pointer of the New Front Friend
If there’s a new front friend, make sure they don’t point back to the removed friend.

```python
if self.front is None:
    self.back = None
else:
    self.front.prev = None
```

- If there’s no friend left, also set the back pointer to `None`.
- Otherwise, make sure the new front friend’s previous pointer is `None`.

#### Step 5: Delete the Removed Friend
Finally, delete the friend who was at the front.

```python
del rm
```

### Full pop_front Code
Putting all these steps together, here’s the full function to remove a toy from the front:

```python
def pop_front(self):
    if self.front is not None:
        rm = self.front
        self.front = self.front.next
        if self.front is None:
            self.back = None
        else:
            self.front.prev = None
        del rm
```

### Summary
- **push_front**: Add a new friend with a toy to the front of the line.
- **pop_front**: Remove the friend at the front and move the front pointer to the next friend.
