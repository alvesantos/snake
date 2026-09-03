# Fix a Falling Test

We have a failing test case for our `avg_luck_boost` function! When an empty list is passed to the function, it should return `0.0`. Instead, it tries to divide by zero and crashes.

Let's update `avg_luck_boost` so that all tests pass again.

Some programmers like to work this way; it's called "test-dirven development":

1. Stub out a function
2. Write tests that expect the correct behavior of that function
3. Run the tests (they should fail)
4. Implement the function and keep updating it until it passes the tests.

TDD is ometimes a controversial topic, and we won't dive into that here. But we will give you much more practice with writing tests in later courses.

## Assignment

Fix the `avg_luck_boost` function in `main.py`.

1. At the beggining of the function, check if `luck_boosts` is an empty list. If so, just return `0.0` to avoid a divide-by-zero error.