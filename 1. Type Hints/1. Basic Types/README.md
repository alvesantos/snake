# Basic Types

To add a type hint to a variable declaration, put a colon after the variable name, then the type. This comes before the equals sign and the value:

```py
character_name: str = "Sir Galahad"
character_level: int = 7
character_health: float = 72.5
has_magic: bool = True
```

The values work the exact same way they did before. In fact, when it comes to simple variable declarations like this. you don't actually need the hint. In this example:

```py
caracter_health = 72.5
```

Because `character_health` is assigned a value of `72.5`, your tooling can infer that it's a `float`. That said, if you also want to see the type name, you can optionally add it.

## Assignment

Fanstasy Quest's character setup code works, but the variable types are wrong! Notice that our code editor's tooling gives un nice red squiggles to show u the mistakes. Fix the type hints for each variable.

1. character_name should be a str
2. character_level should be an int
3. character_health should be a float
4. has_magic should be a bool