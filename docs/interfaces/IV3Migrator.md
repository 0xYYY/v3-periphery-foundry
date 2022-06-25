
# IV3Migrator.sol

    
V3 Migrator

    
*Enables migration of liqudity from Uniswap v2-compatible pairs into Uniswap v3 pools*
## Methods
### createAndInitializePoolIfNecessary
```solidity
createAndInitializePoolIfNecessary(address token0, address token1, uint24 fee, uint160 sqrtPriceX96) external payable returns (address pool)
```

            
This method can be bundled with others via IMulticall for the first action (e.g. mint) performed against a pool

            
*Creates a new pool if it does not exist, then initializes if not initialized*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token0 | address | The contract address of token0 of the pool |
| token1 | address | The contract address of token1 of the pool |
| fee | uint24 | The fee amount of the v3 pool for the specified token pair |
| sqrtPriceX96 | uint160 | The initial square root price of the pool as a Q64.96 value |

#### Return Values

| Name | Type | Description |
|---|---|---|
| pool | address | Returns the pool address based on the pair of tokens and fee, will return the newly created pool address if necessary |

### migrate
```solidity
migrate((address,uint256,uint8,address,address,uint24,int24,int24,uint256,uint256,address,uint256,bool) params) external nonpayable
```

            
Slippage protection is enforced via `amount{0,1}Min`, which should be a discount of the expected values of the maximum amount of v3 liquidity that the v2 liquidity can get. For the special case of migrating to an out-of-range position, `amount{0,1}Min` may be set to 0, enforcing that the position remains out of range

            
*Migrates liquidity to v3 by burning v2 liquidity and minting a new position for v3*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (address,uint256,uint8,address,address,uint24,int24,int24,uint256,uint256,address,uint256,bool) | The params necessary to migrate v2 liquidity, encoded as `MigrateParams` in calldata |

### multicall
```solidity
multicall(bytes[] data) external payable returns (bytes[] results)
```

            
The `msg.value` should not be trusted for any method callable from multicall.

            
*Call multiple functions in the current contract and return the data from all of them if they all succeed*
#### Parameters

| Name | Type | Description |
|---|---|---|
| data | bytes[] | The encoded function data for each of the calls to make to this contract |

#### Return Values

| Name | Type | Description |
|---|---|---|
| results | bytes[] | The results from each of the calls passed in via data |

### selfPermit
```solidity
selfPermit(address token, uint256 value, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this).

            
*Permits this contract to spend a given token from `msg.sender`*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### selfPermitAllowed
```solidity
selfPermitAllowed(address token, uint256 nonce, uint256 expiry, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this)

            
*Permits this contract to spend the sender's tokens for permit signatures that have the `allowed` parameter*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### selfPermitAllowedIfNecessary
```solidity
selfPermitAllowedIfNecessary(address token, uint256 nonce, uint256 expiry, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this) Can be used instead of #selfPermitAllowed to prevent calls from failing due to a frontrun of a call to #selfPermitAllowed.

            
*Permits this contract to spend the sender's tokens for permit signatures that have the `allowed` parameter*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### selfPermitIfNecessary
```solidity
selfPermitIfNecessary(address token, uint256 value, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this). Can be used instead of #selfPermit to prevent calls from failing due to a frontrun of a call to #selfPermit

            
*Permits this contract to spend a given token from `msg.sender`*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


