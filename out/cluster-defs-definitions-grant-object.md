# Grant object Schema

```txt
http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/grant/items
```

A grant object establishes a relation between a role and the cluster objects matching the "on" clause

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                         |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [validate-input.json*](validate-input.json "open original schema") |

## items Type

`object` ([Grant object](cluster-defs-definitions-grant-object.md))

## items Examples

```json
{
  "role": "owner",
  "on": "*"
}
```

# items Properties



## role



`role`

*   is optional

*   cannot be null

*   defined in: [Cluster library](cluster-defs-definitions-grant-object-properties-role.md "http://nethserver.org/json-schema/task/library/cluster#/definitions/grant-object/properties/role")

### role Type

`string`

### role Constraints

**minimum length**: the minimum number of characters for this string is: `1`

## on



`on`

*   is optional

*   cannot be null

*   defined in: [Cluster library](cluster-defs-definitions-grant-object-properties-on.md "http://nethserver.org/json-schema/task/library/cluster#/definitions/grant-object/properties/on")

### on Type

`string`

### on Constraints

**minimum length**: the minimum number of characters for this string is: `1`
