# Dictionary Hints

Dictionaries are container types too, but they map keys to values, so their type hints include both:

```py
item_counts: dict[str, int] = {
    "Wooden Arrow": 30,
    "Small Amethyst": 2
}
```

The first type is for the keys; the second is for the values.

```py
dict[key_type, value_type]
```

So `dict[str, int]` means:

- The keys are strings
- The values are integers

Not all types can be used as dictionary keys. The key types that you'll see most often are strings and integers. Dictionary values, on the other hand, can be any type.

## Assignment

Fantasy Quest also tracks how many of each item a character has in their inventory. Add type hints to the `get_item_count` function.

1. Add a `dict[str, int]` type hint to the item_counts parameter.
2. Add a `str` type hint to the `item_name` parameter
3. Add an `int` return type hint