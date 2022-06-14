
# IERC721Permit.sol
Title: ERC721 with permit
Notice: Extension to ERC721 that includes a permit function for signature based approvals

## Methods
### DOMAIN_SEPARATOR
```solidity
DOMAIN_SEPARATOR() external view returns (bytes32)
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Return Values

| Type | Description |
|---|---|
bytes32 | - |

### PERMIT_TYPEHASH
```solidity
PERMIT_TYPEHASH() external pure returns (bytes32)
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Return Values

| Type | Description |
|---|---|
bytes32 | - |

### approve
```solidity
approve(address to, uint256 tokenId) external nonpayable
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Parameters

| Name | Type | Description |
|---|---|---|
| to | address | - |
| tokenId | uint256 | - |

### balanceOf
```solidity
balanceOf(address owner) external view returns (uint256 balance)
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### getApproved
```solidity
getApproved(uint256 tokenId) external view returns (address operator)
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Type | Description |
|---|---|
address | - |

### isApprovedForAll
```solidity
isApprovedForAll(address owner, address operator) external view returns (bool)
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |
| operator | address | - |

#### Return Values

| Type | Description |
|---|---|
bool | - |

### ownerOf
```solidity
ownerOf(uint256 tokenId) external view returns (address owner)
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Type | Description |
|---|---|
address | - |

### permit
```solidity
permit(address spender, uint256 tokenId, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
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
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |

```solidity
safeTransferFrom(address from, address to, uint256 tokenId, bytes data) external nonpayable
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
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
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Parameters

| Name | Type | Description |
|---|---|---|
| operator | address | - |
| _approved | bool | - |

### supportsInterface
```solidity
supportsInterface(bytes4 interfaceId) external view returns (bool)
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Parameters

| Name | Type | Description |
|---|---|---|
| interfaceId | bytes4 | - |

#### Return Values

| Type | Description |
|---|---|
bool | - |

### transferFrom
```solidity
transferFrom(address from, address to, uint256 tokenId) external nonpayable
```
Notice: Extension to ERC721 that includes a permit function for signature based approvals
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |


### Events

### Errors

