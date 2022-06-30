
# INonfungiblePositionManager.sol

    
Non-fungible token for positions

    
*Wraps Uniswap V3 positions in a non-fungible token interface which allows for them to be transferred and authorized.*
## Methods
### DOMAIN_SEPARATOR
```solidity
function DOMAIN_SEPARATOR() external view returns (bytes32)
```

            

            
*The domain separator used in the permit signature*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### PERMIT_TYPEHASH
```solidity
function PERMIT_TYPEHASH() external pure returns (bytes32)
```

            

            
*The permit typehash used in the permit signature*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### WETH9
```solidity
function WETH9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### approve
```solidity
function approve(address to, uint256 tokenId) external nonpayable
```

            
Gives permission to `to` to transfer `tokenId` token to another account. The approval is cleared when the token is transferred. Only a single account can be approved at a time, so approving the zero address clears previous approvals. Requirements: - The caller must own the token or be an approved operator. - `tokenId` must exist. Emits an {Approval} event.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| to | address | - |
| tokenId | uint256 | - |

### balanceOf
```solidity
function balanceOf(address owner) external view returns (uint256 balance)
```

            
Returns the number of tokens in ``owner``'s account.

            
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
function burn(uint256 tokenId) external payable
```

            

            
*Burns a token ID, which deletes it from the NFT contract. The token must have 0 liquidity and all tokens must be collected first.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | The ID of the token that is being burned |

### collect
```solidity
function collect((uint256,address,uint128,uint128) params) external payable returns (uint256 amount0, uint256 amount1)
```

            

            
*Collects up to a maximum amount of fees owed to a specific position to the recipient*
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
function createAndInitializePoolIfNecessary(address token0, address token1, uint24 fee, uint160 sqrtPriceX96) external payable returns (address pool)
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

