
# IERC721Permit.sol

    
ERC721 with permit

    
*Extension to ERC721 that includes a permit function for signature based approvals*
## Methods
### DOMAIN_SEPARATOR
```solidity
DOMAIN_SEPARATOR() external view returns (bytes32)
```

            

            
*The domain separator used in the permit signature*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### PERMIT_TYPEHASH
```solidity
PERMIT_TYPEHASH() external pure returns (bytes32)
```

            

            
*The permit typehash used in the permit signature*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### approve
```solidity
approve(address to, uint256 tokenId) external nonpayable
```

            
Gives permission to `to` to transfer `tokenId` token to another account. The approval is cleared when the token is transferred. Only a single account can be approved at a time, so approving the zero address clears previous approvals. Requirements: - The caller must own the token or be an approved operator. - `tokenId` must exist. Emits an {Approval} event.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| to | address | - |
| tokenId | uint256 | - |

### balanceOf
```solidity
balanceOf(address owner) external view returns (uint256 balance)
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

### getApproved
```solidity
getApproved(uint256 tokenId) external view returns (address operator)
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

### isApprovedForAll
```solidity
isApprovedForAll(address owner, address operator) external view returns (bool)
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

### ownerOf
```solidity
ownerOf(uint256 tokenId) external view returns (address owner)
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
permit(address spender, uint256 tokenId, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
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

### safeTransferFrom
```solidity
safeTransferFrom(address from, address to, uint256 tokenId) external nonpayable
```

            
Safely transfers `tokenId` token from `from` to `to`, checking first that contract recipients are aware of the ERC721 protocol to prevent tokens from being forever locked. Requirements: - `from` cannot be the zero address. - `to` cannot be the zero address. - `tokenId` token must exist and be owned by `from`. - If the caller is not `from`, it must be have been allowed to move this token by either {approve} or {setApprovalForAll}. - If `to` refers to a smart contract, it must implement {IERC721Receiver-onERC721Received}, which is called upon a safe transfer. Emits a {Transfer} event.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |

```solidity
safeTransferFrom(address from, address to, uint256 tokenId, bytes data) external nonpayable
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
setApprovalForAll(address operator, bool _approved) external nonpayable
```

            
Approve or remove `operator` as an operator for the caller. Operators can call {transferFrom} or {safeTransferFrom} for any token owned by the caller. Requirements: - The `operator` cannot be the caller. Emits an {ApprovalForAll} event.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| operator | address | - |
| _approved | bool | - |

### supportsInterface
```solidity
supportsInterface(bytes4 interfaceId) external view returns (bool)
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

### transferFrom
```solidity
transferFrom(address from, address to, uint256 tokenId) external nonpayable
```

            
Transfers `tokenId` token from `from` to `to`. WARNING: Usage of this method is discouraged, use {safeTransferFrom} whenever possible. Requirements: - `from` cannot be the zero address. - `to` cannot be the zero address. - `tokenId` token must be owned by `from`. - If the caller is not `from`, it must be approved to move this token by either {approve} or {setApprovalForAll}. Emits a {Transfer} event.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |

### Events
### Approval
```solidity
Approval(address owner, address approved, uint256 tokenId)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| owner | address |true| - |
| approved | address |true| - |
| tokenId | uint256 |true| - |

### ApprovalForAll
```solidity
ApprovalForAll(address owner, address operator, bool approved)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| owner | address |true| - |
| operator | address |true| - |
| approved | bool |false| - |

### Transfer
```solidity
Transfer(address from, address to, uint256 tokenId)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| from | address |true| - |
| to | address |true| - |
| tokenId | uint256 |true| - |


