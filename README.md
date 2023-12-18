# Ice Cube Scalper

Ice Cube Scalper is a professional Forex trading robot developed by the Forex Robot Easy Team. This code is a sample implementation of the Ice Cube Scalper strategy in MQL5. 

## Product Description

Ice Cube Scalper is a high-frequency trading robot that aims to generate profits by exploiting short-term price fluctuations in the Forex market. It uses a combination of technical indicators, including the Relative Strength Index (RSI), to identify potential buying opportunities.

The main features of Ice Cube Scalper include:

- **Averaging Strategy**: The robot employs an averaging strategy to open multiple buy positions when the RSI indicator is below the oversold level (30). This allows the robot to take advantage of price reversals and potentially increase profits.

- **Equity Risk Management**: Ice Cube Scalper incorporates a risk management mechanism to limit the maximum equity risk. The user can set the maximum equity risk as a percentage of their account equity. The robot calculates the appropriate lot size based on this risk percentage.

- **Trade Execution**: The robot uses the Trade object from the Trade library to execute trades. It sets a unique expert magic number for identification and subscribes to a free signal called 'FreeSignal' for receiving trade recommendations.

For detailed reviews and trading results of the Ice Cube Scalper product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/review-ice-cube-scalper-for-mt5-a-professional-forex-traders-analysis/). 

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that implements the Ice Cube Scalper strategy. To find the official developer of this product, please refer to MQL5.

## Required Libraries

The code requires the Trade library, which can be found in the 'Trade' folder.

## Input Parameters

- **MaxOrdersForAveraging**: Maximum number of orders for averaging.
- **EquityRiskPercent**: Maximum equity risk in percentage.

## Custom Indicator Initialization Function

The `OnInit` function is called when the custom indicator is initialized. It initializes the Trade object and subscribes to the 'FreeSignal' for trade recommendations.

## Custom Indicator Execution Function

The `OnTick` function is called on every tick. It checks if there are enough bars for indicator calculation and calculates the RSI indicator. If the RSI is below 30, indicating an oversold condition, the robot calculates the lot size based on the equity risk percentage. If the maximum number of orders for averaging is not reached, the robot opens a buy position with averaging.

## Custom Indicator Deinitialization Function

The `OnDeinit` function is called when the custom indicator is deinitialized. It unsubscribes from the 'FreeSignal' to stop receiving trade recommendations.

For more information on the Ice Cube Scalper strategy and its implementation, please refer to the [official developer](https://mql5.com) of this product.
