# SyntheticaFX Zones

## Overview
The SyntheticaFX Zones indicator is a custom indicator for MetaTrader 5 (MT5) platform. It calculates pivotal points using the SyntheticaFX algorithm to identify key levels in the price chart. These key levels can be used by traders to make informed trading decisions.

This code is provided as a sample and is not developed by Forex Robot Easy Team. For detailed reviews and trading results of the official SyntheticaFX Zones product, please visit [this link](https://forexroboteasy.com/forex-robot-review/syntheticafx-zones-review-enhance-trading-with-key-levels/).

## Indicator Inputs
- **period**: The period used for calculating pivotal points. Default value is 14.

## Indicator Initialization
The `OnInit()` function is responsible for initializing the indicator. It registers the indicator with MetaTrader 5 and sets various indicator properties such as name, author, and URL. It also sets up indicator buffers for storing the calculated pivotal points and defines the style and labels for these buffers.

## Indicator Calculation
The `OnCalculate()` function is called for each new bar to calculate the pivotal points using the SyntheticaFX algorithm. It iterates over the price data and calculates the highest high and lowest low within the specified period. Based on these values, it calculates the pivotal points using the formula: `(max_high + min_low) / 2 + ((max_high - min_low) / 4)` for the pivot up level, and `(max_high + min_low) / 2 - ((max_high - min_low) / 4)` for the pivot down level.

The calculated pivotal points are then stored in the indicator buffers for further use.

## Disclaimer
Please note that Forex Robot Easy Team is not the official developer of the SyntheticaFX Zones product. The provided code is only a sample that demonstrates how the algorithm can work. To find the official developer of this product, please refer to the MQL5 platform.

For detailed reviews and trading results of the official SyntheticaFX Zones product, please visit [this link](https://forexroboteasy.com/forex-robot-review/syntheticafx-zones-review-enhance-trading-with-key-levels/).
