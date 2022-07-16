
# `MockTimeNonfungiblePositionManager`

    

    
## Methods
### `DOMAIN_SEPARATOR`
```solidity
function DOMAIN_SEPARATOR() external view returns (bytes32)
```

            

            
*The domain separator used in the permit signature*
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bytes32` | - |

### `PERMIT_TYPEHASH`
```solidity
function PERMIT_TYPEHASH() external view returns (bytes32)
```

            

            
*The permit typehash used in the permit signature*
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bytes32` | - |

### `WETH9`
```solidity
function WETH9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `approve`
```solidity
function approve(address to, uint256 tokenId) external nonpayable
```

            
See {IERC721-approve}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `to` | `address` | - |
| `tokenId` | `uint256` | - |

### `balanceOf`
```solidity
function balanceOf(address owner) external view returns (uint256)
```

            
See {IERC721-balanceOf}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `owner` | `address` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint256` | - |

### `baseURI`
```solidity
function baseURI() external pure returns (string)
```

            
Returns the base URI set via {_setBaseURI}. This will be automatically added as a prefix in {tokenURI} to each token's URI, or to the token ID if no specific URI is set for that token ID.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `string` | - |

### `burn`
```solidity
function burn(uint256 tokenId) external payable
```

            

            
*Burns a token ID, which deletes it from the NFT contract. The token must have 0 liquidity and all tokens must be collected first.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokenId` | `uint256` | The ID of the token that is being burned |

### `collect`
```solidity
function collect((uint256,address,uint128,uint128) params) external payable returns (uint256 amount0, uint256 amount1)
```

            

            
*Collects up to a maximum amount of fees owed to a specific position to the recipient*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `params` | `(uint256,address,uint128,uint128)` | tokenId The ID of the NFT for which tokens are being collected, recipient The account that should receive the tokens, amount0Max The maximum amount of token0 to collect, amount1Max The maximum amount of token1 to collect |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `amount0` | `uint256` | The amount of fees collected in token0 |
| `amount1` | `uint256` | The amount of fees collected in token1 |

### `createAndInitializePoolIfNecessary`
```solidity
function createAndInitializePoolIfNecessary(address token0, address token1, uint24 fee, uint160 sqrtPriceX96) external payable returns (address pool)
```

            
This method can be bundled with others via IMulticall for the first action (e.g. mint) performed against a pool

            
*Creates a new pool if it does not exist, then initializes if not initialized*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `token0` | `address` | The contract address of token0 of the pool |
| `token1` | `address` | The contract address of token1 of the pool |
| `fee` | `uint24` | The fee amount of the v3 pool for the specified token pair |
| `sqrtPriceX96` | `uint160` | The initial square root price of the pool as a Q64.96 value |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `pool` | `address` | Returns the pool address based on the pair of tokens and fee, will return the newly created pool address if necessary |

### `decreaseLiquidity`
```solidity
function decreaseLiquidity((uint256,uint128,uint256,uint256,uint256) params) external payable returns (uint256 amount0, uint256 amount1)
```

            

            
*Decreases the amount of liquidity in a position and accounts it to the position*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `params` | `(uint256,uint128,uint256,uint256,uint256)` | tokenId The ID of the token for which liquidity is being decreased, amount The amount by which liquidity will be decreased, amount0Min The minimum amount of token0 that should be accounted for the burned liquidity, amount1Min The minimum amount of token1 that should be accounted for the burned liquidity, deadline The time by which the transaction must be included to effect the change |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `amount0` | `uint256` | The amount of token0 accounted to the position's tokens owed |
| `amount1` | `uint256` | The amount of token1 accounted to the position's tokens owed |

### `factory`
```solidity
function factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `getApproved`
```solidity
function getApproved(uint256 tokenId) external view returns (address)
```

            
Returns the account approved for `tokenId` token. Requirements: - `tokenId` must exist.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokenId` | `uint256` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `increaseLiquidity`
```solidity
function increaseLiquidity((uint256,uint256,uint256,uint256,uint256,uint256) params) external payable returns (uint128 liquidity, uint256 amount0, uint256 amount1)
```

            

            
*Increases the amount of liquidity in a position, with tokens paid by the `msg.sender`*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `params` | `(uint256,uint256,uint256,uint256,uint256,uint256)` | tokenId The ID of the token for which liquidity is being increased, amount0Desired The desired amount of token0 to be spent, amount1Desired The desired amount of token1 to be spent, amount0Min The minimum amount of token0 to spend, which serves as a slippage check, amount1Min The minimum amount of token1 to spend, which serves as a slippage check, deadline The time by which the transaction must be included to effect the change |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `liquidity` | `uint128` | The new liquidity amount as a result of the increase |
| `amount0` | `uint256` | The amount of token0 to acheive resulting liquidity |
| `amount1` | `uint256` | The amount of token1 to acheive resulting liquidity |

### `isApprovedForAll`
```solidity
function isApprovedForAll(address owner, address operator) external view returns (bool)
```

            
See {IERC721-isApprovedForAll}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `owner` | `address` | - |
| `operator` | `address` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bool` | - |

