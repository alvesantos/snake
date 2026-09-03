# List and Set Hints

We've covered hints for basic types like `str`, `int`, `float`, and `bool`, but you can also add hints for container types: types that hold other values. For example:

- list: mutable sequence of values
- set: unordered collection of unique alues
- dict: collection of key-value pairs
- tuple: immutable sequence of values

When we type-hint a container, we specify waht kind of container it is and what type of values it contains. For example, a list of strings can be express as `list[str]`:

```py
inventory: list[str] = ["Iron Sword", "Healing Potion"]
```

The "contained" type goes in square brackets after the container type. Similarly, for a set of strings, we would write `set[str]`:

```py
unique_items: set[str] = {"Iron Sword", "Healing Potion"}
```

## Assignment

Fantasy Quest has a function that removes duplicate item names from a character's inventory. It works correctly but lacks annotation. Add type hints to `get_unique_items`.

1. Add a `list[str]` type hint to the inventory
2. Add a `set[str]` return type hint.