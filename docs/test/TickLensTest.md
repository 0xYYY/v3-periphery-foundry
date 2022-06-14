
# TickLensTest.sol
Title: Tick Lens contract

## Methods
```solidity
getGasCostOfGetPopulatedTicksInWord
```

### Parameters
| Name | Type | Description |
|---|---|---|
| pool | address |  |
| tickBitmapIndex | int16 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
getPopulatedTicksInWord
```

### Parameters
| Name | Type | Description |
|---|---|---|
| pool | address | The address of the pool for which to fetch populated tick data |
| tickBitmapIndex | int16 | The index of the word in the tick bitmap for which to parse the bitmap and fetch all the populated ticks |


### Return Values
| Name | Type | Description |
|---|---|---|
| populatedTicks | (int24,int128,uint128)[] | An array of tick data for the given word in the tick bitmap |


### Events

### Errors

