
# `PoolAddressTest`

    

    
## Methods
### `POOL_INIT_CODE_HASH`
```solidity
function POOL_INIT_CODE_HASH() external pure returns (bytes32)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bytes32` | - |

### `computeAddress`
```solidity
function computeAddress(address factory, address token0, address token1, uint24 fee) external pure returns (address)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `factory` | `address` | - |
| `token0` | `address` | - |
| `token1` | `address` | - |
| `fee` | `uint24` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `getGasCostOfComputeAddress`
```solidity
function getGasCostOfComputeAddress(address factory, address token0, address token1, uint24 fee) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `factory` | `address` | - |
| `token0` | `address` | - |
| `token1` | `address` | - |
| `fee` | `uint24` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint256` | - |


