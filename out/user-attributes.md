# User attributes Schema

```txt
undefined#/properties/set
```

Display name and similar...

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                         |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [validate-input.json*](validate-input.json "open original schema") |

## set Type

`object` ([User attributes](user-attributes.md))

## set Examples

```json
{
  "display_name": "Mighty Admin"
}
```

# set Properties

| Property                      | Type     | Required | Nullable       | Defined by                                                                                         |
| :---------------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------- |
| [display_name](#display_name) | `string` | Optional | cannot be null | [User attributes](user-attributes-properties-display_name.md "undefined#/properties/display_name") |

## display_name



`display_name`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [User attributes](user-attributes-properties-display_name.md "undefined#/properties/display_name")

### display_name Type

`string`

### display_name Constraints

**minimum length**: the minimum number of characters for this string is: `1`
