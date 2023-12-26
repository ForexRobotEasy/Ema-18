# Ema 18 Forex Software ReadMe File

## Description
This code is for a Forex software that uses the EMA (Exponential Moving Average) indicator with a period of 18 to determine the trend and generate buy or sell orders. The software calculates the dynamic lot size based on the current account balance and also includes fixed take profit and stop loss levels. The maximum allowed spread is also taken into consideration to ensure trades are executed under favorable market conditions.

## Usage
To use this software, you need to have the MetaTrader 5 trading platform and basic knowledge of trading. Simply copy the code into a new MQL5 script or Expert Advisor, compile it, and attach it to a chart of your desired currency pair.

## Parameters
- `EmaPeriod`: The period for the EMA indicator (default: 18).
- `TakeProfit`: The fixed take profit level in pips (default: 50).
- `StopLoss`: The fixed stop loss level in pips (default: 25).
- `MaxSpread`: The maximum allowed spread in pips (default: 10).

## How It Works
The software continuously checks if the current spread is within the allowable range. If the spread is too high, it waits for better market conditions.

Next, it determines the trend by comparing the current EMA value with the previous EMA value. If the current EMA is higher than the previous EMA, it identifies a bullish trend. If the current EMA is lower than the previous EMA, it identifies a bearish trend.

For a bullish trend, the software calculates the lot size based on the current account balance and places a buy order at the current Ask price with the calculated lot size, take profit, and stop loss levels.

For a bearish trend, it does the same but places a sell order at the current Bid price.

The software provides feedback through comments on the chart, indicating the success or failure of order placement.

## Disclaimer
Forex Robot Easy is not the official developer of this product. This code serves as a sample that can work as described in the product. To find the official developer of this product, please refer to MQL5.

## Product Description and Trading Results
For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Ema 18 Forex Software Review](https://forexroboteasy.com/forex-robot-review/ema-18-forex-software-review-on-optimized-trade-features/).
