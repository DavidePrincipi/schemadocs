# Grant object structure Schema

```txt
undefined#/properties/grant/items
```

A grant object establishes a relation between a role and the cluster objects matching the "on" clause

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                         |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [validate-input.json*](validate-input.json "open original schema") |

## items Type

`object` ([Grant object structure](user-grants.md))

## items Examples

```json
{
  "role": "owner",
  "on": "*"
}
```

# items Properties

| Property      | Type     | Required | Nullable       | Defined by                                                                            |
| :------------ | :------- | :------- | :------------- | :------------------------------------------------------------------------------------ |
| [role](#role) | `string` | Optional | cannot be null | [Grant object structure](user-grants-properties-role.md "undefined#/properties/role") |
| [on](#on)     | `string` | Optional | cannot be null | [Grant object structure](user-grants-properties-on.md "undefined#/properties/on")     |

## role



`role`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Grant object structure](user-grants-properties-role.md "undefined#/properties/role")

### role Type

`string`

### role Constraints

**minimum length**: the minimum number of characters for this string is: `1`

## on



`on`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Grant object structure](user-grants-properties-on.md "undefined#/properties/on")

### on Type

`string`

### on Constraints

**minimum length**: the minimum number of characters for this string is: `1`
