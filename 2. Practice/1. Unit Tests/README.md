# Unit Tests

If you end up working as programmer, you'll spend a lot of time writing your own unit tests. So far we've provided unit tests for you, but it's useful to know how they work.

When you're doing your own testing, you'll usually use a library for writing and running tests. For example in Python, pytest and unittest are quite popular.

But it's also OK to write tests from scratch sometimes. We do that on Boot.dev so that the tests integrate nicely with our online environment. That's what the `main_test.py` file is: a custom test harness that we've written for each of your lessons.

## Assignment

Let's flit the script: in `main.py` you'll find a read-only, almost correct function called `avg_luck_boost`. It's used in Fantasy Quest to calculate the average "luck" boost granted to a party of players when they defeat a boss, to determine the loot that they receive.

The function can be used like this:

```py
luck_boosts: list[int] = [5, 3, 10]
avg_boost: float = avg_luck_boost(luck_boosts)
print(avg_boost) #6.0
```

Run the tests. Notice that they all pass! But there's a problem... some odd behavior isn't covered by the existing test cases.

What happes inf no party member has a luck boost? The function will try to divide by zero, i.e. the length of the input list, and crash the program.

```py
luck_boosts: list[int] = []
avg_boost: float = avg_luck_boost(luck_boosts) #ZeroDivisionError
```

What we want this function to do if the input list is empty is to return `0.0`. Add that expected result to `test_cases.py`; we'll fix the function in the next lesson

1. Add a new dictionary to the `run_cases` list, with `luck_boosts` set to an empty list, and `exptected_avg` set to `0.0`