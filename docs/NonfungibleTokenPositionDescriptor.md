
# NonfungibleTokenPositionDescriptor.sol
Title: Describes NFT token positions
Notice: Produces a string containing the data URI for a JSON metadata string

## Methods
### WETH9
```solidity
WETH9() external view returns (address)
```
Notice: Produces a string containing the data URI for a JSON metadata string
#### Return Values

| Type | Description |
|---|---|
address | - |

### flipRatio
```solidity
flipRatio(address token0, address token1, uint256 chainId) external view returns (bool)
```
Notice: Produces a string containing the data URI for a JSON metadata string
#### Parameters

| Name | Type | Description |
|---|---|---|
| token0 | address | - |
| token1 | address | - |
| chainId | uint256 | - |

#### Return Values

| Type | Description |
|---|---|
bool | - |

### nativeCurrencyLabel
```solidity
nativeCurrencyLabel() external view returns (string)
```
Notice: Produces a string containing the data URI for a JSON metadata string
#### Return Values

| Type | Description |
|---|---|
string | - |

### nativeCurrencyLabelBytes
```solidity
nativeCurrencyLabelBytes() external view returns (bytes32)
```
Notice: Produces a string containing the data URI for a JSON metadata string
#### Return Values

| Type | Description |
|---|---|
bytes32 | - |

### tokenRatioPriority
```solidity
tokenRatioPriority(address token, uint256 chainId) external view returns (int256)
```
Notice: Produces a string containing the data URI for a JSON metadata string
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | - |
| chainId | uint256 | - |

#### Return Values

| Type | Description |
|---|---|
int256 | - |

### tokenURI
```solidity
tokenURI(address positionManager, uint256 tokenId) external view returns (string)
```
Notice: Produces a string containing the data URI for a JSON metadata string
#### Parameters

| Name | Type | Description |
|---|---|---|
| positionManager | address | The position manager for which to describe the token |
| tokenId | uint256 | The ID of the token for which to produce a description, which may not be valid |

#### Return Values

| Type | Description |
|---|---|
string | - |


### Events

### Errors

