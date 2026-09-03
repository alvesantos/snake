# Optional Values

Sometimes we work with variables that may or may not have an "actual value". For example, a character might have a damage bonus, or they might not. If they don't, we can represent that of value with `None`.

The `|` operator indicates that a value can be of multiple types:

```py
damage_bonus: int | None
```

That means `damage_bonus` can be either an integer (the bonus amount) or `None`. For another example, a function might return a prepared spell if one is ready, or `None` if no spells is prepared:

```py
def get_prepared_spell(has_spell: bool) -> str | None:
    if has_spell:
        return "Fireball"

    return None
```

## Assignment

1. Add a bool type hint to the has_mount parameter.
2. Add an int type hint to the distance parameter.
3. Add a str | None return type hint.