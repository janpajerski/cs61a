Complete.
# Part 3: Solve a problem together
Imagine you can call only the following three functions:
- `f(x)`: Subtracts one from an integer `x`
- `g(x)`: Doubles an integer `x`
- `h(x, y)`: Concatenates the digits of two different positive integers `x` and `y`. For example, `h(789, 12)` evaluates to `78912` and `h(12, 789)` evaluates to `12789`.

**Definition**: A _small expression_ is a call expression that contains only `f`, `g`, `h`, the number 5, and parentheses. All of these can be repeated. For example, `h(g(5), f(f(5)))` is a small expression that evaluates to 103.

What's the shortest _small expression_ you can find that evaluates to 2024?
## Solution
I worked through the problem. I got `h(h(g(g(5)),f(f(f(5))),f(5))`. It's a solution, but not a general solution.  I'm not sure what they meant by the "shortest" and I wasn't able to find many resources around this problem. I'm okay moving on.
