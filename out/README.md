# README

## Top-level Schemas

*   [Add-user (input)](./validate-input.md "Create a user account for the cluster administration web interface") – `http://nethserver.org/json-schema/task/input/cluster/add-user`

*   [Add-user (output)](./validate-output.md "Output schema of the add-user action") – `http://nethserver.org/json-schema/task/output/cluster/add-user`

*   [Cluster library](./cluster-defs.md "Cluster actions data format definition") – `http://nethserver.org/json-schema/task/library/cluster`

## Other Schemas

### Objects

*   [Grant object](./cluster-defs-definitions-grant-object.md "A grant object establishes a relation between a role and the cluster objects matching the \"on\" clause") – `http://nethserver.org/json-schema/task/library/cluster#/definitions/grant-object`

*   [Grant object](./validate-input-properties-grant-assertions-list-grant-object.md "A grant object establishes a relation between a role and the cluster objects matching the \"on\" clause") – `http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/grant/items`

*   [User attributes](./cluster-defs-definitions-user-attributes.md "Attributes of a User") – `http://nethserver.org/json-schema/task/library/cluster#/definitions/user-attributes`

*   [User attributes](./validate-input-properties-user-attributes.md "Attributes of a User") – `http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/set`

### Arrays

*   [Grant assertions list](./validate-input-properties-grant-assertions-list.md "A list of initial roles on the matching cluster objects") – `http://nethserver.org/json-schema/task/input/cluster/add-user#/properties/grant`

## Version Note

The schemas linked above follow the JSON Schema Spec version: `http://json-schema.org/draft-07/schema#`