### decreaseLiquidity
```solidity
function decreaseLiquidity((uint256,uint128,uint256,uint256,uint256) params) external payable returns (uint256 amount0, uint256 amount1)
```

            

            
*Decreases the amount of liquidity in a position and accounts it to the position*
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
function factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### getApproved
```solidity
function getApproved(uint256 tokenId) external view returns (address operator)
```

            
Returns the account approved for `tokenId` token. Requirements: - `tokenId` must exist.

            
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
function increaseLiquidity((uint256,uint256,uint256,uint256,uint256,uint256) params) external payable returns (uint128 liquidity, uint256 amount0, uint256 amount1)
```

            

            
*Increases the amount of liquidity in a position, with tokens paid by the `msg.sender`*
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
function isApprovedForAll(address owner, address operator) external view returns (bool)
```

            
Returns if the `operator` is allowed to manage all of the assets of `owner`. See {setApprovalForAll}

            
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
function mint((address,address,uint24,int24,int24,uint256,uint256,uint256,uint256,address,uint256) params) external payable returns (uint256 tokenId, uint128 liquidity, uint256 amount0, uint256 amount1)
```

            
Call this when the pool does exist and is initialized. Note that if the pool is created but not initialized a method does not exist, i.e. the pool is assumed to be initialized.

            
*Creates a new position wrapped in a NFT*
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
function name() external view returns (string)
```

            
Returns the token collection name.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### ownerOf
```solidity
function ownerOf(uint256 tokenId) external view returns (address owner)
```

            
Returns the owner of the `tokenId` token. Requirements: - `tokenId` must exist.

            
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
function permit(address spender, uint256 tokenId, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            

            
*Approve of a specific token ID for spending by spender via signature*
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
function positions(uint256 tokenId) external view returns (uint96 nonce, address operator, address token0, address token1, uint24 fee, int24 tickLower, int24 tickUpper, uint128 liquidity, uint256 feeGrowthInside0LastX128, uint256 feeGrowthInside1LastX128, uint128 tokensOwed0, uint128 tokensOwed1)
```

            
Throws if the token ID is not valid.

            
*Returns the position information associated with a given token ID.*
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
function refundETH() external payable
```

            
Useful for bundling with mint or increase liquidity that uses ether, or exact output swaps that use ether for the input amount

            
*Refunds any ETH balance held by this contract to the `msg.sender`*
### safeTransferFrom
```solidity
function safeTransferFrom(address from, address to, uint256 tokenId) external nonpayable
```

            
Safely transfers `tokenId` token from `from` to `to`, checking first that contract recipients are aware of the ERC721 protocol to prevent tokens from being forever locked. Requirements: - `from` cannot be the zero address. - `to` cannot be the zero address. - `tokenId` token must exist and be owned by `from`. - If the caller is not `from`, it must be have been allowed to move this token by either {approve} or {setApprovalForAll}. - If `to` refers to a smart contract, it must implement {IERC721Receiver-onERC721Received}, which is called upon a safe transfer. Emits a {Transfer} event.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |

```solidity
function safeTransferFrom(address from, address to, uint256 tokenId, bytes data) external nonpayable
```

            
Safely transfers `tokenId` token from `from` to `to`. Requirements: - `from` cannot be the zero address. - `to` cannot be the zero address. - `tokenId` token must exist and be owned by `from`. - If the caller is not `from`, it must be approved to move this token by either {approve} or {setApprovalForAll}. - If `to` refers to a smart contract, it must implement {IERC721Receiver-onERC721Received}, which is called upon a safe transfer. Emits a {Transfer} event.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |
| data | bytes | - |

### setApprovalForAll
```solidity
function setApprovalForAll(address operator, bool _approved) external nonpayable
```

            
Approve or remove `operator` as an operator for the caller. Operators can call {transferFrom} or {safeTransferFrom} for any token owned by the caller. Requirements: - The `operator` cannot be the caller. Emits an {ApprovalForAll} event.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| operator | address | - |
| _approved | bool | - |

### supportsInterface
```solidity
function supportsInterface(bytes4 interfaceId) external view returns (bool)
```

            
Returns true if this contract implements the interface defined by `interfaceId`. See the corresponding https://eips.ethereum.org/EIPS/eip-165#how-interfaces-are-identified[EIP section] to learn more about how these ids are created. This function call must use less than 30 000 gas.

            
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
function sweepToken(address token, uint256 amountMinimum, address recipient) external payable
```

            
The amountMinimum parameter prevents malicious contracts from stealing the token from users

            
*Transfers the full amount of a token held by this contract to recipient*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The contract address of the token which will be transferred to `recipient` |
| amountMinimum | uint256 | The minimum amount of token required for a transfer |
| recipient | address | The destination address of the token |

### symbol
```solidity
function symbol() external view returns (string)
```

            
Returns the token collection symbol.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### tokenByIndex
```solidity
function tokenByIndex(uint256 index) external view returns (uint256)
```

            
Returns a token ID at a given `index` of all the tokens stored by the contract. Use along with {totalSupply} to enumerate all tokens.

            
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
function tokenOfOwnerByIndex(address owner, uint256 index) external view returns (uint256 tokenId)
```

            
Returns a token ID owned by `owner` at a given `index` of its token list. Use along with {balanceOf} to enumerate all of ``owner``'s tokens.

            
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
function tokenURI(uint256 tokenId) external view returns (string)
```

            
Returns the Uniform Resource Identifier (URI) for `tokenId` token.

            
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
function totalSupply() external view returns (uint256)
```

            
Returns the total amount of tokens stored by the contract.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### transferFrom
```solidity
function transferFrom(address from, address to, uint256 tokenId) external nonpayable
```

            
Transfers `tokenId` token from `from` to `to`. WARNING: Usage of this method is discouraged, use {safeTransferFrom} whenever possible. Requirements: - `from` cannot be the zero address. - `to` cannot be the zero address. - `tokenId` token must be owned by `from`. - If the caller is not `from`, it must be approved to move this token by either {approve} or {setApprovalForAll}. Emits a {Transfer} event.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |

### unwrapWETH9
```solidity
function unwrapWETH9(uint256 amountMinimum, address recipient) external payable
```

            
The amountMinimum parameter prevents malicious contracts from stealing WETH9 from users.

            
*Unwraps the contract's WETH9 balance and sends it to recipient as ETH.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |

### Events
### Approval
```solidity
event Approval(address owner, address approved, uint256 tokenId)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| owner | address |true| - |
| approved | address |true| - |
| tokenId | uint256 |true| - |

### ApprovalForAll
```solidity
event ApprovalForAll(address owner, address operator, bool approved)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| owner | address |true| - |
| operator | address |true| - |
| approved | bool |false| - |

### Collect
```solidity
event Collect(uint256 tokenId, address recipient, uint256 amount0, uint256 amount1)
```

            
The amounts reported may not be exactly equivalent to the amounts transferred, due to rounding behavior

            
*Emitted when tokens are collected for a position NFT*
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| tokenId | uint256 |true| The ID of the token for which underlying tokens were collected |
| recipient | address |false| The address of the account that received the collected tokens |
| amount0 | uint256 |false| The amount of token0 owed to the position that was collected |
| amount1 | uint256 |false| The amount of token1 owed to the position that was collected |

### DecreaseLiquidity
```solidity
event DecreaseLiquidity(uint256 tokenId, uint128 liquidity, uint256 amount0, uint256 amount1)
```

            

            
*Emitted when liquidity is decreased for a position NFT*
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| tokenId | uint256 |true| The ID of the token for which liquidity was decreased |
| liquidity | uint128 |false| The amount by which liquidity for the NFT position was decreased |
| amount0 | uint256 |false| The amount of token0 that was accounted for the decrease in liquidity |
| amount1 | uint256 |false| The amount of token1 that was accounted for the decrease in liquidity |

### IncreaseLiquidity
```solidity
event IncreaseLiquidity(uint256 tokenId, uint128 liquidity, uint256 amount0, uint256 amount1)
```

            
Also emitted when a token is minted

            
*Emitted when liquidity is increased for a position NFT*
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| tokenId | uint256 |true| The ID of the token for which liquidity was increased |
| liquidity | uint128 |false| The amount by which liquidity for the NFT position was increased |
| amount0 | uint256 |false| The amount of token0 that was paid for the increase in liquidity |
| amount1 | uint256 |false| The amount of token1 that was paid for the increase in liquidity |

### Transfer
```solidity
event Transfer(address from, address to, uint256 tokenId)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| from | address |true| - |
| to | address |true| - |
| tokenId | uint256 |true| - |


