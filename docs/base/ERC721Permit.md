
# ERC721Permit.sol
Title: ERC721 with permit
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

## Methods
```solidity
DOMAIN_SEPARATOR
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | bytes32 |  |

```solidity
PERMIT_TYPEHASH
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | bytes32 |  |

```solidity
approve
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| to | address |  |
| tokenId | uint256 |  |


### Return Values
```solidity
balanceOf
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| owner | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
baseURI
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
getApproved
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| tokenId | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
isApprovedForAll
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

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
name
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
ownerOf
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| tokenId | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
permit
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

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
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

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
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| from | address |  |
| to | address |  |
| tokenId | uint256 |  |
| _data | bytes |  |


### Return Values
```solidity
setApprovalForAll
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| operator | address |  |
| approved | bool |  |


### Return Values
```solidity
supportsInterface
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| interfaceId | bytes4 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |

```solidity
symbol
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
tokenByIndex
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| index | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
tokenOfOwnerByIndex
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| owner | address |  |
| index | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
tokenURI
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| tokenId | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
totalSupply
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
transferFrom
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

### Parameters
| Name | Type | Description |
|---|---|---|
| from | address |  |
| to | address |  |
| tokenId | uint256 |  |


### Return Values

### Events

### Errors

