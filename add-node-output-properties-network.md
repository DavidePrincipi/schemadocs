# Untitled string in add-node output Schema

```txt
http://schema.nethserver.org/cluster/add-node-output.json#/properties/network
```

The VPN network CIDR used by the cluster

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                   |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :--------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [add-node-output.json*](cluster/add-node-output.json "open original schema") |

## network Type

`string`

## network Constraints

**IPv4**: the string must be an IPv4 address (dotted quad), according to [RFC 2673, section 3.2](https://tools.ietf.org/html/rfc2673 "check the specification")
