# Price Action Finder Multi MT5

This code is a custom indicator for MetaTrader 5 that detects and displays various price action patterns on the chart. It can be used to identify potential trading opportunities based on these patterns.

The code defines different types of price action patterns using the `ENUM_PATTERNS` enum. Some of the patterns included are Pin Bar, Outside Bar, Inside Bar, PPR, Force Bar, Hanging Man, and Inverted Hammer.

The `OnInit()` function is the initialization function for the custom indicator. It is responsible for adding any necessary indicators and initializing them. This function returns `INIT_SUCCEEDED` to indicate successful initialization.

The `OnCalculate()` function is the calculation function for the custom indicator. It is called for each new bar on the chart. Within this function, the code iterates through all timeframes and symbols to detect and display price action patterns using the `DetectAndDisplayPatterns()` function.

The `DetectAndDisplayPatterns()` function iterates through all bars on the chart and checks for pattern conditions using individual functions for each pattern type. If a pattern is detected, the `DisplayPattern()` function is called to display the pattern on the chart.

Each pattern detection function (`IsPinBar()`, `IsOutsideBar()`, etc.) implements the logic to check if a specific bar meets the criteria for that pattern. Currently, all pattern detection functions return `false`, indicating that no pattern is detected. The logic for detecting each pattern needs to be implemented within these functions.

The `DisplayPattern()` function is responsible for the display logic of the specified pattern on the chart. Currently, this function does not contain any code and needs to be implemented to display the patterns.

Please note that this code is provided as a sample and is not the official developer's code. ForexRobotEasy is not the official developer of this product. You can find the official developer of this product by using MQL5.

For detailed reviews and trading results of this product, you can visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/price-action-finder-multi-mt5-review-optimize-forex-trades/).
