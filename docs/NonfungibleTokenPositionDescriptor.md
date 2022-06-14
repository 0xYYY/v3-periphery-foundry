
# NonfungibleTokenPositionDescriptor.sol

    
Describes NFT token positions

    
*Produces a string containing the data URI for a JSON metadata string*
## Methods
### WETH9
```solidity
WETH9() external view returns (address -)
```

            

            
*Produces a string containing the data URI for a JSON metadata string*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### flipRatio
```solidity
flipRatio(address token0, address token1, uint256 chainId) external view returns (bool -)
```

            

            
*Produces a string containing the data URI for a JSON metadata string*
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
nativeCurrencyLabel() external view returns (string -)
```

            

            
*Produces a string containing the data URI for a JSON metadata string*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### nativeCurrencyLabelBytes
```solidity
nativeCurrencyLabelBytes() external view returns (bytes32 -)
```

            

            
*Produces a string containing the data URI for a JSON metadata string*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### tokenRatioPriority
```solidity
tokenRatioPriority(address token, uint256 chainId) external view returns (int256 -)
```

            

            
*Produces a string containing the data URI for a JSON metadata string*
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
tokenURI(address positionManager, uint256 tokenId) external view returns (string -)
```

            

            
*Produces a string containing the data URI for a JSON metadata string*
#### Parameters

| Name | Type | Description |
|---|---|---|
| positionManager | address | The position manager for which to describe the token |
| tokenId | uint256 | The ID of the token for which to produce a description, which may not be valid |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |


