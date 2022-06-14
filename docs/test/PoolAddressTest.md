
# PoolAddressTest.sol

## Methods
### POOL_INIT_CODE_HASH
```solidity
POOL_INIT_CODE_HASH() external pure returns (bytes32)
```
#### Return Values

| Type | Description |
|---|---|
bytes32 | - |

### computeAddress
```solidity
computeAddress(address factory, address token0, address token1, uint24 fee) external pure returns (address)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| factory | address | - |
| token0 | address | - |
| token1 | address | - |
| fee | uint24 | - |

#### Return Values

| Type | Description |
|---|---|
address | - |

### getGasCostOfComputeAddress
```solidity
getGasCostOfComputeAddress(address factory, address token0, address token1, uint24 fee) external view returns (uint256)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| factory | address | - |
| token0 | address | - |
| token1 | address | - |
| fee | uint24 | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |


### Events

### Errors

