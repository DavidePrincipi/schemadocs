# Cluster library Schema

```txt
http://nethserver.org/json-schema/task/library/cluster
```

Cluster actions data format definition

| Abstract               | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                    |
| :--------------------- | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------ |
| Cannot be instantiated | Yes        | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [cluster-defs.json](cluster-defs.json "open original schema") |

## Cluster library Type

unknown ([Cluster library](cluster-defs.md))

# Cluster library Definitions

## Definitions group sha256-string

Reference this group by using

```json
{"$ref":"http://nethserver.org/json-schema/task/library/cluster#/definitions/sha256-string"}
```



## Definitions group user-attributes

Reference this group by using

```json
{"$ref":"http://nethserver.org/json-schema/task/library/cluster#/definitions/user-attributes"}
```



### display_name



`display_name`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Cluster library](cluster-defs-definitions-user-attributes-properties-display_name.md "http://nethserver.org/json-schema/task/library/cluster#/definitions/user-attributes/properties/display_name")

#### display_name Type

`string`

#### display_name Constraints

**minimum length**: the minimum number of characters for this string is: `1`

## Definitions group grant-object

Reference this group by using

```json
{"$ref":"http://nethserver.org/json-schema/task/library/cluster#/definitions/grant-object"}
```



### role



`role`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Cluster library](cluster-defs-definitions-grant-object-properties-role.md "http://nethserver.org/json-schema/task/library/cluster#/definitions/grant-object/properties/role")

#### role Type

`string`

#### role Constraints

**minimum length**: the minimum number of characters for this string is: `1`

### on



`on`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Cluster library](cluster-defs-definitions-grant-object-properties-on.md "http://nethserver.org/json-schema/task/library/cluster#/definitions/grant-object/properties/on")

#### on Type

`string`

#### on Constraints

**minimum length**: the minimum number of characters for this string is: `1`

## Definitions group strict-username-string

Reference this group by using

```json
{"$ref":"http://nethserver.org/json-schema/task/library/cluster#/definitions/strict-username-string"}
```

