# Nested Types

We've looked at relatively simple contaienr types like `list[str]`, but they can get more complex when one container holds another container. That is, it's possible to have nested container types.

A dictionary, for example, could map each character's name to their list of spells:

```py
character_spells: dict[str, list[str]] = {
    "Gandalf": ["Fireball", "Light"],
    "Frodo": ["Hide"],
}
```

We read `dict[str, list[str]]` from the outside in:

- It's a dictionary (`dict`)
- Each key is a string (`str`)
- Each value is a list of strings (`list[str]`)

In extreme cases, nested types can get super confusing, but honestly it's less consufing than in would be without the typing. For the time being, just know that type hints can describe containers withing containers.