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

### Sentinels in Linked Lists

Imagine you have a line of toy cars. Each car can connect to the one in front of it and the one behind it. Sometimes, you have to check if there's no car at the front or back, which can be tricky. So, let's add two special toy cars: one at the very front and one at the very back. These special cars don't hold any real data—they are just there to make things simpler. These special cars are called **sentinel nodes**.

### Constructor with Sentinels

When we first set up our line of toy cars, we create these two sentinel cars:

```python
class LinkedList:
    class Node:
        def __init__(self, data, next=None, prev=None):
            self.data = data
            self.next = next
            self.prev = prev

    def __init__(self):
        self.front = self.Node(None)
        self.back = self.Node(None, None, self.front)
        self.front.next = self.back
```

Here’s what this does:
- We have two special cars (nodes) with no data.
- The first special car (`front`) points to the second special car (`back`).
- The second special car points back to the first special car.

### `push_front` with Sentinels

Let’s add a new car to the front of our line:

```python
def push_front(self, data):
    nn = self.Node(data, self.front.next, self.front)
    self.front.next.prev = nn
    self.front.next = nn
```

Step-by-step:
1. We create a new car (`nn`) with the data we want.
2. The new car's next pointer points to the car that comes after the front sentinel.
3. The new car's previous pointer points to the front sentinel.
4. We update the next pointer of the front sentinel to point to our new car.
5. We also update the previous pointer of the car that was originally after the front sentinel to point back to our new car.

This way, the new car is correctly added right after the front sentinel, making it the first real car in the line.

### `pop_front` with Sentinels

Now let’s remove the first real car from the front of our line:

```python
def pop_front(self):
    if self.front.next is not self.back:
        rm = self.front.next
        rm.next.prev = rm.prev
        rm.prev.next = rm.next
        del rm
```

Step-by-step:
1. We check if there is a real car to remove. If the front sentinel's next pointer points to the back sentinel, it means there are no real cars, so we do nothing.
2. We point to the first real car (`rm`), which is the one after the front sentinel.
3. We update the next pointer of the front sentinel to skip this car and point to the next real car in line.
4. We update the previous pointer of the next real car to skip the car being removed and point back to the front sentinel.
5. Finally, we remove (`del`) the car from the line.

This way, the first real car is removed without any issues.

### Summary

Sentinel nodes are like special placeholder cars that help us manage our line of toy cars more easily. They ensure we always have a car at the front and back, which simplifies adding and removing cars. This means we don’t have to worry about special cases where the line is empty or has only one car. Instead, our functions can always assume there are at least two cars (the sentinels), making our code cleaner and simpler!

### Stacks and Queues

#### Stacks
Imagine you have a stack of pancakes. You can only add a new pancake to the top, and you can only take the top pancake off to eat it. This is called a **stack**. The last pancake you put on the stack is the first one you take off. So, it's a **First In, Last Out (FILO)** system.

#### Queues
Now, think of a line of people waiting for ice cream. The first person in line is the first to get ice cream, and new people join the end of the line. This is called a **queue**. The first person who came is the first to get served. So, it's a **First In, First Out (FIFO)** system.

### Operations

