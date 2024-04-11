---
tags:
  - problem-solving
  - programming
---
The three steps in the problem solving process (in programming)
# Programming
See [How to think like a programmer](freecodecamp.org/news/how-to-think-like-a-programmer-lessons-in-problem-solving-d1d8bf1de7d2/) and [The Odin Project - Problem Solving](https://www.theodinproject.com/lessons/foundations-problem-solving)
## 1. Understand The Problem
- Understand exactly what the problem is. 
- Write it down on paper, reword it in plain English until it makes sense, draw diagrams, etc., 
- If you can explain the problem to someone else in plain English, you understand it
## 2. Plan
Before jumping into code, into solving the problem, plan out how you're going to solve it. 
Some useful questions to ask:
- Is there a user interface? What will it look like? What functionality will the interface have? Sketch this out.
- What inputs will your program have? Will the user enter data or will you get input from somewhere else?
- What's the desired output?
- Given the inputs, what are the steps necessary to return the desired output? **This is where you write out an algorithm in pseudocode**
### Pseudocode
- Writing out the logic of your program in natural language instead of code. 
- Here is an example:
```
  When the user inputs a number
  Initialize a counter variable and set its value to zero
  While the counter is smaller than user inputted number, increment the counter by one
  Print the value of the counter variable
```
## 3. Divide and Conquer
**Break the big problem down and solve each of the smaller problems until you’ve solved the big problem.**

From your planning, you should have identified some subproblems of the big problem you’re solving. Each of the steps in the algorithm we wrote out in the last section are subproblems. Pick the smallest or simplest one and start there with coding.

It’s important to remember that you might not know all the steps that you might need up front, so your algorithm may be incomplete -— this is fine. Getting started with and solving one of the subproblems you have identified in the planning stage often reveals the next subproblem you can work on. Or, if you already know the next subproblem, it’s often simpler with the first subproblem solved.

==Many beginners try to solve the big problem in one go. **Don’t do this**==. If the problem is sufficiently complex, you’ll get yourself tied in knots and make life a lot harder for yourself. Decomposing problems into smaller and easier to solve subproblems is a much better approach. Decomposition is the main way to deal with complexity, making problems easier and more approachable to solve and understand.
# From CS61a
See the [cs61a study guide](https://cs61a.org/articles/studying/)
## 1. Reinterpret the problem prompt
Read _and reinterpret_ the question. Usually, we begin with a description of the problem to be solved. What's important is not just reading the problem, but thinking critically about the implications of the details in the problems and clear up any ambiguities. Don't jump into coding directly without first thinking through the problem and posing questions for ourselves.

A couple concrete starting questions to ask yourself on any problem include:

- What is the **domain** (input) and **range** (output) of the program?
- Restate the intended behavior of the program in your own words.
- How will the values in this program change as the program executes?

Verify your understanding by studying the doctests. In computer science, the mental representation for a problem is often closely related to its solution.

**Big hints are always given away in the doctest!** The doctests inform us about the shape and format of the solution. If we look closely enough for the patterns in the doctest, we'll often expose details in the structure of how the problem is meant to be solved.

Although they provide many hints, the doctests are not exhaustive and they usually don't show the most important cases. Develop examples that cover at least the following situations:

- What's the smallest or simplest possible input I could give to this function?
- Is there a similar small input that is _invalid_ for this problem? How is it related to or different from the earlier case?
- Can we come up with any larger inputs to the program that are related to or rely on smaller cases? The idea is to come up with some of the subproblems we might have to solve with recursion or other techniques.
## 2. Search for analogous problems
Does this problem look similar to something you've seen before? Armed with your experience from homework, lab, and discussion, develop a general idea of how to solve the problem.

Once we've identified a similar problem, we can then extract the general strategy for solving the problem. While details are useful, copy-and-pasting the solution from the analogous problem usually won't get us very far. Instead, verbalize the code and reinterpret it in English by asking, "What's the purpose of including this code?"
## 3. Adapting previous solutions

Implement a solution by applying the problem solving techniques you've learned alongside your experience with analogous problems. With recursion, for example, it helps to try to follow the steps of finding a base case, identifying the recursive calls, and then combining the results. However, the particular implementation in code will depend upon the specific details of the problem.

This is where our rigorous understanding of the problem will come in handy. We found an analogous problem that has a similar, but not exactly the same behavior, so we have a **general approach** in mind. We know the domain, range, and behavior in the correct program. Using _problem-solving techniques_ learned in class, _apply the general approach_ to the particular problem to come up with a rough draft that is a step towards the solution.

It might not be fully correct, but that's fine and completely normal; refining mental representations of the problem takes time and practice.

## 4. Evaluating solutions

Analyze and test the resulting implementation. We'd like to answer two central questions:

1. Is my approach on the right track? If not, maybe we should consider another analogous problem.
2. If my approach is in the right direction, **let's evaluate** and verify the correctness of the solution.

**To improve our code, we just need to ask ourselves the right questions.** What input would break the program? Think like Python: run through the code step-by-step until there's a problem. We have examples of what the output should look like, so make sure the actual result matches expectations.

If the results aren't consistent, let's try to identify why and make adjustments by asking more specific questions. Where is the root of problem? Let's trace back through the code to find the source of the problem. Then, once we've found the problem, let's try the same approach of searching for analogous