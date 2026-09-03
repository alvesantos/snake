# Specific Container Types

It's possible to type-hint a container with just the container type:

```py
items: list = ["Black Firebomb", "Titanite Chunk"]
```

This says `items` is a list, but it doesn't tell us what kind of values go inside! Assuming you know what's inside, best to be specific:

```py
items: list[str] = ["Black Firebomb", "Titanite chunk"]
```

That said, bare container type hints aren't wrong. Sometimes you really don't know that types of values a container will hold, or the specific type hint would be too complicated to be userful. You'll see that occasionally with `dict`s. Just give clear type hint whenever possible.

## Assignment

1. Update `ìtems` from `list` to `list[str]`
2. Update `items_counts` from `dict` to `dict[str, int]`
3. Update the function return type from `tuple` to `tuple[str, int]`