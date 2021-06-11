# add-user input Schema

```txt
undefined
```

Create a user account for the cluster administration web interface

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                        |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [validate-input.json](validate-input.json "open original schema") |

## add-user input Type

`object` ([add-user input](validate-input.md))

## add-user input Examples

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

# add-user input Properties

| Property                        | Type     | Required | Nullable       | Defined by                                                                         |
| :------------------------------ | :------- | :------- | :------------- | :--------------------------------------------------------------------------------- |
| [user](#user)                   | `string` | Required | cannot be null | [add-user input](username-strict.md "undefined#/properties/user")                  |
| [password_hash](#password_hash) | `string` | Required | cannot be null | [add-user input](sha256-string.md "undefined#/properties/password_hash")           |
| [set](#set)                     | `object` | Required | cannot be null | [add-user input](user-attributes.md "undefined#/properties/set")                   |
| [grant](#grant)                 | `array`  | Required | cannot be null | [add-user input](validate-input-properties-grant.md "undefined#/properties/grant") |

## user

See <https://www.unix.com/man-page/linux/8/useradd/>

`user`

*   is required

*   Type: `string` ([Strict username validation schema](username-strict.md))

*   cannot be null

*   defined in: [add-user input](username-strict.md "undefined#/properties/user")

### user Type

`string` ([Strict username validation schema](username-strict.md))

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

A SHA256 string is 64 hexadecimal numbers long

`password_hash`

*   is required

*   Type: `string` ([SHA256 string format](sha256-string.md))

*   cannot be null

*   defined in: [add-user input](sha256-string.md "undefined#/properties/password_hash")

### password_hash Type

`string` ([SHA256 string format](sha256-string.md))

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

Display name and similar...

`set`

*   is required

*   Type: `object` ([User attributes](user-attributes.md))

*   cannot be null

*   defined in: [add-user input](user-attributes.md "undefined#/properties/set")

### set Type

`object` ([User attributes](user-attributes.md))

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

*   Type: `object[]` ([Grant object structure](user-grants.md))

*   cannot be null

*   defined in: [add-user input](validate-input-properties-grant.md "undefined#/properties/grant")

### grant Type

`object[]` ([Grant object structure](user-grants.md))

### grant Constraints

**unique items**: all items in this array must be unique. Duplicates are not allowed.
