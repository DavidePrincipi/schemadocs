# README

## Top-level Schemas

*   [Grant object structure](./user-grants.md "A grant object establishes a relation between a role and the cluster objects matching the \"on\" clause") – `-`

*   [SHA256 string format](./sha256-string.md "A SHA256 string is 64 hexadecimal numbers long") – `-`

*   [Strict username validation schema](./username-strict.md "See https://www") – `-`

*   [User attributes](./user-attributes.md "Display name and similar") – `-`

*   [add-user input](./validate-input.md "Create a user account for the cluster administration web interface") – `-`

*   [add-user output](./validate-output.md "Output schema of the add-user action") – `-`

## Other Schemas

### Objects

*   [Grant object structure](./validate-input-properties-grant-grant-object-structure.md "A grant object establishes a relation between a role and the cluster objects matching the \"on\" clause") – `undefined#/properties/grant/items`

*   [User attributes](./validate-input-properties-user-attributes.md "Display name and similar") – `undefined#/properties/set`

### Arrays

*   [Untitled array in add-user input](./validate-input-properties-grant.md "A list of initial roles on the matching cluster objects") – `undefined#/properties/grant`

## Version Note

The schemas linked above follow the JSON Schema Spec version: `http://json-schema.org/draft-07/schema#`
