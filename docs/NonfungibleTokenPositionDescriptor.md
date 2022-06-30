
# NonfungibleTokenPositionDescriptor.sol

    
Describes NFT token positions

    
*Produces a string containing the data URI for a JSON metadata string*
## Methods
### WETH9
```solidity
function WETH9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### flipRatio
```solidity
function flipRatio(address token0, address token1, uint256 chainId) external view returns (bool)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| token0 | address | - |
| token1 | address | - |
| chainId | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### nativeCurrencyLabel
```solidity
function nativeCurrencyLabel() external view returns (string)
```

            

            
*Returns the native currency label as a string*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### nativeCurrencyLabelBytes
```solidity
function nativeCurrencyLabelBytes() external view returns (bytes32)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### tokenRatioPriority
```solidity
function tokenRatioPriority(address token, uint256 chainId) external view returns (int256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | - |
| chainId | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | int256 | - |

### tokenURI
```solidity
function tokenURI(address positionManager, uint256 tokenId) external view returns (string)
```

            
Note this URI may be a data: URI with the JSON contents directly inlined

            
*Produces the URI describing a particular token ID for a position manager*
#### Parameters

| Name | Type | Description |
|---|---|---|
| positionManager | address | The position manager for which to describe the token |
| tokenId | uint256 | The ID of the token for which to produce a description, which may not be valid |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |


