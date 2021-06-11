# Grant assertions list Schema

```txt
http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/grant
```

A list of initial roles on the matching cluster objects

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                         |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [validate-input.json*](validate-input.json "open original schema") |

## grant Type

`object[]` ([Grant object](cluster-defs-definitions-grant-object.md))

## grant Constraints

**unique items**: all items in this array must be unique. Duplicates are not allowed.
