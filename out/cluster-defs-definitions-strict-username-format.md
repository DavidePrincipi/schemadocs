# Strict username format Schema

```txt
http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/user
```

See <https://www.unix.com/man-page/linux/8/useradd/>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                         |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [validate-input.json*](validate-input.json "open original schema") |

## user Type

`string` ([Strict username format](cluster-defs-definitions-strict-username-format.md))

## user Constraints

**maximum length**: the maximum number of characters for this string is: `32`

**minimum length**: the minimum number of characters for this string is: `1`

**pattern**: the string must match the following regular expression: 

```regexp
^[a-z_][a-z0-9_-]*[$]?$
```

[try pattern](https://regexr.com/?expression=%5E%5Ba-z\_%5D%5Ba-z0-9\_-%5D\*%5B%24%5D%3F%24 "try regular expression with regexr.com")

## user Examples

```json
"admin"
```

```json
"u0000"
```

```json
"worker$"
```

```json
"test-user"
```

```json
"test_user"
```
