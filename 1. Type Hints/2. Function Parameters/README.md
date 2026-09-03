# Function Parameters

Can have type hints too! The syntax is the same variable type hints: put a colon after the parameter name, then the type.

```py
def greet_player(name: str):
    print(f"Welcome, {name}")
```

When a function has multiple parameters, each one can have its own type hint:

```py
def add_gold(current_gold: int, found_gold: int):
    return current_gold + found_gold
```

While adding a type hint to a variable declaration like:

```py
character_health: float = 72.5
```

is considered a bit redundant due to type inference, adding type hints to function parameters is not redundant. If you don't add them, your tooling won't know what types the function expects, which makes autocomplete and error checking less effective.

## Assignment

Fantasy Quest's character status function already works, but its parameters arent't labeled yet. Add type hint to the parameters of `get_character_status`

1. Add a str type hint to name
2. Add an int type hint to level
3. Add a float type hint to health
4. Add a bool type hint to has_magic

Don't change the function body.

