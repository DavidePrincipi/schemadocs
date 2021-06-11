# SHA256 string format Schema

```txt
http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/password_hash
```

A SHA256 string is 64 hexadecimal digits long

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                         |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [validate-input.json*](validate-input.json "open original schema") |

## password_hash Type

`string` ([SHA256 string format](cluster-defs-definitions-sha256-string-format.md))

## password_hash Constraints

**maximum length**: the maximum number of characters for this string is: `64`

**minimum length**: the minimum number of characters for this string is: `64`

**pattern**: the string must match the following regular expression: 

```regexp
^[a-f0-9]{64}$
```

[try pattern](https://regexr.com/?expression=%5E%5Ba-f0-9%5D%7B64%7D%24 "try regular expression with regexr.com")

## password_hash Examples

```json
"73cb3858a687a8494ca3323053016282f3dad39d42cf62ca4e79dda2aac7d9ac"
```
