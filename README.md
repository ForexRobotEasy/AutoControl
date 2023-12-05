# AutoControl

AutoControl is a trading robot developed by the Forex Robot Easy Team. It is designed to automate the trading process and make it easier for traders to manage their trades. This readme file provides a brief overview of how the code works and its main features.

## Input Parameters

The code includes two input parameters that can be adjusted to customize the trading strategy:

- `tradingCycle`: Specifies the trading cycle in hours. This parameter determines the duration of the trading session.

- `stopTradingTime`: Specifies the stop trading time in hours. Once this time is reached, the trading activity will be stopped.

## How it Works

The main logic of the code is implemented in the `OnTick()` function. Here is a step-by-step breakdown of how it works:

1. The function checks if it's time to stop trading by comparing the current hour with the `stopTradingTime` parameter. If the current hour is greater than or equal to the `stopTradingTime`, the function prints a message indicating that trading has been stopped and returns.

2. The function then calls the `CheckTrend()` function to determine whether the market is in a trend or sideways movement. The result is stored in the `isTrend` and `isSideways` variables.

3. Based on the result from the `CheckTrend()` function, the code either calls the `OpenOrders()` or `CloseOrders()` functions.

- If the market is in a trend (`isTrend` is true), the code calls the `OpenOrders()` function to open new trades based on the selected strategy.

- If the market is in a sideways movement (`isSideways` is true), the code calls the `CloseOrders()` function to close any existing trades.

## Functions

The code includes three additional functions:

1. `CheckTrend()`: This function implements an AI algorithm to judge order trends and calculate lot numbers. It returns true if a trend is detected and false otherwise.

2. `OpenOrders()`: This function implements the code to manually open orders with flexible options based on the selected strategy. Traders can customize this function to place trades according to their preferred strategy.

3. `CloseOrders()`: This function implements the code to manually close orders with flexible options based on the selected strategy. Traders can customize this function to close trades according to their preferred strategy.

## Product Description

[AutoControl](https://forexroboteasy.com/forex-robot-review/autocontrol-forex-software-review-download-and-real-results/) is a powerful trading robot developed by the Forex Robot Easy Team. It is designed to automate the trading process and help traders generate consistent profits in the forex market.

With AutoControl, traders can take advantage of its advanced AI algorithm to identify market trends and make informed trading decisions. The robot is equipped with flexible options, allowing traders to customize their trading strategies and adapt to changing market conditions.

The main features of AutoControl include:

- Ability to define the trading cycle and stop trading time.
- Automatic detection of market trends.
- Manual opening and closing of trades based on selected strategies.
- Flexible options to customize trading parameters.
- Regular updates and improvements to enhance performance.

Please note that ForexRobotEasy is not the official developer of this product. We only provide this sample code as an example of how the product works. To find the official developer of this product and access detailed reviews and trading results, please visit [here](https://forexroboteasy.com/forex-robot-review/autocontrol-forex-software-review-download-and-real-results/). For additional information and support, we recommend using the MQL5 platform.