### `mint`
```solidity
function mint((address,address,uint24,int24,int24,uint256,uint256,uint256,uint256,address,uint256) params) external payable returns (uint256 tokenId, uint128 liquidity, uint256 amount0, uint256 amount1)
```

            
Call this when the pool does exist and is initialized. Note that if the pool is created but not initialized a method does not exist, i.e. the pool is assumed to be initialized.

            
*Creates a new position wrapped in a NFT*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `params` | `(address,address,uint24,int24,int24,uint256,uint256,uint256,uint256,address,uint256)` | The params necessary to mint a position, encoded as `MintParams` in calldata |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `tokenId` | `uint256` | The ID of the token that represents the minted position |
| `liquidity` | `uint128` | The amount of liquidity for this position |
| `amount0` | `uint256` | The amount of token0 |
| `amount1` | `uint256` | The amount of token1 |

### `multicall`
```solidity
function multicall(bytes[] data) external payable returns (bytes[] results)
```

            
The `msg.value` should not be trusted for any method callable from multicall.

            
*Call multiple functions in the current contract and return the data from all of them if they all succeed*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `data` | `bytes[]` | The encoded function data for each of the calls to make to this contract |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `results` | `bytes[]` | The results from each of the calls passed in via data |

### `name`
```solidity
function name() external view returns (string)
```

            
See {IERC721Metadata-name}.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `string` | - |

