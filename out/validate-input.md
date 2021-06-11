# Add-user (input) Schema

```txt
http://nethserver.org/json-schema/task/input/cluster/add-user
```

Create a user account for the cluster administration web interface

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                        |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [validate-input.json](validate-input.json "open original schema") |

## Add-user (input) Type

`object` ([Add-user (input)](validate-input.md))

## Add-user (input) Examples

```json
{
  "user": "admin",
  "password_hash": "73cb3858a687a8494ca3323053016282f3dad39d42cf62ca4e79dda2aac7d9ac",
  "set": {
    "display_name": "The Administrator"
  },
  "grant": [
    {
      "role": "owner",
      "on": "*"
    }
  ]
}
```

# Add-user (input) Properties



## user

See <https://www.unix.com/man-page/linux/8/useradd/>

`user`

*   is required

*   cannot be null

*   defined in: [Add-user (input)](cluster-defs-definitions-strict-username-format.md "http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/user")

### user Type

`string` ([Strict username format](cluster-defs-definitions-strict-username-format.md))

### user Constraints

**maximum length**: the maximum number of characters for this string is: `32`

**minimum length**: the minimum number of characters for this string is: `1`

**pattern**: the string must match the following regular expression: 

```regexp
^[a-z_][a-z0-9_-]*[$]?$
```

[try pattern](https://regexr.com/?expression=%5E%5Ba-z\_%5D%5Ba-z0-9\_-%5D\*%5B%24%5D%3F%24 "try regular expression with regexr.com")

### user Examples

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

## password_hash

A SHA256 string is 64 hexadecimal digits long

`password_hash`

*   is required

*   cannot be null

*   defined in: [Add-user (input)](cluster-defs-definitions-sha256-string-format.md "http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/password_hash")

### password_hash Type

`string` ([SHA256 string format](cluster-defs-definitions-sha256-string-format.md))

### password_hash Constraints

**maximum length**: the maximum number of characters for this string is: `64`

**minimum length**: the minimum number of characters for this string is: `64`

**pattern**: the string must match the following regular expression: 

```regexp
^[a-f0-9]{64}$
```

[try pattern](https://regexr.com/?expression=%5E%5Ba-f0-9%5D%7B64%7D%24 "try regular expression with regexr.com")

### password_hash Examples

```json
"73cb3858a687a8494ca3323053016282f3dad39d42cf62ca4e79dda2aac7d9ac"
```

## set

Attributes of a User

`set`

*   is required

*   cannot be null

*   defined in: [Add-user (input)](cluster-defs-definitions-user-attributes.md "http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/set")

### set Type

`object` ([User attributes](cluster-defs-definitions-user-attributes.md))

### set Examples

```json
{
  "display_name": "Mighty Admin"
}
```

## grant

A list of initial roles on the matching cluster objects

`grant`

*   is required

*   cannot be null

*   defined in: [Add-user (input)](validate-input-properties-grant-assertions-list.md "http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/grant")

### grant Type

`object[]` ([Grant object](cluster-defs-definitions-grant-object.md))

### grant Constraints

**unique items**: all items in this array must be unique. Duplicates are not allowed.
