
# INonfungiblePositionManager.sol

    
Non-fungible token for positions

    
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
## Methods
### DOMAIN_SEPARATOR
```solidity
DOMAIN_SEPARATOR() external view returns (bytes32 -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### PERMIT_TYPEHASH
```solidity
PERMIT_TYPEHASH() external pure returns (bytes32 -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### WETH9
```solidity
WETH9() external view returns (address -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### approve
```solidity
approve(address to, uint256 tokenId) external nonpayable
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| to | address | - |
| tokenId | uint256 | - |

### balanceOf
```solidity
balanceOf(address owner) external view returns (uint256 balance)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| balance | uint256 | - |

### burn
```solidity
burn(uint256 tokenId) external payable
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | The ID of the token that is being burned |

### collect
```solidity
collect((uint256,address,uint128,uint128) params) external payable returns (uint256 amount0, uint256 amount1)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (uint256,address,uint128,uint128) | tokenId The ID of the NFT for which tokens are being collected, recipient The account that should receive the tokens, amount0Max The maximum amount of token0 to collect, amount1Max The maximum amount of token1 to collect |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amount0 | uint256 | The amount of fees collected in token0 |
| amount1 | uint256 | The amount of fees collected in token1 |

### createAndInitializePoolIfNecessary
```solidity
createAndInitializePoolIfNecessary(address token0, address token1, uint24 fee, uint160 sqrtPriceX96) external payable returns (address pool)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
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

### decreaseLiquidity
```solidity
decreaseLiquidity((uint256,uint128,uint256,uint256,uint256) params) external payable returns (uint256 amount0, uint256 amount1)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (uint256,uint128,uint256,uint256,uint256) | tokenId The ID of the token for which liquidity is being decreased, amount The amount by which liquidity will be decreased, amount0Min The minimum amount of token0 that should be accounted for the burned liquidity, amount1Min The minimum amount of token1 that should be accounted for the burned liquidity, deadline The time by which the transaction must be included to effect the change |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amount0 | uint256 | The amount of token0 accounted to the position's tokens owed |
| amount1 | uint256 | The amount of token1 accounted to the position's tokens owed |

### factory
```solidity
factory() external view returns (address -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### getApproved
```solidity
getApproved(uint256 tokenId) external view returns (address operator)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| operator | address | - |

### increaseLiquidity
```solidity
increaseLiquidity((uint256,uint256,uint256,uint256,uint256,uint256) params) external payable returns (uint128 liquidity, uint256 amount0, uint256 amount1)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (uint256,uint256,uint256,uint256,uint256,uint256) | tokenId The ID of the token for which liquidity is being increased, amount0Desired The desired amount of token0 to be spent, amount1Desired The desired amount of token1 to be spent, amount0Min The minimum amount of token0 to spend, which serves as a slippage check, amount1Min The minimum amount of token1 to spend, which serves as a slippage check, deadline The time by which the transaction must be included to effect the change |

#### Return Values

| Name | Type | Description |
|---|---|---|
| liquidity | uint128 | The new liquidity amount as a result of the increase |
| amount0 | uint256 | The amount of token0 to acheive resulting liquidity |
| amount1 | uint256 | The amount of token1 to acheive resulting liquidity |

### isApprovedForAll
```solidity
isApprovedForAll(address owner, address operator) external view returns (bool -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |
| operator | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### mint
```solidity
mint((address,address,uint24,int24,int24,uint256,uint256,uint256,uint256,address,uint256) params) external payable returns (uint256 tokenId, uint128 liquidity, uint256 amount0, uint256 amount1)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,int24,int24,uint256,uint256,uint256,uint256,address,uint256) | The params necessary to mint a position, encoded as `MintParams` in calldata |

#### Return Values

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | The ID of the token that represents the minted position |
| liquidity | uint128 | The amount of liquidity for this position |
| amount0 | uint256 | The amount of token0 |
| amount1 | uint256 | The amount of token1 |

### name
```solidity
name() external view returns (string -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### ownerOf
```solidity
ownerOf(uint256 tokenId) external view returns (address owner)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| owner | address | - |

### permit
```solidity
permit(address spender, uint256 tokenId, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| spender | address | The account that is being approved |
| tokenId | uint256 | The ID of the token that is being approved for spending |
| deadline | uint256 | The deadline timestamp by which the call must be mined for the approve to work |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### positions
```solidity
positions(uint256 tokenId) external view returns (uint96 nonce, address operator, address token0, address token1, uint24 fee, int24 tickLower, int24 tickUpper, uint128 liquidity, uint256 feeGrowthInside0LastX128, uint256 feeGrowthInside1LastX128, uint128 tokensOwed0, uint128 tokensOwed1)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | The ID of the token that represents the position |

#### Return Values

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

### refundETH
```solidity
refundETH() external payable
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
### safeTransferFrom
```solidity
safeTransferFrom(address from, address to, uint256 tokenId) external nonpayable
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |

```solidity
safeTransferFrom(address from, address to, uint256 tokenId, bytes data) external nonpayable
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |
| data | bytes | - |

### setApprovalForAll
```solidity
setApprovalForAll(address operator, bool _approved) external nonpayable
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| operator | address | - |
| _approved | bool | - |

### supportsInterface
```solidity
supportsInterface(bytes4 interfaceId) external view returns (bool -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| interfaceId | bytes4 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### sweepToken
```solidity
sweepToken(address token, uint256 amountMinimum, address recipient) external payable
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The contract address of the token which will be transferred to `recipient` |
| amountMinimum | uint256 | The minimum amount of token required for a transfer |
| recipient | address | The destination address of the token |

### symbol
```solidity
symbol() external view returns (string -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### tokenByIndex
```solidity
tokenByIndex(uint256 index) external view returns (uint256 -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| index | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### tokenOfOwnerByIndex
```solidity
tokenOfOwnerByIndex(address owner, uint256 index) external view returns (uint256 tokenId)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |
| index | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

### tokenURI
```solidity
tokenURI(uint256 tokenId) external view returns (string -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### totalSupply
```solidity
totalSupply() external view returns (uint256 -)
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### transferFrom
```solidity
transferFrom(address from, address to, uint256 tokenId) external nonpayable
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |

### unwrapWETH9
```solidity
unwrapWETH9(uint256 amountMinimum, address recipient) external payable
```

            

            
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |


