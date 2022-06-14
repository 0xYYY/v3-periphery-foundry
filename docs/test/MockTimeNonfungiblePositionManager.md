
# MockTimeNonfungiblePositionManager.sol

## Methods
```solidity
DOMAIN_SEPARATOR
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | bytes32 |  |

```solidity
PERMIT_TYPEHASH
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | bytes32 |  |

```solidity
WETH9
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
approve
```

### Parameters
| Name | Type | Description |
|---|---|---|
| to | address |  |
| tokenId | uint256 |  |


### Return Values
```solidity
balanceOf
```

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

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
burn
```

### Parameters
| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | The ID of the token that is being burned |


### Return Values
```solidity
collect
```

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (uint256,address,uint128,uint128) | tokenId The ID of the NFT for which tokens are being collected, recipient The account that should receive the tokens, amount0Max The maximum amount of token0 to collect, amount1Max The maximum amount of token1 to collect |


### Return Values
| Name | Type | Description |
|---|---|---|
| amount0 | uint256 | The amount of fees collected in token0 |
| amount1 | uint256 | The amount of fees collected in token1 |

```solidity
createAndInitializePoolIfNecessary
```

### Parameters
| Name | Type | Description |
|---|---|---|
| token0 | address | The contract address of token0 of the pool |
| token1 | address | The contract address of token1 of the pool |
| fee | uint24 | The fee amount of the v3 pool for the specified token pair |
| sqrtPriceX96 | uint160 | The initial square root price of the pool as a Q64.96 value |


### Return Values
| Name | Type | Description |
|---|---|---|
| pool | address | Returns the pool address based on the pair of tokens and fee, will return the newly created pool address if necessary |

```solidity
decreaseLiquidity
```

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (uint256,uint128,uint256,uint256,uint256) | tokenId The ID of the token for which liquidity is being decreased, amount The amount by which liquidity will be decreased, amount0Min The minimum amount of token0 that should be accounted for the burned liquidity, amount1Min The minimum amount of token1 that should be accounted for the burned liquidity, deadline The time by which the transaction must be included to effect the change |


### Return Values
| Name | Type | Description |
|---|---|---|
| amount0 | uint256 | The amount of token0 accounted to the position's tokens owed |
| amount1 | uint256 | The amount of token1 accounted to the position's tokens owed |

```solidity
factory
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
getApproved
```

### Parameters
| Name | Type | Description |
|---|---|---|
| tokenId | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
increaseLiquidity
```

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (uint256,uint256,uint256,uint256,uint256,uint256) | tokenId The ID of the token for which liquidity is being increased, amount0Desired The desired amount of token0 to be spent, amount1Desired The desired amount of token1 to be spent, amount0Min The minimum amount of token0 to spend, which serves as a slippage check, amount1Min The minimum amount of token1 to spend, which serves as a slippage check, deadline The time by which the transaction must be included to effect the change |


### Return Values
| Name | Type | Description |
|---|---|---|
| liquidity | uint128 | The new liquidity amount as a result of the increase |
| amount0 | uint256 | The amount of token0 to acheive resulting liquidity |
| amount1 | uint256 | The amount of token1 to acheive resulting liquidity |

```solidity
isApprovedForAll
```

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
mint
```

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,int24,int24,uint256,uint256,uint256,uint256,address,uint256) | The params necessary to mint a position, encoded as `MintParams` in calldata |


### Return Values
| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | The ID of the token that represents the minted position |
| liquidity | uint128 | The amount of liquidity for this position |
| amount0 | uint256 | The amount of token0 |
| amount1 | uint256 | The amount of token1 |

```solidity
multicall
```

### Parameters
| Name | Type | Description |
|---|---|---|
| data | bytes[] | The encoded function data for each of the calls to make to this contract |


### Return Values
| Name | Type | Description |
|---|---|---|
| results | bytes[] | The results from each of the calls passed in via data |

```solidity
name
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
ownerOf
```

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
positions
```

### Parameters
| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | The ID of the token that represents the position |


### Return Values
| Name | Type | Description |
|---|---|---|
| nonce | uint96 | The nonce for permits |
| operator | address | The address that is approved for spending |
| token0 | address | The address of the token0 for a specific pool |
| token1 | address | The address of the token1 for a specific pool |
| fee | uint24 | The fee associated with the pool |
| tickLower | int24 | The lower end of the tick range for the position |
| tickUpper | int24 | The higher end of the tick range for the position |
| liquidity | uint128 | The liquidity of the position |
| feeGrowthInside0LastX128 | uint256 | The fee growth of token0 as of the last action on the individual position |
| feeGrowthInside1LastX128 | uint256 | The fee growth of token1 as of the last action on the individual position |
| tokensOwed0 | uint128 | The uncollected amount of token0 owed to the position as of the last computation |
| tokensOwed1 | uint128 | The uncollected amount of token1 owed to the position as of the last computation |

```solidity
refundETH
```

### Parameters

### Return Values
```solidity
safeTransferFrom
```

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

### Parameters
| Name | Type | Description |
|---|---|---|
| from | address |  |
| to | address |  |
| tokenId | uint256 |  |
| _data | bytes |  |


### Return Values
```solidity
selfPermit
```

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
selfPermitAllowed
```

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
selfPermitAllowedIfNecessary
```

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
selfPermitIfNecessary
```

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
setApprovalForAll
```

### Parameters
| Name | Type | Description |
|---|---|---|
| operator | address |  |
| approved | bool |  |


### Return Values
```solidity
setTime
```

### Parameters
| Name | Type | Description |
|---|---|---|
| _time | uint256 |  |


### Return Values
```solidity
supportsInterface
```

### Parameters
| Name | Type | Description |
|---|---|---|
| interfaceId | bytes4 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |

```solidity
sweepToken
```

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The contract address of the token which will be transferred to `recipient` |
| amountMinimum | uint256 | The minimum amount of token required for a transfer |
| recipient | address | The destination address of the token |


### Return Values
```solidity
symbol
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
tokenByIndex
```

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

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
transferFrom
```

### Parameters
| Name | Type | Description |
|---|---|---|
| from | address |  |
| to | address |  |
| tokenId | uint256 |  |


### Return Values
```solidity
uniswapV3MintCallback
```

### Parameters
| Name | Type | Description |
|---|---|---|
| amount0Owed | uint256 | The amount of token0 due to the pool for the minted liquidity |
| amount1Owed | uint256 | The amount of token1 due to the pool for the minted liquidity |
| data | bytes | Any data passed through by the caller via the IUniswapV3PoolActions#mint call |


### Return Values
```solidity
unwrapWETH9
```

### Parameters
| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |


### Return Values

### Events

### Errors

