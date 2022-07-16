
# `TestERC20`

    

    
## Methods
### `DOMAIN_SEPARATOR`
```solidity
function DOMAIN_SEPARATOR() external view returns (bytes32)
```

            
See {IERC20Permit-DOMAIN_SEPARATOR}.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bytes32` | - |

### `allowance`
```solidity
function allowance(address owner, address spender) external view returns (uint256)
```

            
See {IERC20-allowance}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `owner` | `address` | - |
| `spender` | `address` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint256` | - |

### `approve`
```solidity
function approve(address spender, uint256 amount) external nonpayable returns (bool)
```

            
See {IERC20-approve}. Requirements: - `spender` cannot be the zero address.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `spender` | `address` | - |
| `amount` | `uint256` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bool` | - |

### `balanceOf`
```solidity
function balanceOf(address account) external view returns (uint256)
```

            
See {IERC20-balanceOf}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `account` | `address` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint256` | - |

### `decimals`
```solidity
function decimals() external view returns (uint8)
```

            
Returns the number of decimals used to get its user representation. For example, if `decimals` equals `2`, a balance of `505` tokens should be displayed to a user as `5,05` (`505 / 10 ** 2`). Tokens usually opt for a value of 18, imitating the relationship between Ether and Wei. This is the value {ERC20} uses, unless {_setupDecimals} is called. NOTE: This information is only used for _display_ purposes: it in no way affects any of the arithmetic of the contract, including {IERC20-balanceOf} and {IERC20-transfer}.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint8` | - |

### `decreaseAllowance`
```solidity
function decreaseAllowance(address spender, uint256 subtractedValue) external nonpayable returns (bool)
```

            
Atomically decreases the allowance granted to `spender` by the caller. This is an alternative to {approve} that can be used as a mitigation for problems described in {IERC20-approve}. Emits an {Approval} event indicating the updated allowance. Requirements: - `spender` cannot be the zero address. - `spender` must have allowance for the caller of at least `subtractedValue`.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `spender` | `address` | - |
| `subtractedValue` | `uint256` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bool` | - |

### `increaseAllowance`
```solidity
function increaseAllowance(address spender, uint256 addedValue) external nonpayable returns (bool)
```

            
Atomically increases the allowance granted to `spender` by the caller. This is an alternative to {approve} that can be used as a mitigation for problems described in {IERC20-approve}. Emits an {Approval} event indicating the updated allowance. Requirements: - `spender` cannot be the zero address.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `spender` | `address` | - |
| `addedValue` | `uint256` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bool` | - |

### `name`
```solidity
function name() external view returns (string)
```

            
Returns the name of the token.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `string` | - |

### `nonces`
```solidity
function nonces(address owner) external view returns (uint256)
```

            
See {IERC20Permit-nonces}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `owner` | `address` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint256` | - |

### `permit`
```solidity
function permit(address owner, address spender, uint256 value, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external nonpayable
```

            
See {IERC20Permit-permit}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `owner` | `address` | - |
| `spender` | `address` | - |
| `value` | `uint256` | - |
| `deadline` | `uint256` | - |
| `v` | `uint8` | - |
| `r` | `bytes32` | - |
| `s` | `bytes32` | - |

### `symbol`
```solidity
function symbol() external view returns (string)
```

            
Returns the symbol of the token, usually a shorter version of the name.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `string` | - |

### `totalSupply`
```solidity
function totalSupply() external view returns (uint256)
```

            
See {IERC20-totalSupply}.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint256` | - |

### `transfer`
```solidity
function transfer(address recipient, uint256 amount) external nonpayable returns (bool)
```

            
See {IERC20-transfer}. Requirements: - `recipient` cannot be the zero address. - the caller must have a balance of at least `amount`.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `recipient` | `address` | - |
| `amount` | `uint256` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bool` | - |

### `transferFrom`
```solidity
function transferFrom(address sender, address recipient, uint256 amount) external nonpayable returns (bool)
```

            
See {IERC20-transferFrom}. Emits an {Approval} event indicating the updated allowance. This is not required by the EIP. See the note at the beginning of {ERC20}. Requirements: - `sender` and `recipient` cannot be the zero address. - `sender` must have a balance of at least `amount`. - the caller must have allowance for ``sender``'s tokens of at least `amount`.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `sender` | `address` | - |
| `recipient` | `address` | - |
| `amount` | `uint256` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `bool` | - |

### Events
### `Approval`
```solidity
event Approval(address owner, address spender, uint256 value)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| `owner` | `address` |`true`| - |
| `spender` | `address` |`true`| - |
| `value` | `uint256` |`false`| - |

### `Transfer`
```solidity
event Transfer(address from, address to, uint256 value)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| `from` | `address` |`true`| - |
| `to` | `address` |`true`| - |
| `value` | `uint256` |`false`| - |


