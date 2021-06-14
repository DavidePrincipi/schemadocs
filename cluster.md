# Cluster library Schema

```txt
http://schema.nethserver.org/cluster.json
```

Cluster actions validation data formats

| Abstract               | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                          |
| :--------------------- | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------- |
| Cannot be instantiated | Yes        | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [cluster.json](cluster.json "open original schema") |

## Cluster library Type

unknown ([Cluster library](cluster.md))

# Cluster library Definitions

## Definitions group redis-pwh

Reference this group by using

```json
{"$ref":"http://schema.nethserver.org/cluster.json#/definitions/redis-pwh"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | :--- | :------- | :------- | :--------- |

## Definitions group user-attributes

Reference this group by using

```json
{"$ref":"http://schema.nethserver.org/cluster.json#/definitions/user-attributes"}
```

| Property                      | Type     | Required | Nullable       | Defined by                                                                                                                                                                         |
| :---------------------------- | :------- | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [display_name](#display_name) | `string` | Optional | cannot be null | [Cluster library](cluster-definitions-user-attributes-properties-display_name.md "http://schema.nethserver.org/cluster.json#/definitions/user-attributes/properties/display_name") |

### display_name



`display_name`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Cluster library](cluster-definitions-user-attributes-properties-display_name.md "http://schema.nethserver.org/cluster.json#/definitions/user-attributes/properties/display_name")

#### display_name Type

`string`

#### display_name Constraints

**minimum length**: the minimum number of characters for this string is: `1`

## Definitions group grant-object

Reference this group by using

```json
{"$ref":"http://schema.nethserver.org/cluster.json#/definitions/grant-object"}
```

| Property      | Type     | Required | Nullable       | Defined by                                                                                                                                                   |
| :------------ | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [role](#role) | `string` | Optional | cannot be null | [Cluster library](cluster-definitions-grant-object-properties-role.md "http://schema.nethserver.org/cluster.json#/definitions/grant-object/properties/role") |
| [on](#on)     | `string` | Optional | cannot be null | [Cluster library](cluster-definitions-grant-object-properties-on.md "http://schema.nethserver.org/cluster.json#/definitions/grant-object/properties/on")     |

### role



`role`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Cluster library](cluster-definitions-grant-object-properties-role.md "http://schema.nethserver.org/cluster.json#/definitions/grant-object/properties/role")

#### role Type

`string`

#### role Constraints

**minimum length**: the minimum number of characters for this string is: `1`

### on



`on`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Cluster library](cluster-definitions-grant-object-properties-on.md "http://schema.nethserver.org/cluster.json#/definitions/grant-object/properties/on")

#### on Type

`string`

#### on Constraints

**minimum length**: the minimum number of characters for this string is: `1`

## Definitions group strict-username-string

Reference this group by using

```json
{"$ref":"http://schema.nethserver.org/cluster.json#/definitions/strict-username-string"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | :--- | :------- | :------- | :--------- |
