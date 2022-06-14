
# TickLens.sol
Title: Tick Lens contract

## Methods
### getPopulatedTicksInWord
```solidity
getPopulatedTicksInWord(address pool, int16 tickBitmapIndex) external view returns ((int24,int128,uint128)[] populatedTicks)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | The address of the pool for which to fetch populated tick data |
| tickBitmapIndex | int16 | The index of the word in the tick bitmap for which to parse the bitmap and fetch all the populated ticks |

#### Return Values

| Type | Description |
|---|---|
(int24,int128,uint128)[] | An array of tick data for the given word in the tick bitmap |


### Events

### Errors

