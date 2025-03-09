# PRECISION CANDLES & SMT DIVERGENCE INDICATOR
## User Manual & Best Practices Guide

## TABLE OF CONTENTS

1. [Introduction](#introduction)
2. [Key Features](#key-features)
3. [Quick Start Guide](#quick-start-guide)
4. [Visual Elements Explained](#visual-elements-explained)
5. [Configuration Settings](#configuration-settings)
6. [Interpreting PSP Signals](#interpreting-psp-signals)
7. [Interpreting SMT Divergence](#interpreting-smt-divergence)
8. [Correlation Analysis](#correlation-analysis)
9. [Advanced Trading Strategies](#advanced-trading-strategies)
10. [Known Limitations](#known-limitations)
11. [Installation Process](#how-to-install)
12. [FAQs & Troubleshooting](#faqs--troubleshooting)

---

## INTRODUCTION

The Precision Candles & SMT Divergence indicator is an advanced technical analysis tool designed to identify potential reversal and continuation points through two complementary methods:

1. **PSP (Precision Swing Points)**: Detects when the main chart symbol and a comparison symbol move in opposite directions, with enhanced swing point filtering
2. **SMT Divergence**: Identifies divergences between price action and technical indicators at multiple timeframe levels

> **IMPORTANT**: This indicator is designed as an analytical tool to highlight potential trading opportunities. It should be used in conjunction with other confirmation tools and proper risk management practices.

---

## KEY FEATURES

### Precision Swing Points (PSP)
- Highlights candles where your chart symbol moves opposite to a comparison symbol
- Advanced swing point detection with customizable sensitivity
- Color-coded bullish and bearish PSP identification
- Configurable border highlighting for easy visual detection

### Enhanced Swing Point Filtering
- Configurable swing point detection with customizable lookback and threshold
- Option to display PSP signals only at significant market swing points
- Adjustable sensitivity for swing point identification

### SMT Divergence Analysis
- Multi-level fractal analysis (primary, secondary, tertiary)
- Detects both regular and hidden divergences
- Strength filtering to reduce false signals
- Optional volume confirmation

### Intermarket Analysis
- Real-time correlation calculation and display
- Visualizes comparison symbol candles on the indicator pane
- Automatically adapts analysis to different timeframes

### Visual Customization
- Monochrome mode for reduced visual noise
- Extensive color customization options
- Adjustable line styles and transparency levels

---

## QUICK START GUIDE

### 1. Add the indicator to your chart
- Search for "Imbalances: Precision Candles & SMT Divergence" in the indicator library
- Click "Add to Chart"

### 2. Configure the comparison symbol
- For indices like ES1, try correlated symbols (SPY, QQQ)
- For stocks, try sector ETFs or major index futures
- For forex, try related currency pairs or economic indicators

### 3. Configure Swing Point Detection
- Enable "Only Show PSP at Swing Points" for more meaningful signals
- Adjust "Swing Point Lookback" (recommended: 3)
- Set "Minimum Swing Threshold" based on market volatility

### 4. Select visualization options
- Enable PSP highlighting for entry signals
- Enable SMT divergence lines for trend continuation/reversal signals
- Set the minimum correlation threshold (recommended: 0.5 or higher)

### 5. How to read the indicator
- **Highlighted Candles**: Potential PSP entry signals
- **Colored Lines**: Divergence patterns on multiple timeframes
- **Correlation Display**: Shows statistical relationship between symbols

![Quick Reference](quick_reference_placeholder.png)

---

## CONFIGURATION SETTINGS

### Swing Point Filter Settings

| Setting | Recommended | Description |
|---------|-------------|-------------|
| Only Show PSP at Swing Points | ✅ Enabled | Restrict PSP signals to significant market swing points |
| Swing Point Lookback | 3 | Number of bars to analyze for determining swing points |
| Minimum Swing Threshold (%) | 0.2-1.0 | Percentage difference required between swing point and surrounding candles |

### Interpreting Swing Point Detection

#### How Swing Point Detection Works
- Identifies potential swing highs and lows based on price action
- Compares candle heights within a configurable lookback period
- Applies a minimum percentage threshold to confirm swing points
- Helps reduce noise and focus on more meaningful market turning points

### Best Practices for Swing Point Detection
- Experiment with lookback and threshold settings to match your trading style
- Lower threshold values will identify more swing points
- Higher lookback values provide more conservative swing point detection
- Consider market context and volatility when adjusting settings

---

## VISUAL ELEMENTS EXPLAINED

### Swing Point Filtered PSP Signals

| Element | Description | Reliability |
|---------|-------------|-------------|
| **Green Border/Highlight** | Bullish PSP at Significant Swing Point | ⭐⭐⭐⭐ |
| **Red Border/Highlight** | Bearish PSP at Significant Swing Point | ⭐⭐⭐⭐ |

### Significance of Swing Point Filtering
- Reduces false signals by focusing on meaningful market turning points
- Provides a more refined approach to identifying potential entry/exit opportunities
- Adapts to different market conditions through configurable parameters

### PSP Highlighting

| Element | Description | Reliability |
|---------|-------------|-------------|
| **Green Border/Highlight** | Bullish PSP (comparison red, main green) | ⭐⭐⭐ |
| **Red Border/Highlight** | Bearish PSP (comparison green, main red) | ⭐⭐⭐ |

### Divergence Lines

| Element | Description | Reliability |
|---------|-------------|-------------|
| **Primary Bullish Divergence** | Green line connecting higher lows | ⭐⭐⭐⭐ |
| **Primary Bearish Divergence** | Red line connecting lower highs | ⭐⭐⭐⭐ |
| **Secondary Divergence** | Blue lines (both bullish and bearish) | ⭐⭐⭐ |
| **Tertiary Divergence** | Purple lines (both bullish and bearish) | ⭐⭐ |

### Comparison Symbol Candles

The indicator displays the comparison symbol's candles directly on the indicator pane:

- **Green Candles**: Bullish moves in comparison symbol
- **Red Candles**: Bearish moves in comparison symbol
- **Highlighted Borders**: Indicates PSP conditions

### Correlation Display

Located in the top-right corner of the indicator pane:
- Green text: Positive correlation above threshold
- Red text: Negative correlation below threshold
- Gray text: Correlation too weak (signals less reliable)

> **TIP**: For most reliable signals, the correlation should be consistently above 0.5 (or below -0.5 for inversely correlated instruments).

---

## CONFIGURATION SETTINGS

### General Settings (⚙️ General Settings)

| Setting | Recommended | Description |
|---------|-------------|-------------|
| Comparison Symbol | ES1! for stocks | Symbol to compare against main chart |
| Show Symbol Correlation | ✅ Enabled | Display statistical correlation value |
| Correlation Length | 20 | Period for correlation calculation |
| Minimum Correlation | 0.5 | Threshold for reliable signals |

### PSP Settings (⚙️ PSP Settings)

| Setting | Recommended | Description |
|---------|-------------|-------------|
| Highlight Bullish PSP | ✅ Enabled | Show green borders/highlights |
| Highlight Bearish PSP | ✅ Enabled | Show red borders/highlights |
| Show PSP Borders | ✅ Enabled | Highlight candles with borders |
| Bullish/Bearish Colors | Default colors | Color customization options |

### SMT Divergence Settings (⚙️ SMT Divergence Settings)

#### Fractal Periods

| Setting | Recommended | Description |
|---------|-------------|-------------|
| Primary | 2 | Main fractal period (most reliable) |
| Secondary | 3 | Mid-timeframe fractal (context) |
| Tertiary | 4 | Longer-timeframe fractal (context) |

> **BEST PRACTICE**: For higher timeframes, use smaller fractal periods (1-2). For lower timeframes, use larger values (3-5).

#### Divergence Types

| Setting | Recommended | Description |
|---------|-------------|-------------|
| Regular Divergence | ✅ Enabled | Shows potential trend reversals |
| Hidden Divergence | Optional | Shows potential trend continuation |

#### Divergence Filtering

| Setting | Recommended | Description |
|---------|-------------|-------------|
| Minimum Strength (%) | 0.5-2.0 | Higher values = fewer signals but more reliable |
| Volume Confirmation | ✅ For stocks/futures | Requires increasing volume for valid signals |
| Show Bullish/Bearish Lines | ✅ Enabled | Display divergence lines |
| Show Bullish/Bearish Labels | Optional | Text labels for divergence types |

### Display Settings (⚙️ Display Mode)

| Setting | Recommended | Description |
|---------|-------------|-------------|
| Monochrome Mode | ❌ Disabled | Use grayscale instead of colors |
| Brightness Adjustment | 0.0 | Adjust overall brightness |
| Show Lines on Main Chart | ✅ Enabled | Display divergence on price chart |
| Show Lines on Indicator | ✅ Enabled | Display divergence on indicator |

### Timeframe Adaptation (⚙️ Timeframe Adaptation Settings)

| Setting | Recommended | Description |
|---------|-------------|-------------|
| Auto-Adapt to Timeframe | ✅ Enabled | Automatically adjust parameters based on timeframe |
| Lookback Multiplier | 1.0 | Increase for fewer signals, decrease for more |

---

## INTERPRETING PSP SIGNALS

Precision Swing Points identify when the main symbol and comparison symbol move in opposite directions, potentially signaling strength or weakness.

### Bullish PSP Signal

**Occurs when:**
- Comparison symbol candle is bearish (red)
- Main chart symbol candle is bullish (green)

**Indicates:** The main symbol is showing relative strength against the comparison symbol, potentially signaling upward momentum.

### Bearish PSP Signal

**Occurs when:**
- Comparison symbol candle is bullish (green)
- Main chart symbol candle is bearish (red)

**Indicates:** The main symbol is showing relative weakness against the comparison symbol, potentially signaling downward momentum.

### PSP Signal Strength Factors:

| Factor | Strong Signal | Weak Signal |
|--------|---------------|-------------|
| **Correlation** | Above 0.7 | Below 0.5 |
| **Candle Size** | Large, decisive candles | Small, indecisive candles |
| **Market Context** | Aligned with overall trend | Against overall trend |
| **Volume** | High volume on PSP candle | Low volume on PSP candle |

> **TRADING TIP**: PSP signals work best when they occur at key support/resistance levels or after extended moves in one direction, Use with P&D Levels To Strengthen the PSP and to validate its impact.

---

## INTERPRETING SMT DIVERGENCE

SMT Divergence signals identify when price action and technical indicators move in ways that suggest potential reversals or continuations.

### Regular Divergence (Reversal Signals)

**Bullish Regular Divergence:**
- Price makes lower lows
- Indicator makes higher lows
- **Potential Signal:** Upward reversal

**Bearish Regular Divergence:**
- Price makes higher highs
- Indicator makes lower highs
- **Potential Signal:** Downward reversal

### Hidden Divergence (Continuation Signals)

**Bullish Hidden Divergence:**
- Price makes higher lows
- Indicator makes lower lows
- **Potential Signal:** Upward continuation

**Bearish Hidden Divergence:**
- Price makes lower highs
- Indicator makes higher highs
- **Potential Signal:** Downward continuation

### Fractal Level Significance:

| Fractal Level | Color | Significance | Usage |
|---------------|-------|--------------|-------|
| **Primary** | Green/Red | Immediate signal | Main entry/exit trigger |
| **Secondary** | Blue | Intermediate context | Supporting confirmation |
| **Tertiary** | Purple | Long-term context | Overall trend guide |

> **KEY INSIGHT**: The most powerful signals occur when multiple fractal levels show divergence simultaneously.

---

## CORRELATION ANALYSIS

The correlation between your main chart symbol and comparison symbol is crucial for PSP signal reliability.

### Understanding Correlation Values:

| Correlation | Interpretation | PSP Signal Reliability |
|-------------|----------------|------------------------|
| 0.8 to 1.0 | Strong positive correlation | ⭐⭐⭐⭐⭐ |
| 0.5 to 0.8 | Moderate positive correlation | ⭐⭐⭐⭐ |
| 0.0 to 0.5 | Weak positive correlation | ⭐⭐ |
| -0.5 to 0.0 | Weak negative correlation | ⭐⭐ |
| -0.8 to -0.5 | Moderate negative correlation | ⭐⭐⭐⭐ |
| -1.0 to -0.8 | Strong negative correlation | ⭐⭐⭐⭐⭐ |

### Best Comparison Symbol Pairs:

| Main Instrument | Recommended Comparison | Typical Correlation |
|-----------------|------------------------|---------------------|
| **Futures** | ES1!, NQ! | 0.8-0.9 |
| **Financial Stocks** | XLF, KBE | 0.5-0.8 |
| **EUR/USD** | DXY (inverted) | -0.7 to -0.9 |
| **Gold** | US Dollar (inverted) | -0.6 to -0.8 |
| **Oil** | USO, Energy sector ETFs | 0.7-0.9 |

> **IMPORTANT**: Regularly verify the correlation value. Market relationships change over time, and symbols that were once correlated can become uncorrelated.

---

## ADVANCED TRADING STRATEGIES

### PSP Pullback Strategy

1. Identify strong overall trend direction
2. Wait for a pullback against the trend
3. Look for PSP signal in the direction of the main trend
4. Enter at next candle open with stop below/above PSP candle
5. Target next resistance/support level

### Divergence Confirmation Strategy

1. Identify primary divergence (regular or hidden)
2. Wait for PSP signal in the same direction as divergence
3. Check correlation strength (minimum 0.5)
4. Verify volume is above average (if applicable)
5. Enter with stop beyond the divergence pivot point

### Multiple Timeframe Approach

1. Start on higher timeframe (daily/4H)
2. Identify major divergences and trend direction
3. Move to lower timeframe (1H/15min)
4. Look for PSP entry signals aligned with higher timeframe bias
5. Use tighter stops based on lower timeframe structure

### Intermarket Rotation Detection

1. Monitor correlation between main and comparison symbols
2. When correlation weakens, prepare for potential rotation
3. Look for consecutive PSP signals in one direction
4. Enter early in potential new trend direction
5. Manage risk with wider stops during rotation periods

> **PROFESSIONAL TIP**: The most reliable trades occur when PSP signals, divergence signals, and traditional support/resistance levels all align simultaneously.

---

## KNOWN LIMITATIONS

⚠️ **Be aware of these important limitations:**

1. **Correlation Dependency**
   - PSP signals lose meaning when correlation weakens
   - Correlations change over market regimes
   - No warning when correlation becomes unstable

2. **PSP Signal Quality**
   - Simple directional comparison without magnitude consideration
   - No filtering for small or inside candles
   - Can generate excessive signals in choppy markets

3. **Divergence Limitations**
   - Fixed fractal periods may not adapt to all market conditions
   - No adjustment for varying volatility
   - Lagging nature of divergence patterns

4. **Data Handling**
   - Uses `gaps=barmerge.gaps_off` which can affect real-time signals
   - No handling for missing data in comparison symbol
   - Potential issues with less liquid comparison symbols

5. **Performance Impact**
   - Multiple fractal calculations could slow down charts
   - Drawing many lines can impact performance
   - No cleanup of invalid or aged signals

> **IMPORTANT**: Never trade solely based on PSP or divergence signals. Always use additional confirmation and proper risk management.

---

## How To Install
1. Download the ".pine" script, and copy its context ( or copy directly )
2. Open trading videw, and in the bottom section select the "Pine Editor" option
3. Paste the code inside of the pine editor, and press "Add To Chart" or "Update". ( If a code already exists there, create a new indicator and paste it there )
4. Fully read the manual before usage.
5. Enjoy!

---


## FAQs & TROUBLESHOOTING

### Common Questions

**Q: How should I select the best comparison symbol?**  
A: Choose a symbol with known correlation to your main chart. Index components should use the index, sectors should use sector ETFs, and currencies should use related pairs or economic indicators.

**Q: Should I use Regular or Hidden divergences?**  
A: Regular divergences work best for reversal trades. Hidden divergences work better for continuation trades in established trends.

**Q: Does the indicator repaint?**  
A: The indicator uses `gaps=barmerge.gaps_off` to prevent repainting, but this can introduce some lag in real-time signals.

**Q: Which fractal period is best?**  
A: For lower timeframes (1-15 min), use higher fractal periods (3-5). For higher timeframes (1H+), use lower fractal periods (1-2).

### Troubleshooting

| Issue | Solution |
|-------|----------|
| **Too many signals** | Increase minimum strength filter, increase fractal periods |
| **Too few signals** | Decrease minimum strength filter, decrease fractal periods |
| **Correlation always weak** | Try different comparison symbol with better relationship |
| **Excessive visual clutter** | Enable monochrome mode, reduce number of enabled fractal levels |
| **Performance issues** | Reduce max lines count, disable tertiary fractals |

---

## QUICK REFERENCE CHART

| Element | Description | Reliability | Best Use |
|---------|-------------|-------------|----------|
| **Bullish PSP** | Green border/highlight | ⭐⭐⭐ | Entry timing in uptrends |
| **Bearish PSP** | Red border/highlight | ⭐⭐⭐ | Entry timing in downtrends |
| **Primary Divergence** | Green/Red lines | ⭐⭐⭐⭐ | Major reversal signals |
| **Secondary Divergence** | Blue lines | ⭐⭐⭐ | Trend confirmation |
| **Tertiary Divergence** | Purple lines | ⭐⭐ | Long-term context |
| **Correlation > 0.7** | Strong statistical relationship | ⭐⭐⭐⭐⭐ | Enhanced signal reliability |
| **Volume Confirmation** | Increasing volume at pivots | ⭐⭐⭐⭐ | Signal strength validation |

---

### Final Best Practices

1. **Always verify correlation** before taking signals
2. **Combine PSP and divergence signals** for highest probability trades
3. **Use multiple timeframes** for context and confirmation
4. **Apply proper filtering** to reduce false signals in your market conditions
5. **Adjust fractal periods** based on your timeframe
6. **Use as a confirmation tool**, not a standalone trading system
7. **Understand each market's behavior** - different markets require different settings

---

*This manual is designed for Precision Candles & SMT Divergence Indicator v1.1.0*

*Last Updated: February 2025*
