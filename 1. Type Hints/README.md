# Type Hints

Some Functions accept numbers as arguments; others accept strings. Some return lists; others return dictionaries, booleans, or None.

When a program is small, you can usually remember the types of your variables. But as programs grow, it's easy to forget:

- Is `level` an `int` or a `str`?
- Does `get_item()` always return an item name (`str`), or sometimes `None` if it can't find one?
- Is `Inventory` a list of strings, or a dictionary of item counts?

```py
def get_damage(weapon: dict, level: int) -> int:
    return weapon["damage"] + (level * 2)
```

The `weapon: dict`, `level: int`, and -> `int` parts are type hints. They tell humans and code editors what kinds of values the function expects and returns.

Type hints don't make Python stop being Python. It's still a dynamically typed language, and it won't automatically reject the wrong value just because a type hint says so.

Type hints are for:

- Making code easier to read
- Helping your editor autocomplete and warn you about mistakes
- Making bugs easier to spot before running your code

