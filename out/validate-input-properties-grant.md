# Untitled array in add-user input Schema

```txt
undefined#/properties/grant
```

A list of initial roles on the matching cluster objects

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                         |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [validate-input.json*](validate-input.json "open original schema") |

## grant Type

`object[]` ([Grant object structure](user-grants.md))

## grant Constraints

**unique items**: all items in this array must be unique. Duplicates are not allowed.