### `ownerOf`
```solidity
function ownerOf(uint256 tokenId) external view returns (address)
```

            
See {IERC721-ownerOf}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokenId` | `uint256` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `permit`
```solidity
function permit(address spender, uint256 tokenId, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            

            
*Approve of a specific token ID for spending by spender via signature*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `spender` | `address` | The account that is being approved |
| `tokenId` | `uint256` | The ID of the token that is being approved for spending |
| `deadline` | `uint256` | The deadline timestamp by which the call must be mined for the approve to work |
| `v` | `uint8` | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| `r` | `bytes32` | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| `s` | `bytes32` | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### `positions`
```solidity
function positions(uint256 tokenId) external view returns (uint96 nonce, address operator, address token0, address token1, uint24 fee, int24 tickLower, int24 tickUpper, uint128 liquidity, uint256 feeGrowthInside0LastX128, uint256 feeGrowthInside1LastX128, uint128 tokensOwed0, uint128 tokensOwed1)
```

            
Throws if the token ID is not valid.

            
*Returns the position information associated with a given token ID.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokenId` | `uint256` | The ID of the token that represents the position |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `nonce` | `uint96` | The nonce for permits |
| `operator` | `address` | The address that is approved for spending |
| `token0` | `address` | The address of the token0 for a specific pool |
| `token1` | `address` | The address of the token1 for a specific pool |
| `fee` | `uint24` | The fee associated with the pool |
| `tickLower` | `int24` | The lower end of the tick range for the position |
| `tickUpper` | `int24` | The higher end of the tick range for the position |
| `liquidity` | `uint128` | The liquidity of the position |
| `feeGrowthInside0LastX128` | `uint256` | The fee growth of token0 as of the last action on the individual position |
| `feeGrowthInside1LastX128` | `uint256` | The fee growth of token1 as of the last action on the individual position |
| `tokensOwed0` | `uint128` | The uncollected amount of token0 owed to the position as of the last computation |
| `tokensOwed1` | `uint128` | The uncollected amount of token1 owed to the position as of the last computation |

### `refundETH`
```solidity
function refundETH() external payable
```

            
Useful for bundling with mint or increase liquidity that uses ether, or exact output swaps that use ether for the input amount

            
*Refunds any ETH balance held by this contract to the `msg.sender`*
### `safeTransferFrom`
```solidity
function safeTransferFrom(address from, address to, uint256 tokenId) external nonpayable
```

            
See {IERC721-safeTransferFrom}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `from` | `address` | - |
| `to` | `address` | - |
| `tokenId` | `uint256` | - |

```solidity
function safeTransferFrom(address from, address to, uint256 tokenId, bytes _data) external nonpayable
```

            
See {IERC721-safeTransferFrom}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `from` | `address` | - |
| `to` | `address` | - |
| `tokenId` | `uint256` | - |
| `_data` | `bytes` | - |

### `selfPermit`
```solidity
function selfPermit(address token, uint256 value, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this).

            
*Permits this contract to spend a given token from `msg.sender`*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `token` | `address` | The address of the token spent |
| `value` | `uint256` | The amount that can be spent of token |
| `deadline` | `uint256` | A timestamp, the current blocktime must be less than or equal to this timestamp |
| `v` | `uint8` | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| `r` | `bytes32` | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| `s` | `bytes32` | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### `selfPermitAllowed`
```solidity
function selfPermitAllowed(address token, uint256 nonce, uint256 expiry, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this)

            
*Permits this contract to spend the sender's tokens for permit signatures that have the `allowed` parameter*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `token` | `address` | The address of the token spent |
| `nonce` | `uint256` | The current nonce of the owner |
| `expiry` | `uint256` | The timestamp at which the permit is no longer valid |
| `v` | `uint8` | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| `r` | `bytes32` | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| `s` | `bytes32` | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### `selfPermitAllowedIfNecessary`
```solidity
function selfPermitAllowedIfNecessary(address token, uint256 nonce, uint256 expiry, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this) Can be used instead of #selfPermitAllowed to prevent calls from failing due to a frontrun of a call to #selfPermitAllowed.

            
*Permits this contract to spend the sender's tokens for permit signatures that have the `allowed` parameter*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `token` | `address` | The address of the token spent |
| `nonce` | `uint256` | The current nonce of the owner |
| `expiry` | `uint256` | The timestamp at which the permit is no longer valid |
| `v` | `uint8` | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| `r` | `bytes32` | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| `s` | `bytes32` | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### `selfPermitIfNecessary`
```solidity
function selfPermitIfNecessary(address token, uint256 value, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this). Can be used instead of #selfPermit to prevent calls from failing due to a frontrun of a call to #selfPermit

            
*Permits this contract to spend a given token from `msg.sender`*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `token` | `address` | The address of the token spent |
| `value` | `uint256` | The amount that can be spent of token |
| `deadline` | `uint256` | A timestamp, the current blocktime must be less than or equal to this timestamp |
| `v` | `uint8` | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| `r` | `bytes32` | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| `s` | `bytes32` | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### `setApprovalForAll`
```solidity
function setApprovalForAll(address operator, bool approved) external nonpayable
```

            
See {IERC721-setApprovalForAll}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `operator` | `address` | - |
| `approved` | `bool` | - |

### `setTime`
```solidity
function setTime(uint256 _time) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `_time` | `uint256` | - |

### `supportsInterface`
```solidity
function supportsInterface(bytes4 interfaceId) external view returns (bool)
```

            
See {IERC165-supportsInterface}. Time complexity O(1), guaranteed to always use less than 30 000 gas.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `interfaceId` | `bytes4` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bool` | - |

### `sweepToken`
```solidity
function sweepToken(address token, uint256 amountMinimum, address recipient) external payable
```

            
The amountMinimum parameter prevents malicious contracts from stealing the token from users

            
*Transfers the full amount of a token held by this contract to recipient*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `token` | `address` | The contract address of the token which will be transferred to `recipient` |
| `amountMinimum` | `uint256` | The minimum amount of token required for a transfer |
| `recipient` | `address` | The destination address of the token |

### `symbol`
```solidity
function symbol() external view returns (string)
```

            
See {IERC721Metadata-symbol}.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `string` | - |

### `tokenByIndex`
```solidity
function tokenByIndex(uint256 index) external view returns (uint256)
```

            
See {IERC721Enumerable-tokenByIndex}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `index` | `uint256` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint256` | - |

### `tokenOfOwnerByIndex`
```solidity
function tokenOfOwnerByIndex(address owner, uint256 index) external view returns (uint256)
```

            
See {IERC721Enumerable-tokenOfOwnerByIndex}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `owner` | `address` | - |
| `index` | `uint256` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint256` | - |

### `tokenURI`
```solidity
function tokenURI(uint256 tokenId) external view returns (string)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokenId` | `uint256` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `string` | - |

### `totalSupply`
```solidity
function totalSupply() external view returns (uint256)
```

            
See {IERC721Enumerable-totalSupply}.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint256` | - |

### `transferFrom`
```solidity
function transferFrom(address from, address to, uint256 tokenId) external nonpayable
```

            
See {IERC721-transferFrom}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `from` | `address` | - |
| `to` | `address` | - |
| `tokenId` | `uint256` | - |

### `uniswapV3MintCallback`
```solidity
function uniswapV3MintCallback(uint256 amount0Owed, uint256 amount1Owed, bytes data) external nonpayable
```

            
In the implementation you must pay the pool tokens owed for the minted liquidity. The caller of this method must be checked to be a UniswapV3Pool deployed by the canonical UniswapV3Factory.

            
*Called to `msg.sender` after minting liquidity to a position from IUniswapV3Pool#mint.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `amount0Owed` | `uint256` | The amount of token0 due to the pool for the minted liquidity |
| `amount1Owed` | `uint256` | The amount of token1 due to the pool for the minted liquidity |
| `data` | `bytes` | Any data passed through by the caller via the IUniswapV3PoolActions#mint call |

### `unwrapWETH9`
```solidity
function unwrapWETH9(uint256 amountMinimum, address recipient) external payable
```

            
The amountMinimum parameter prevents malicious contracts from stealing WETH9 from users.

            
*Unwraps the contract's WETH9 balance and sends it to recipient as ETH.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `amountMinimum` | `uint256` | The minimum amount of WETH9 to unwrap |
| `recipient` | `address` | The address receiving ETH |

### Events
### `Approval`
```solidity
event Approval(address owner, address approved, uint256 tokenId)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| `owner` | `address` |`true`| - |
| `approved` | `address` |`true`| - |
| `tokenId` | `uint256` |`true`| - |

### `ApprovalForAll`
```solidity
event ApprovalForAll(address owner, address operator, bool approved)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| `owner` | `address` |`true`| - |
| `operator` | `address` |`true`| - |
| `approved` | `bool` |`false`| - |

### `Collect`
```solidity
event Collect(uint256 tokenId, address recipient, uint256 amount0, uint256 amount1)
```

            

            
*Emitted when tokens are collected for a position NFT*
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| `tokenId` | `uint256` |`true`| - |
| `recipient` | `address` |`false`| - |
| `amount0` | `uint256` |`false`| - |
| `amount1` | `uint256` |`false`| - |

### `DecreaseLiquidity`
```solidity
event DecreaseLiquidity(uint256 tokenId, uint128 liquidity, uint256 amount0, uint256 amount1)
```

            

            
*Emitted when liquidity is decreased for a position NFT*
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| `tokenId` | `uint256` |`true`| - |
| `liquidity` | `uint128` |`false`| - |
| `amount0` | `uint256` |`false`| - |
| `amount1` | `uint256` |`false`| - |

### `IncreaseLiquidity`
```solidity
event IncreaseLiquidity(uint256 tokenId, uint128 liquidity, uint256 amount0, uint256 amount1)
```

            

            
*Emitted when liquidity is increased for a position NFT*
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| `tokenId` | `uint256` |`true`| - |
| `liquidity` | `uint128` |`false`| - |
| `amount0` | `uint256` |`false`| - |
| `amount1` | `uint256` |`false`| - |

### `Transfer`
```solidity
event Transfer(address from, address to, uint256 tokenId)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| `from` | `address` |`true`| - |
| `to` | `address` |`true`| - |
| `tokenId` | `uint256` |`true`| - |


