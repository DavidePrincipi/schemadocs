# add-node output Schema

```txt
http://schema.nethserver.org/cluster/add-node-output.json
```

Output schema of the add-node action

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                  |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [add-node-output.json](cluster/add-node-output.json "open original schema") |

## add-node output Type

`object` ([add-node output](add-node-output.md))

## add-node output Examples

```json
{}
```

# add-node output Properties

| Property                                | Type      | Required | Nullable       | Defined by                                                                                                                                                   |
| :-------------------------------------- | :-------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [node_id](#node_id)                     | `integer` | Required | cannot be null | [add-node output](add-node-output-properties-node_id.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/node_id")                     |
| [ip_address](#ip_address)               | `string`  | Required | cannot be null | [add-node output](add-node-output-properties-ip_address.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/ip_address")               |
| [network](#network)                     | `string`  | Required | cannot be null | [add-node output](add-node-output-properties-network.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/network")                     |
| [leader_public_key](#leader_public_key) | `string`  | Required | cannot be null | [add-node output](add-node-output-properties-leader_public_key.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/leader_public_key") |
| [leader_ip_address](#leader_ip_address) | `string`  | Required | cannot be null | [add-node output](add-node-output-properties-leader_ip_address.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/leader_ip_address") |
| [leader_endpoint](#leader_endpoint)     | `string`  | Required | cannot be null | [add-node output](add-node-output-properties-leader_endpoint.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/leader_endpoint")     |

## node_id

Node identifier

`node_id`

*   is required

*   Type: `integer`

*   cannot be null

*   defined in: [add-node output](add-node-output-properties-node_id.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/node_id")

### node_id Type

`integer`

### node_id Constraints

**minimum**: the value of this number must greater than or equal to: `1`

## ip_address

VPN IP address of the added node

`ip_address`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [add-node output](add-node-output-properties-ip_address.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/ip_address")

### ip_address Type

`string`

### ip_address Constraints

**IPv4**: the string must be an IPv4 address (dotted quad), according to [RFC 2673, section 3.2](https://tools.ietf.org/html/rfc2673 "check the specification")

## network

The VPN network CIDR used by the cluster

`network`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [add-node output](add-node-output-properties-network.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/network")

### network Type

`string`

### network Constraints

**IPv4**: the string must be an IPv4 address (dotted quad), according to [RFC 2673, section 3.2](https://tools.ietf.org/html/rfc2673 "check the specification")

## leader_public_key

WireGuard public key of the leader node

`leader_public_key`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [add-node output](add-node-output-properties-leader_public_key.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/leader_public_key")

### leader_public_key Type

`string`

## leader_ip_address

VPN IP address of the leader node

`leader_ip_address`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [add-node output](add-node-output-properties-leader_ip_address.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/leader_ip_address")

### leader_ip_address Type

`string`

### leader_ip_address Constraints

**IPv4**: the string must be an IPv4 address (dotted quad), according to [RFC 2673, section 3.2](https://tools.ietf.org/html/rfc2673 "check the specification")

## leader_endpoint

WireGuard endpoint address to contact the leader node

`leader_endpoint`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [add-node output](add-node-output-properties-leader_endpoint.md "http://schema.nethserver.org/cluster/add-node-output.json#/properties/leader_endpoint")

### leader_endpoint Type

`string`
