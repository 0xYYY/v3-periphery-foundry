
# PathTest.sol

    

    
## Methods
### decodeFirstPool
```solidity
decodeFirstPool(bytes path) external pure returns (address tokenA, address tokenB, uint24 fee)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| path | bytes | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| tokenA | address | - |
| tokenB | address | - |
| fee | uint24 | - |

### getFirstPool
```solidity
getFirstPool(bytes path) external pure returns (bytes -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| path | bytes | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes | - |

### getGasCostOfDecodeFirstPool
```solidity
getGasCostOfDecodeFirstPool(bytes path) external view returns (uint256 -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| path | bytes | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### hasMultiplePools
```solidity
hasMultiplePools(bytes path) external pure returns (bool -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| path | bytes | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### skipToken
```solidity
skipToken(bytes path) external pure returns (bytes -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| path | bytes | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes | - |


