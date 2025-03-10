# 📊 PRECISION CANDLES & SMT DIVERGENCE INDICATOR
## 🌟 Comprehensive User Manual

---

## 📋 TABLE OF CONTENTS

1. [Introduction](#-introduction)
2. [Core Features](#-core-features)
3. [Installation Guide](#-installation-guide)
4. [Visual Elements Guide](#-visual-elements-guide)
5. [Quick Start Guide](#-quick-start-guide)
6. [Configuration Settings](#-configuration-settings)
7. [Signal Interpretation](#-signal-interpretation)
8. [Trading Strategies](#-trading-strategies)
9. [Correlation Analysis](#-correlation-analysis)
10. [Optimization Tips](#-optimization-tips)
11. [Troubleshooting](#-troubleshooting)
12. [Important Warnings](#-important-warnings)

---

## 🔍 INTRODUCTION

The **Precision Candles & SMT Divergence Indicator** is an advanced technical analysis tool designed to identify potential market reversals and continuation patterns through two complementary methods:

1. **PSP (Precision Swing Points)**: Detects when the main chart symbol and comparison symbols move in opposite directions, revealing relative strength and weakness.

2. **SMT Divergence**: Identifies divergences between price action and technical indicators across multiple timeframe levels.

> ⚠️ **IMPORTANT**:  
> This is an ANALYTICAL TOOL, not an automated trading system. It provides insights that require interpretation, not guaranteed signals. Always use proper risk management.

---

## 🚀 CORE FEATURES

### 🎯 Precision Swing Points (PSP)
- Identifies candles where your chart symbol moves opposite to comparison symbols
- Color-coded for intuitive recognition of bullish and bearish signals
- Enhanced swing point filtering with customizable sensitivity

### 📈 SMT Divergence Analysis
- Multi-level analysis (primary, secondary, tertiary timeframes)
- Detects both regular (reversal) and hidden (continuation) divergences
- Strength filtering to reduce false signals

### 🔄 Multi-Symbol Comparison
- Analyze relationships between up to three correlated symbols
- Real-time correlation calculation and display
- Flexible signal generation modes (Any, All, Majority)

### 🎨 Visual Customization
- Comprehensive color settings for all elements
- Monochrome mode for reduced visual noise
- Adjustable transparency and line styles

---

## 🛠️ INSTALLATION GUIDE

### Step-by-Step Installation

1. **Access TradingView Pine Editor**
   - Click on "Indicators" in the top toolbar
   - Select "Pine Editor" from the dropdown menu

2. **Import the Indicator**
   - Clear the default code in the editor
   - Paste the Precision Candles & SMT Divergence indicator code

3. **Save the Indicator**
   - Click "Save" in the Pine Editor
   - Give it a name (e.g., "Precision Candles & SMT Divergence")
   - Click "Save" again

4. **Add to Chart**
   - Click "Add to Chart" to apply the indicator
   - The indicator will appear on your active chart

5. **Configure Settings**
   - Right-click on the indicator name on the chart
   - Select "Settings" to open the configuration panel
   - Adjust parameters as needed (see Configuration section)

> 💡 **TIP**:  
> This indicator works best on timeframes of 5 minutes or higher. Lower timeframes may generate excessive signals.

---

## 🎨 VISUAL ELEMENTS GUIDE

### 💹 PSP Signal Indicators

| Visual Element | Description | Meaning | Reliability |
|----------------|-------------|---------|-------------|
| 🟢 **Green Border** | Bullish PSP | Main chart is green while comparison is red | ⭐⭐⭐ |
| 🔴 **Red Border** | Bearish PSP | Main chart is red while comparison is green | ⭐⭐⭐ |
| 🟩 **Green Zone** | Bullish PSP Zone | Area between body and wick of bullish candle | ⭐⭐⭐ |
| 🟥 **Red Zone** | Bearish PSP Zone | Area between body and wick of bearish candle | ⭐⭐⭐ |
| 🔺 **Swing High Marker** | Identified swing high | Potential resistance point | ⭐⭐⭐⭐ |
| 🔻 **Swing Low Marker** | Identified swing low | Potential support point | ⭐⭐⭐⭐ |

### 📉 Divergence Lines

| Visual Element | Description | Meaning | Reliability |
|----------------|-------------|---------|-------------|
| 📗 **Green Line** (Primary) | Bullish Divergence | Price making lower lows while indicator makes higher lows | ⭐⭐⭐⭐ |
| 📕 **Red Line** (Primary) | Bearish Divergence | Price making higher highs while indicator makes lower highs | ⭐⭐⭐⭐ |
| 📘 **Blue Line** (Secondary) | Secondary Timeframe Divergence | Longer-term divergence pattern | ⭐⭐⭐ |
| 📓 **Purple Line** (Tertiary) | Tertiary Timeframe Divergence | Longest-term divergence pattern | ⭐⭐ |

### 📊 Correlation Table

The correlation table displays in the top-right corner of your chart when enabled, showing:
- Symbol names
- Correlation values (ranging from -1 to 1)
- Current signal status (Bullish, Bearish, or -)

> 💡 **TIP**:  
> Pay close attention to correlation values. Signals are most reliable when correlation is above 0.7 or below -0.7.

---

## 🚦 QUICK START GUIDE

### 1️⃣ Basic Setup for Indices

```
Symbol: ES1! (S&P 500 Futures)
Comparison Symbol 1: NQ1! (Nasdaq Futures)
Minimum Correlation: 0.6
Signal Generation Mode: Any
```

### 2️⃣ Basic Setup for Stocks

```
Symbol: AAPL (Apple Inc.)
Comparison Symbol 1: QQQ (Nasdaq ETF)
Minimum Correlation: 0.5
Signal Generation Mode: Any
```

### 3️⃣ Basic Setup for Forex

```
Symbol: EURUSD (Euro/US Dollar)
Comparison Symbol 1: DXY (US Dollar Index)
Minimum Correlation: 0.7
Signal Mode: Any
```

### 4️⃣ Recommended Initial Settings

```
- Enable PSP Borders: Yes
- Show Correlation: Yes
- Show PSP Zones: Yes
- Fractal Periods: Primary only (enabled)
- Divergence Types: Regular only (enabled)
```

> 🔍 **EXAMPLE**:  
> For S&P 500 trading, use ES1! as your main chart with NQ1! as comparison symbol. Look for bullish PSP signals (green borders) at market swing lows, particularly when they align with bullish divergences (green lines).

---

## ⚙️ CONFIGURATION SETTINGS

### 🌐 General Settings

| Setting | Description | Recommended Value | Notes |
|---------|-------------|-------------------|-------|
| Show Symbol Correlation | Displays correlation values in a table | ✅ Enabled | Essential for signal validation |
| Correlation Length | Period for correlation calculation | 20 | Increase for more stability |
| Minimum Correlation | Threshold for valid signals | 0.5-0.7 | Higher values = fewer but stronger signals |

### 🔄 Multi-Symbol Comparison

| Setting | Description | Options | Notes |
|---------|-------------|---------|-------|
| **Symbols 1-3** | Comparison instruments | Market-dependent | Choose correlated instruments |
| Signal Generation Mode | How to combine multiple signals | Any/All/Majority | "Any" for more signals, "All" for higher quality |
| Display Mode | Which symbols to show on chart | Primary Only/All/Active Signal | Start with "Primary Only" to reduce clutter |

> 💡 **TIP**:  
> For stocks, try sector ETFs as comparison symbols. For indices, other indices or futures work well. For forex, use related currency pairs or economic indicators.

### 📊 Divergence Settings

| Setting | Description | Recommended | Impact |
|---------|-------------|-------------|--------|
| Fractal Periods | Timeframe for divergence detection | Primary: 2<br>Secondary: 7<br>Tertiary: 14 | Higher values = fewer but stronger signals |
| Divergence Types | Which divergences to detect | Regular: ✅<br>Hidden: ⬜ | Enable both for more signals |
| Minimum Strength | Filter weak divergences | 0-2% | Higher = fewer false signals |
| Volume Confirmation | Require higher volume at pivots | ⬜ Disabled | Enable for additional confirmation |

> ⚠️ **IMPORTANT**:  
> Starting with only Primary Fractal enabled is recommended. Add Secondary and Tertiary fractals once you're comfortable with the indicator.

### 🎭 Display Settings

| Setting | Description | Recommended | Notes |
|---------|-------------|-------------|-------|
| Monochrome Mode | Uses grayscale for all elements | ⬜ Disabled | Enable to reduce visual complexity |
| Show Lines on Main Chart | Display divergence lines on price chart | ✅ Enabled | Essential for divergence visualization |
| Line Style | Visual appearance of divergence lines | Dashed | Makes lines distinct from other indicators |
| Maximum Lines | Number of divergence lines to display | 10 | Reduce if chart becomes cluttered |

### 📍 PSP Settings

| Setting | Description | Recommended | Impact |
|---------|-------------|-------------|--------|
| Highlight Bullish/Bearish PSP | Color coding for PSP signals | Both ✅ Enabled | Core functionality of the indicator |
| Show PSP Borders | Highlight candle borders for PSP signals | ✅ Enabled | Makes signals easy to spot |
| Show PSP Zones | Highlight area between body and wick | ✅ Enabled | Visualizes potential entry/exit zones |
| Zone Extension | How many candles to extend PSP zones | 3 | Higher = more visible but potentially cluttered |

> 💡 **TIP**:  
> PSP Zones often act as support/resistance areas. Consider placing stop-loss orders just beyond these zones.

### 🔍 Advanced Swing Point Settings

| Setting | Description | Recommended | Notes |
|---------|-------------|-------------|-------|
| Swing Point Lookback | Bars to analyze for swing detection | 1-3 | Higher = stronger swing points |
| Minimum Swing Threshold | Minimum % change for valid swing | 0.1-1.0% | Adjust based on instrument volatility |
| Check Entire Lookback Window | More thorough swing detection | ✅ Enabled | More accurate but slightly slower |
| Use ATR Filter | Filter based on volatility | ⬜ Disabled | Enable in volatile markets |

---

## 🧠 SIGNAL INTERPRETATION

### 📗 Bullish PSP Signal

**Occurs when:**
- Comparison symbol candle is bearish (red)
- Main chart symbol candle is bullish (green)

**Indicates:** Relative strength against the comparison symbol

**Best used when:**
- Occurs at a swing low
- Correlates with bullish divergence
- Correlation is above minimum threshold
- During an established uptrend or at potential reversal points

### 📕 Bearish PSP Signal

**Occurs when:**
- Comparison symbol candle is bullish (green)
- Main chart symbol candle is bearish (red)

**Indicates:** Relative weakness against the comparison symbol

**Best used when:**
- Occurs at a swing high
- Correlates with bearish divergence
- Correlation is above minimum threshold
- During an established downtrend or at potential reversal points

### 📈 Divergence Signal Quality Factors

| Factor | Strong Signal | Weak Signal |
|--------|---------------|-------------|
| Price Movement | Clear higher/lower highs/lows | Sideways choppy price action |
| Indicator Movement | Strong opposite direction to price | Slight opposite direction |
| Timeframe Alignment | Multiple timeframes show divergence | Only one timeframe shows divergence |
| Volume | Increasing on pivots | Declining on pivots |
| Market Context | Occurs near support/resistance | Occurs in no-man's-land |

> 🔍 **EXAMPLE**:  
> A bullish divergence occurs when price makes a lower low but the indicator makes a higher low. This suggests weakening downward momentum and a potential reversal.

---

## 🎲 TRADING STRATEGIES

### 1️⃣ PSP Reversal Strategy

**Setup:**
1. Identify a strong trend
2. Wait for a pullback against the trend
3. Look for PSP signal in the direction of the main trend
4. Confirm with divergence if possible

**Entry:**
- Enter at the open of the candle following the PSP signal

**Stop-Loss:**
- Place stop below/above the PSP signal candle

**Take-Profit:**
- Target the next significant support/resistance level
- OR use a risk-reward ratio of at least 1:2

### 2️⃣ Multi-Symbol Consensus Strategy

**Setup:**
1. Enable 2-3 highly correlated comparison symbols
2. Set Signal Generation Mode to "All"
3. Wait for consensus signal (all symbols agree)

**Entry:**
- Enter at the open of the candle following the consensus signal

**Stop-Loss:**
- Place stop at recent swing high/low

**Take-Profit:**
- Use previous swing high/low as target
- OR implement trailing stop once in profit

### 3️⃣ Divergence Confirmation Strategy

**Setup:**
1. Identify significant divergence on primary timeframe
2. Wait for PSP signal in the same direction
3. Verify correlation is above 0.7

**Entry:**
- Enter on break of PSP signal candle high/low

**Stop-Loss:**
- Place stop beyond the divergence pivot point

**Take-Profit:**
- Target the previous swing high/low
- OR use measured move (distance of divergence formation)

> ⚠️ **IMPORTANT**:  
> Always combine this indicator with other forms of analysis. Never trade based solely on these signals.

---

## 🌈 CORRELATION ANALYSIS

### Understanding Correlation Values

| Correlation | Interpretation | Signal Quality |
|-------------|----------------|----------------|
| 0.8 to 1.0 | Strong positive correlation | Excellent |
| 0.5 to 0.8 | Moderate positive correlation | Good |
| 0.0 to 0.5 | Weak positive correlation | Poor |
| -0.5 to 0.0 | Weak negative correlation | Poor |
| -0.8 to -0.5 | Moderate negative correlation | Good |
| -1.0 to -0.8 | Strong negative correlation | Excellent |

### Recommended Symbol Pairs

| Main Instrument | Recommended Comparison | Expected Correlation |
|-----------------|------------------------|----------------------|
| ES1! (S&P 500) | NQ1! (Nasdaq) | 0.8-0.9 |
| SPY (S&P 500 ETF) | QQQ (Nasdaq ETF) | 0.7-0.9 |
| EURUSD | DXY (inverted) | -0.7 to -0.9 |
| Gold | US Dollar (inverted) | -0.6 to -0.8 |
| Bank stocks | XLF (Financial ETF) | 0.6-0.8 |
| Oil stocks | XLE (Energy ETF) | 0.7-0.9 |

> 💡 **TIP**:  
> Correlation changes over time. Regularly check the correlation table to ensure your symbol relationships remain strong.

---

## 🔧 OPTIMIZATION TIPS

### Performance Optimization

1. **Reduce Visual Elements**
   - Disable additional comparison symbols
   - Use "Primary Only" display mode
   - Limit the maximum number of divergence lines

2. **Focus Computation**
   - Enable only the fractal periods you actually use
   - Use Primary fractal only for faster charts
   - Set higher minimum strength to filter weak signals

3. **Display Optimization**
   - Consider using Monochrome Mode for cleaner visuals
   - Reduce zone opacity for less visual clutter
   - Disable labels if not needed

### Parameter Tuning by Timeframe

| Timeframe | Fractal Settings | Lookback | Swing Threshold |
|-----------|------------------|----------|-----------------|
| 1-5 min | Primary: 2, Secondary: 5 | 1 | 0.1% |
| 15-30 min | Primary: 2, Secondary: 7 | 2 | 0.2% |
| 1-4 hour | Primary: 3, Secondary: 9 | 2-3 | 0.3-0.5% |
| Daily | Primary: 5, Secondary: 13 | 3 | 0.5-1.0% |
| Weekly | Primary: 8, Secondary: 21 | 3-5 | 1.0-2.0% |

### Market-Specific Adjustments

| Market Type | Correlation Threshold | Signal Mode | Special Considerations |
|-------------|----------------------|-------------|------------------------|
| Trending | 0.5 | Any | Focus on hidden divergences |
| Ranging | 0.7 | All | Focus on regular divergences |
| Volatile | 0.8 | All | Increase swing threshold |
| Low Volatility | 0.6 | Any | Decrease swing threshold |

> 💡 **TIP**:  
> Backtest your settings during different market conditions. What works in trending markets might not work in ranging markets.

---

## ❓ TROUBLESHOOTING

### Common Issues and Solutions

| Issue | Possible Cause | Solution |
|-------|---------------|----------|
| Too Many Signals | Sensitivity too high | Increase strength filter, use "All" signal mode |
| Too Few Signals | Sensitivity too low | Decrease strength filter, use "Any" signal mode |
| Missed Important Moves | Timeframe mismatch | Try different fractal periods, check correlation |
| Correlation Always Low | Wrong comparison symbol | Select a more correlated instrument |
| Excessive Visual Clutter | Too many elements enabled | Use monochrome mode, reduce opacity, limit lines |
| Slow Chart Performance | Excessive calculations | Reduce max bars back, disable tertiary fractals |
| No Divergences Showing | Strength filter too high | Lower minimum strength, enable both divergence types |

### Checking Signal Quality

**Good PSP Signal Characteristics:**
- Occurs at significant swing points
- Has strong correlation (>0.7)
- Clear candle pattern (decisive move)
- Alignment with overall trend or at reversal points
- Confirmed by divergence

**Poor PSP Signal Characteristics:**
- Occurs in choppy price action
- Low correlation (<0.5)
- Small, indecisive candles
- Contradicts higher timeframe trend
- No divergence confirmation

> 🔍 **EXAMPLE**:  
> If you get too many signals in choppy markets, try increasing the minimum correlation to 0.8 and using the "All" signal mode with multiple comparison symbols.

---

## ⚠️ IMPORTANT WARNINGS

### Risk Management

1. **Never trade based solely on indicator signals**
   - Use this indicator as one component of a complete trading system
   - Always confirm with other forms of analysis
   - Consider price action, support/resistance, and trend

2. **Position sizing is critical**
   - Limit risk to 1-2% of account per trade
   - Don't increase position size based on signal strength
   - Use a consistent risk management approach

3. **The indicator is not predictive**
   - It identifies potential opportunities, not guaranteed moves
   - Past performance does not guarantee future results
   - Always use stop-loss orders

### Known Limitations

1. **Correlation Dependency**
   - PSP signals lose meaning when correlation weakens
   - Correlations change over time and market regimes
   - Regularly verify correlation strength

2. **Signal Quality Varies**
   - Simple direction comparison may generate false signals
   - Particularly prone to false signals in sideways markets
   - Performance varies across instruments and timeframes

3. **Divergence Constraints**
   - Fixed fractal periods may not adapt to all market conditions
   - No automatic volatility adjustment
   - Can miss divergences in certain pattern formations

4. **Data Handling Limitations**
   - Potential data lag in real-time trading
   - Limited handling of missing data
   - May have repainting issues in certain configurations

> ⚠️ **CRITICAL WARNING**:  
> This indicator is a tool to assist your analysis, not a replacement for proper trading education, practice, and risk management. Never risk money you cannot afford to lose.

---

## 🏆 FINAL BEST PRACTICES

1. **Start Simple**
   - Begin with only primary fractal and one comparison symbol
   - Add complexity gradually as you gain experience
   - Document settings and results for different markets

2. **Verify Correlation**
   - Always check correlation before trusting signals
   - Adapt comparison symbols as market relationships change
   - Consider inverse correlations for certain pairs

3. **Use Multiple Timeframes**
   - Check signals across different timeframes for confirmation
   - Higher timeframe signals generally have higher reliability
   - Look for alignment across timeframes

4. **Apply Proper Filtering**
   - Adjust strength filters based on current market volatility
   - Tune swing point detection to reduce noise
   - Use ATR filters in highly volatile markets

5. **Treat as Confirmation Tool**
   - Use as confirmation for other analysis methods
   - Combine with support/resistance, trend analysis, and patterns
   - Build a complete trading system around the indicator

6. **Continuous Learning**
   - Markets evolve and so should your approach
   - Regularly review performance and adjust settings
   - Keep journal of trades and indicator performance

---

*Precision Candles & SMT Divergence Indicator Manual v1.3.x*
*Last Updated: March 2025*
