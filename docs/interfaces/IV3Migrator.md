
# IV3Migrator.sol

    
V3 Migrator

    
*Enables migration of liqudity from Uniswap v2-compatible pairs into Uniswap v3 pools*
## Methods
### createAndInitializePoolIfNecessary
```solidity
createAndInitializePoolIfNecessary(address token0, address token1, uint24 fee, uint160 sqrtPriceX96) external payable returns (address pool)
```

            

            
*Enables migration of liqudity from Uniswap v2-compatible pairs into Uniswap v3 pools*
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

            

            
*Enables migration of liqudity from Uniswap v2-compatible pairs into Uniswap v3 pools*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (address,uint256,uint8,address,address,uint24,int24,int24,uint256,uint256,address,uint256,bool) | The params necessary to migrate v2 liquidity, encoded as `MigrateParams` in calldata |

### multicall
```solidity
multicall(bytes[] data) external payable returns (bytes[] results)
```

            

            
*Enables migration of liqudity from Uniswap v2-compatible pairs into Uniswap v3 pools*
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

            

            
*Enables migration of liqudity from Uniswap v2-compatible pairs into Uniswap v3 pools*
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

            

            
*Enables migration of liqudity from Uniswap v2-compatible pairs into Uniswap v3 pools*
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

            

            
*Enables migration of liqudity from Uniswap v2-compatible pairs into Uniswap v3 pools*
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

            

            
*Enables migration of liqudity from Uniswap v2-compatible pairs into Uniswap v3 pools*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


