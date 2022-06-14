
# NonfungibleTokenPositionDescriptor.sol
Title: Describes NFT token positions
Notice: Produces a string containing the data URI for a JSON metadata string

## Methods
```solidity
WETH9
```
Notice: Produces a string containing the data URI for a JSON metadata string

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
flipRatio
```
Notice: Produces a string containing the data URI for a JSON metadata string

### Parameters
| Name | Type | Description |
|---|---|---|
| token0 | address |  |
| token1 | address |  |
| chainId | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |

```solidity
nativeCurrencyLabel
```
Notice: Produces a string containing the data URI for a JSON metadata string

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
nativeCurrencyLabelBytes
```
Notice: Produces a string containing the data URI for a JSON metadata string

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | bytes32 |  |

```solidity
tokenRatioPriority
```
Notice: Produces a string containing the data URI for a JSON metadata string

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address |  |
| chainId | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | int256 |  |

```solidity
tokenURI
```
Notice: Produces a string containing the data URI for a JSON metadata string

### Parameters
| Name | Type | Description |
|---|---|---|
| positionManager | address | The position manager for which to describe the token |
| tokenId | uint256 | The ID of the token for which to produce a description, which may not be valid |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |


### Events

### Errors

