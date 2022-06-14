
# IERC721Permit.sol
Title: ERC721 with permit
Notice: Extension to ERC721 that includes a permit function for signature based approvals

## Methods
```solidity
DOMAIN_SEPARATOR
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | bytes32 |  |

```solidity
PERMIT_TYPEHASH
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | bytes32 |  |

```solidity
approve
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| to | address |  |
| tokenId | uint256 |  |


### Return Values
```solidity
balanceOf
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| owner | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| balance | uint256 |  |

```solidity
getApproved
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| tokenId | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| operator | address |  |

```solidity
isApprovedForAll
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| owner | address |  |
| operator | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |

```solidity
ownerOf
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| tokenId | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| owner | address |  |

```solidity
permit
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| spender | address | The account that is being approved |
| tokenId | uint256 | The ID of the token that is being approved for spending |
| deadline | uint256 | The deadline timestamp by which the call must be mined for the approve to work |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
safeTransferFrom
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| from | address |  |
| to | address |  |
| tokenId | uint256 |  |


### Return Values
```solidity
safeTransferFrom
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| from | address |  |
| to | address |  |
| tokenId | uint256 |  |
| data | bytes |  |


### Return Values
```solidity
setApprovalForAll
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| operator | address |  |
| _approved | bool |  |


### Return Values
```solidity
supportsInterface
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| interfaceId | bytes4 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |

```solidity
transferFrom
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals

### Parameters
| Name | Type | Description |
|---|---|---|
| from | address |  |
| to | address |  |
| tokenId | uint256 |  |


### Return Values

### Events

### Errors