For both stacks and queues, you can do three main things:
1. **Add an item** (like adding a pancake or a person to the line).
2. **Remove an item** (like taking a pancake off the stack or serving the next person in line).
3. **See the next item to be removed** (like looking at the top pancake or seeing who's first in line).

Here’s what we call these operations:

| Operation                     | Stack     | Queue     |
|-------------------------------|-----------|-----------|
| **Add an item**               | Push      | Enqueue   |
| **Remove an item**            | Pop       | Dequeue   |
| **Access the "next" item**    | Top       | Front     |

### Stacks and Queues are Special Lists

- **Stacks**: Only work with the topmost pancake.
- **Queues**: Only work with the first person in line.

### Applications

- **Bracket checking**: Using stacks to see if parentheses in math expressions are balanced.
- **Breadth-first tree traversals**: Using queues to explore data structures like family trees.
- **Infix to postfix expressions**: Using stacks to convert math expressions.
- **Postfix expression calculation**: Using stacks to solve math expressions.

### Implementing a Stack

We can make a stack using either an array or a linked list.

#### Array Implementation
Think of an array like a row of boxes. We keep adding new boxes to the end. If we want to remove the last box, we just take it away. This makes adding and removing very quick.

#### Linked List Implementation
Imagine a chain of train cars. Each car links to the next one. If we always add new cars to the front, the newest car is always at the front, making it easy to add and remove cars quickly.

### Implementing a Queue

Like stacks, we can make a queue using either an array or a linked list.

#### Linked List Implementation
To make a queue with a linked list, think of adding new cars to the end of the train. The first car in line is the first to be removed. We can add cars quickly to the end and remove them quickly from the front.

#### Array Implementation
Using an array for a queue is trickier because we need to keep track of the front and back of the line. If the line goes out of bounds, we can think of the array as a circle where the end connects back to the beginning.

### Conclusion

- **Stacks**: Like a stack of pancakes. Last added is first removed (FILO).
- **Queues**: Like a line for ice cream. First added is first served (FIFO).

### What is a Table?

Imagine you have a toy box where each toy has a special tag with a number on it. This toy box is like a table. 

- **Table**: It's a box where you keep your toys. Each toy has a tag (key) and the toy itself (value).

### Key-Value Pair

- **Key**: The special number or tag on the toy. Each toy has a different tag number.
- **Value**: The toy itself. Different toys can have the same name (like two teddy bears), but they will have different tag numbers.

### Unique Keys

In your toy box, no two toys can have the same tag number. Each tag number is special and used only once.

### Table Operations

Here are the different things you can do with your toy box (table):

1. **Initialize**

   - **Initialize**: This means you start with an empty toy box. It’s like when you first get your toy box, and it doesn’t have any toys inside yet.

2. **isEmpty**

   - **isEmpty**: This is how you check if your toy box has any toys in it. If there are no toys, the toy box is empty.

3. **isFull**

   - **isFull**: This is how you check if your toy box has no more space to put any more toys in it. If there's no space left, the toy box is full.

4. **Insert**

   - **Insert**: This is when you add a new toy to your toy box. You put the toy in the box and give it a unique tag number.

5. **Delete**

   - **Delete**: This is when you take a toy out of your toy box. You look for the toy with a specific tag number and remove it from the box.

6. **Update**

   - **Update**: This is when you want to change a toy in your toy box. You find the toy with a specific tag number and change it to a new toy.

7. **Find**

   - **Find**: This is when you look for a toy in your toy box. You search for the toy by its tag number.

8. **Enumerate**

   - **Enumerate**: This is when you count or list all the toys in your toy box. You look at each toy and see how many you have.

### Putting It All Together

- You start with an empty toy box (initialize).
- You check if there are any toys in it (isEmpty).
- You can check if there's still space for more toys (isFull).
- You can add new toys with unique tag numbers (insert).
- You can take toys out by their tag numbers (delete).
- You can change a toy by finding its tag number and replacing it with a new toy (update).
- You can find a specific toy by its tag number (find).
- You can count or list all the toys in the box (enumerate).

### Simple Implementation of a Table

Think of your toy box again, but this time we are organizing the toys in a neat row, sorted by their tag numbers.

### Using an Array Sorted by Keys

Imagine lining up all your toys in a straight line, with each toy having a unique number (key) on its tag. The toys are arranged in order from the smallest number to the largest.

### Insertion/Update

When you want to add a new toy or change an existing one:

1. **Finding the Spot**: 
   - Imagine you have a magic way (binary search) to quickly find where a toy with a certain tag number should go in the line. This is like looking at the numbers quickly to find the right spot.
   - This magic search is very quick, and it takes a short time (O(log n)).

2. **Adding a New Toy**:
   - If there's no toy with that tag number, you have to make space for the new toy. This means shifting the toys over to make room. This can take a bit of time because you might have to move many toys (O(n)).

3. **Updating a Toy**:
   - If there's already a toy with that tag number, you just replace the old toy with the new one. This is quick (O(log n)).

### Removing a Toy

When you want to take a toy out of the line:

1. **Finding the Toy**:
   - You use the same magic way (binary search) to quickly find the toy by its tag number. This is quick (O(log n)).

2. **Removing and Shifting**:
   - Once you find the toy, you take it out and shift the other toys to fill the gap. This takes some time because you might have to move many toys (O(n)).

### Searching for a Toy

When you just want to find a toy by its tag number:

- You use the magic search (binary search) to quickly find it. This is quick (O(log n)).

### Drawbacks

This way of organizing your toys has some problems:

- **Searching**: Finding a toy is fast (O(log n)), which is good.
- **Adding New Toys**: Making space for new toys can be slow (O(n)) because you have to move a lot of toys.
- **Removing Toys**: Taking a toy out and shifting the others can be slow (O(n)) for the same reason.

### Summary

- Your toys are lined up in order by their tag numbers.
- Finding a toy is fast because you use a special search.
- Adding a new toy or removing one can be slow because you have to move other toys around.

This way of organizing is not perfect because only finding toys is fast, but adding and removing toys is slow. We need to find a better way to make everything fast!

### Hash Tables

Imagine you have a huge toy box with lots of little compartments (slots). Each toy has a special number (key) on it. A hash table helps you quickly find which compartment each toy goes into.

### Hash Functions

A hash function is like a magic spell that takes the number (key) on a toy and turns it into a smaller number. This smaller number tells you which compartment to put the toy in.

- **Hash Function**: A magic spell that always changes the same number into the same smaller number. It helps you decide where to put each toy.

### Example with Phone Numbers

Let's pretend each toy has a phone number tag like (###) ###-####. We want to use the phone number to decide which compartment it goes into.

- If we only used the first part of the phone number (area code), it wouldn't be good. Why? Because many toys might have the same area code and end up in the same compartment.
- Instead, using the last part of the phone number is better because it's more random and spreads the toys out better.

### Good Hash Functions

A good hash function makes sure:

- **Uniform**: All compartments are equally likely to get toys.
- **Random**: It's hard to predict where a toy will go, making the spread more even.

### Load Factor (λ)

Load factor is like checking how full your toy box is. It’s a number that shows how crowded your compartments are.

- **Load Factor (λ)**: The number of toys divided by the number of compartments.
  
  \[
  \lambda = \frac{\text{number of toys}}{\text{number of compartments}}
  \]

### Collisions

Collisions happen when two toys end up in the same compartment.

#### The Pigeonhole Principle

Imagine you have more toys (letters) than compartments (mailboxes). If you put all toys into compartments, at least one compartment will have more than one toy. This is called the pigeonhole principle.

- **Collision**: When two toys end up in the same compartment because the hash function gave them the same smaller number.

### Dealing with Collisions

Collisions are like when two friends want to sit in the same chair. Since this happens, we need ways to handle it:

1. **Separate Chaining**: Each compartment has a small line of chairs (a linked list). If more than one toy ends up in the same compartment, they just line up one behind the other.
2. **Open Addressing**: If a toy's compartment is full, we look for the next empty one in a specific way until we find one.

So, hash tables help us find places for our toys quickly, even if they sometimes end up trying to share a spot. We use smart ways to handle those times when they do share.

### Chaining in Hash Tables

Imagine you have a big toy box with many small compartments (slots). Each compartment can hold a line of toys, one behind the other (a linked list).

### How Chaining Works

1. **Hash Index**: A magic spell (hash function) changes a toy's number (key) into a smaller number. This smaller number tells you which compartment the toy goes into.

2. **Linked List**: Inside each compartment, toys can line up one after the other. If two toys get the same compartment number, they just form a line.

### Example with Chaining

Let's say you have 6 toys with these keys (special numbers): k1, k2, k3, k4, k5, k6. Your hash function changes these keys into smaller numbers (hash indexes) as follows:

- k1 -> 0
- k2 -> m - 3
- k3 -> m - 1
- k4 -> m - 3
- k5 -> 0
- k6 -> m - 3

If `m` is the number of compartments (slots), the toys will be stored like this:

- Compartment 0: k1, k5
- Compartment m - 3: k2, k4, k6
- Compartment m - 1: k3

Each compartment has a line of toys (linked list).

### Operations in Chaining

1. **Insert (k, v)**:
   - Find the compartment using the hash function.
   - Search the linked list in that compartment for the key.
   - If the key exists, update the toy.
   - If the key doesn't exist, add the new toy to the end of the line.

2. **Search (k)**:
   - Find the compartment using the hash function.
   - Search the linked list in that compartment for the key.
   - If the key is found, return the toy.
   - If the key is not found, the toy is not in the box.

3. **Delete (k)**:
   - Find the compartment using the hash function.
   - Search the linked list in that compartment for the key.
   - If the key is found, remove the toy from the line.
   - If the key is not found, the toy is not in the box.

### Run Time for Operations

- **Find Compartment**: Quick (takes the same time no matter how many toys) because we just use the magic spell (hash function).
- **Add/Modify/Delete Toy**: Quick, once we find the right spot in the line.
- **Search in Linked List**: Takes longer if the line is very long. The worst case is if all toys end up in one compartment, making the search slow (but this rarely happens).

### Load Factor (λ)

The load factor (λ) shows how full the compartments are:

\[
\lambda = \frac{\text{number of toys}}{\text{number of compartments}}
\]

### Worst Case vs. Average Case

- **Worst Case**: If all toys go into one compartment, searching the line takes a long time (θ(n)).
- **Average Case**: If toys are spread out evenly (which usually happens), each line is short, making the search quick (θ(1 + λ)).

### Summary

- Chaining uses a linked list in each compartment to handle collisions (when two toys want the same spot).
- Operations like insert, search, and delete are generally quick.
- The length of the lines (linked lists) depends on how full the table is (load factor λ).
- The worst-case scenario is rare, and usually, the operations are efficient.

### 1. Linear Probing vs Chaining

#### **Chaining**
- **Chaining** uses a "second dimension" to handle collisions in a hash table.
- Imagine each slot in the hash table has a "bucket" where multiple items can be stored if they hash to the same slot.
- When you look for an item, you only look at the bucket of the calculated hash slot.
- Chaining is like having multiple boxes at each slot, so you can store several items in one place if needed.

#### **Linear Probing**
- **Linear Probing** only allows one item per slot.
- If there's a collision (two items hash to the same slot), it looks for the next available slot.
- Linear probing checks the next slot, and if it's full, the next one, and so on.
- This is like a single line of boxes where each box can hold only one item, and if a box is full, you look for the next empty box.

### 2. How Linear Probing Works

#### **Insertion**
- **Step 1**: Use a hash function to find the index for a record.
- **Step 2**: If the spot is occupied, look for the next available spot in a higher index.
- **Step 3**: Treat the hash table as circular. If you reach the end, go back to the front.
- **Example**: 
  - You have keys (items) k1 to k5.
  - k1 goes to slot 8, k2 to slot 7, k3 to slot 9, k4 to slot 1.
  - k5 also hashes to slot 8. Since it's full, you put k5 in the next available slot, which is 0.

#### **Searching**
- **Step 1**: Use the hash function to find where an item should be.
- **Step 2**: If the slot is occupied by something else, search the next slots until you find the item or an empty slot.
- **Note**: Stop searching as soon as you find an empty spot.

#### **Removal**
- **Step 1**: Find the record and remove it, leaving an empty spot.
- **Step 2**: Check the following records in the cluster (group of continuous records).
- **Step 3**: Move records to fill the empty spot if needed.
- **Example**:
  - You have a cluster of items from slot 7 to 1.
  - Remove k3 from slot 9.
  - If needed, move items to keep the cluster intact.

### 3. Tombstoning

#### **Statuses**
- **Empty**: No item has ever been placed here.
- **Occupied**: A record is stored here.
- **Deleted**: An item was here but has been deleted.

#### **Insertion**
- **Step 1**: If the spot is empty or marked as deleted, put the item there.

#### **Searching**
- **Step 1**: Use the hash function to find where the item should be.
- **Step 2**: Check if the key matches. If not, look in the next slot according to the probing method until you find it or hit an empty slot.

#### **Removal**
- **Step 1**: Find the record and mark it as deleted.
- **Example**:
  - Insert items k1 to k3 without collisions.
  - Insert k4, k5, and k6. Handle collisions by placing them in the next available slot.
  - If you search for k5, look in the slots according to its probe sequence until you find it.

### 4. Quadratic Probing

#### **How It Works**
- Instead of looking at the next slot, quadratic probing uses a formula to decide where to look next.
- The formula: `hash(k) + i^2` for i = 0, 1, 2, 3, etc.
- This means you look at the slot, then 1 slot away, then 4 slots away, then 9 slots away, and so on.

#### **Example**
- Insert k1 to k3 (no collisions).
- Insert k4. If slots are occupied, use the probe sequence to find the next spot.
- Insert k5 using its quadratic probe sequence.

### 5. Double Hashing

#### **How It Works**
- Uses two different hash functions.
- The first hash function finds the initial position.
- The second hash function determines the offset for the next probes.
- The probe sequence: `hash1(k), (hash1(k) + hash2(k)) % m, (hash1(k) + 2 * hash2(k)) % m, ...`

#### **Example**
- Insert k1, k2, k3 without collisions.
- Insert k4. If there's a collision, use the second hash function to find the next spot.
- Insert k5 using its double hash sequence.

### Summary

- **Chaining**: Multiple items per slot using a second dimension.
- **Linear Probing**: One item per slot, look for next empty slot if needed.
- **Tombstoning**: Marks slots as empty, occupied, or deleted.
- **Quadratic Probing**: Uses a formula to find next slots further away.
- **Double Hashing**: Uses two hash functions to find next slots.

I understand your question. Let's make it clear how the hash indices are calculated in the context of our example.

In our example, the hash function for determining the index where each toy should be stored is based on the first letter of the toy's name. Let's assume a simple hash function where:

- `hash1(toy) = (ASCII value of the first character) % 10`
- `hash2(toy) = (ASCII value of the second character) % 10` (used only for double hashing)

### Let's define the toy names and their corresponding hash indices:

Let's assume toy names are `k1`, `k2`, `k3`, `k4`, `k5`, `k6`, and `k7`.

To get their ASCII values:

- `k` has an ASCII value of 107.
- `1`, `2`, `3`, `4`, `5`, `6`, and `7` have ASCII values 49, 50, 51, 52, 53, 54, and 55 respectively.

### Calculating Hash Indices

For simplicity, let's focus on the hash1 function for now.

#### k1:
- First character: `k` -> ASCII value 107
- `hash1(k1) = 107 % 10 = 7`

#### k2:
- First character: `k` -> ASCII value 107
- `hash1(k2) = 107 % 10 = 7`

#### k3:
- First character: `k` -> ASCII value 107
- `hash1(k3) = 107 % 10 = 7`

#### k4:
- First character: `k` -> ASCII value 107
- `hash1(k4) = 107 % 10 = 7`

#### k5:
- First character: `k` -> ASCII value 107
- `hash1(k5) = 107 % 10 = 7`

#### k6:
- First character: `k` -> ASCII value 107
- `hash1(k6) = 107 % 10 = 7`

#### k7:
- First character: `k` -> ASCII value 107
- `hash1(k7) = 107 % 10 = 7`

Since all toys have the same first character `k`, their `hash1` values will all be 7.

### Example with Linear Probing

Now, let’s rework the example to handle collisions using linear probing.

#### Initial Insertions:

1. **k1**: 
   - `hash1(k1) = 7`
   - Insert **k1** at box 7.

2. **k2**:
   - `hash1(k2) = 7`
   - Box 7 is occupied.
   - Move to box 8.
   - Insert **k2** at box 8.

3. **k3**:
   - `hash1(k3) = 7`
   - Box 7 is occupied.
   - Box 8 is occupied.
   - Move to box 9.
   - Insert **k3** at box 9.

4. **k4**:
   - `hash1(k4) = 7`
   - Box 7 is occupied.
   - Box 8 is occupied.
   - Box 9 is occupied.
   - Move to box 0.
   - Insert **k4** at box 0.

5. **k5**:
   - `hash1(k5) = 7`
   - Box 7 is occupied.
   - Box 8 is occupied.
   - Box 9 is occupied.
   - Box 0 is occupied.
   - Move to box 1.
   - Insert **k5** at box 1.

6. **k6**:
   - `hash1(k6) = 7`
   - Box 7 is occupied.
   - Box 8 is occupied.
   - Box 9 is occupied.
   - Box 0 is occupied.
   - Box 1 is occupied.
   - Move to box 2.
   - Insert **k6** at box 2.

7. **k7**:
   - `hash1(k7) = 7`
   - Box 7 is occupied.
   - Box 8 is occupied.
   - Box 9 is occupied.
   - Box 0 is occupied.
   - Box 1 is occupied.
   - Box 2 is occupied.
   - Move to box 3.
   - Insert **k7** at box 3.

The final state of the toy boxes is:

```
0  1  2  3  4  5  6  7  8  9
k4 k5 k6 k7 -  -  -  k1 k2 k3
```

### Double Hashing Example

Now, let’s rework the example to handle collisions using double hashing.

#### Initial Insertions:

1. **k1**:
   - `hash1(k1) = 7`
   - Insert **k1** at box 7.

2. **k2**:
   - `hash1(k2) = 7`
   - `hash2(k2) = 50 % 10 = 0`
   - Box 7 is occupied.
   - Move to box `(7 + 0) % 10 = 7`.
   - Box 7 is occupied.
   - Move to box `(7 + 0*0) % 10 = 7`.
   - Insert **k2** at box 0.

3. **k3**:
   - `hash1(k3) = 7`
   - `hash2(k3) = 51 % 10 = 1`
   - Box 7 is occupied.
   - Move to box `(7 + 1) % 10 = 8`.
   - Insert **k3** at box 8.

4. **k4**:
   - `hash1(k4) = 7`
   - `hash2(k4) = 52 % 10 = 2`
   - Box 7 is occupied.
   - Move to box `(7 + 2) % 10 = 9`.
   - Insert **k4** at box 9.

5. **k5**:
   - `hash1(k5) = 7`
   - `hash2(k5) = 53 % 10 = 3`
   - Box 7 is occupied.
   - Move to box `(7 + 3) % 10 = 0`.
   - Box 0 is occupied.
   - Move to box `(7 + 2*3) % 10 = 3`.
   - Insert **k5** at box 3.

6. **k6**:
   - `hash1(k6) = 7`
   - `hash2(k6) = 54 % 10 = 4`
   - Box 7 is occupied.
   - Move to box `(7 + 4) % 10 = 1`.
   - Insert **k6** at box 1.

7. **k7**:
   - `hash1(k7) = 7`
   - `hash2(k7) = 55 % 10 = 5`
   - Box 7 is occupied.
   - Move to box `(7 + 5) % 10 = 2`.
   - Insert **k7** at box 2.

The final state of the toy boxes with double hashing is:

```
0  1  2  3  4  5  6  7  8  9
k2 k6 k7 k5 -  -  -  k1 k3 k4
```

### Trees

**Trees** are a very important data structure in computer science. They are used to organize data hierarchically, which helps in searching and managing data efficiently. Trees are used in many areas of computing, such as databases, file systems, and more.

### Definitions

#### Node
- A **node** is a fundamental part of a tree that stores data. In diagrams, each circle represents a node.
  
#### Root Node
- The **root node** is the topmost node in a tree from which all other nodes branch out. In the given diagram, **A** is the root node.

#### Subtree
- A **subtree** is a portion of a tree that includes a node and all its descendants (all nodes that come down from it). For example, if we consider **B** as the root of a subtree, then the subtree includes **B**, **D**, **E**, and **F**.

#### Empty Trees
- An **empty tree** is a tree with no nodes at all.

#### Leaf Node
- A **leaf node** is a node that does not have any children. It is at the end of a branch. Examples from the diagram include **D**, **E**, **F**, **I**, **J**, and **G**.

#### Children
- **Children** are nodes that are directly connected one level below a given node. For example, **B** is a child of **A**. **I** is a child of **H**.

#### Parent
- A **parent** is a node directly connected one level above a given node. For instance, **A** is the parent of **B**. **H** is the parent of **I**.

#### Sibling
- **Siblings** are nodes that share the same parent. For example, **E** and **F** are siblings since they both share **D** as their parent. However, **H** is not a sibling of **E** and **F**.

#### Ancestor
- An **ancestor** is any node that can be reached by moving upwards from a given node. For example, **C**, **A**, and **H** are all ancestors of **I**. **B** and **G** are not.

#### Descendants (or Successors)
- **Descendants** (or **successors**) are nodes that can be reached by moving downwards from a given node. For instance, **G**, **H**, **I**, and **J** are descendants of **C**.

#### Depth
- **Depth** is the distance from the root node to a particular node. The root node is at depth 0. **B** and **C** are at depth 1. **D**, **E**, **F**, **G**, and **H** are at depth 2. **I** and **J** are at depth 3.

#### Height
- **Height** is the total number of nodes from the root to the furthest leaf. The height of the given tree is 4.

#### Path
- A **path** is a sequence of nodes and edges connecting a node to an ancestor or descendant. For example, the path from **A** to **J** might be described as **A -> C -> H -> J**.

#### Binary Tree
- A **binary tree** is a tree where every node has at most two children, which are referred to as the left child and the right child. The given tree is not a binary tree because node **B** has three children.

### Tree Implementation

#### Linked Structure
- Trees are often implemented using a linked structure similar to linked lists. In a linked list, each node contains data and a pointer to the next node (and sometimes to the previous node). In a tree, each node contains data and pointers to its children.

#### Array/List Implementation
- Trees can also be implemented using arrays or lists. For a binary heap, the root is stored at index 0. For any node stored at index \(i\):
  - The left child's index is \(2i + 1\)
  - The right child's index is \(2i + 2\)
  - The parent's index is \(\left\lfloor\frac{i-1}{2}\right\rfloor\)
  
  This method is efficient for complete trees (trees where every level, except possibly the last, is fully filled, and all nodes are as far left as possible). For non-complete trees, it can lead to many unused spaces in the array.

### Summary
- Trees are hierarchical data structures used for efficient data organization and search.
- Nodes are the basic elements of trees.
- The root node is the topmost node.
- Subtrees are parts of the tree starting from a node.
- Empty trees have no nodes.
- Leaf nodes have no children.
- Children are nodes directly below a parent node.
- Parents are nodes directly above a child node.
- Siblings share the same parent.
- Ancestors are nodes that can be reached by moving upwards.
- Descendants are nodes that can be reached by moving downwards.
- Depth is the distance from the root node.
- Height is the total number of nodes from the root to the furthest leaf.
- Paths are sequences of nodes connecting an ancestor to a descendant.
- Binary trees have at most two children per node.
- Trees can be implemented using linked structures or arrays/lists.

### Heap and Heap Sort

**Heap Sort** is a sorting algorithm that uses a binary heap data structure to sort elements. A binary heap is a type of complete binary tree which can be used to implement a priority queue.

### Priority Queue

A **priority queue** is a special type of queue where the element that comes out next depends on its priority rather than the order in which it was added. In a regular queue, the first element in is the first element out (FIFO - First In, First Out). In a priority queue, elements are removed based on their priority.

### Basic Operations on a Binary Heap

#### Insert
- **Insert** operation adds an item to the binary heap. The new item is initially added at the end of the heap and then "bubbled up" to its correct position to maintain the heap property.

#### Delete
- **Delete** operation removes the item with the highest priority (in a max-heap) or the lowest priority (in a min-heap) from the binary heap. The root element is removed and replaced with the last element in the heap, which is then "bubbled down" to its correct position to maintain the heap property.

### Binary Heap

A **binary heap** is a complete binary tree that satisfies the heap property:
- **Max-Heap:** The value of each node is greater than or equal to the values of its children.
- **Min-Heap:** The value of each node is less than or equal to the values of its children.

### Heap Sort Algorithm

The idea behind **Heap Sort** is to use the binary heap to sort an array. The steps are:

1. **Build the Heap:** Convert the array into a binary heap. This involves inserting each element of the array into the heap. If it's a max-heap, the largest element will be at the root; if it's a min-heap, the smallest element will be at the root.
2. **Sort the Array:** Repeatedly remove the root (the largest or smallest element) from the heap and place it at the end of the array. After each removal, reheapify the remaining elements to maintain the heap property. This process continues until all elements have been removed from the heap and placed back into the array in sorted order.

### Detailed Steps of Heap Sort

1. **Build the Heap**
   - Start with an unsorted array.
   - Insert each element into the binary heap. For example, if you have an array `[4, 10, 3, 5, 1]`, you insert 4, then 10, then 3, and so on, maintaining the heap property at each step.

2. **Heapify**
   - After building the heap, ensure that the heap property is maintained throughout the tree. For example, in a max-heap, the largest element should always be at the root.

3. **Sort the Array**
   - Remove the root element (the largest in a max-heap or the smallest in a min-heap) and place it at the end of the array.
   - Replace the root with the last element in the heap and reduce the heap size by one.
   - Reheapify the heap to maintain the heap property.
   - Repeat this process until all elements are sorted.

### Example of Heap Sort

Let's say we have an array `[4, 10, 3, 5, 1]` and we want to sort it using heap sort.

1. **Build the Heap:** Convert the array into a max-heap:
   ```
   Initial array: [4, 10, 3, 5, 1]
   Max-Heap:      [10, 5, 3, 4, 1]
   ```

2. **Sort the Array:** Repeatedly remove the largest element and reheapify:
   ```
   Remove 10: [5, 4, 3, 1, 10]
   Reheapify: [5, 4, 3, 1]
   Remove 5:  [4, 1, 3, 5, 10]
   Reheapify: [4, 1, 3]
   Remove 4:  [3, 1, 4, 5, 10]
   Reheapify: [3, 1]
   Remove 3:  [1, 3, 4, 5, 10]
   Reheapify: [1]
   Remove 1:  [1, 3, 4, 5, 10]
   ```

   The array is now sorted: `[1, 3, 4, 5, 10]`.

### Summary
- **Heap Sort** is a sorting algorithm that uses a binary heap to sort elements.
- A **priority queue** allows elements to be removed based on their priority.
- A **binary heap** is a complete binary tree that satisfies the heap property (max-heap or min-heap).
- **Insert** operation adds an item to the heap and ensures the heap property is maintained.
- **Delete** operation removes the root (highest or lowest priority) and reheapifies the remaining elements.
- **Heap Sort** involves building a heap from the array and repeatedly removing the root element to sort the array.

