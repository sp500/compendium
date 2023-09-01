## Bollinger Band

### Overview


Bollinger Bands are a set of lines plotted around a moving average of
a stock's price. Developed by John Bollinger in the 1980s, these bands
are designed to adapt to price volatility in a stock (or other
financial instrument). Bollinger Bands consist of three lines:

**Middle Band**: This is typically a 20-day simple moving average
(SMA) of closing prices, although the time period can be adjusted.

**Upper Band**: This is calculated by adding a chosen number of
standard deviations (usually two) to the middle band.

**Lower Band**: This is calculated by subtracting a chosen number
of standard deviations (usually two) from the middle band.

---

### Volatility Measurement

**The width of the bands** can serve as an indicator of market
volatility. A widening gap between the bands indicates increasing
volatility, while a narrowing gap suggests decreasing volatility.

**Bollinger Bandwidth** is a measure of the width of the Bollinger
Bands and is calculated as the difference between the upper band and
the lower band divided by the middle band. Decreasing bandwidth
indicates decreased volatility, while increasing bandwidth indicates
increased volatility.

----

### Strong Trends

**The Width of the Bands** often increases in a strongly trending
market as the volatility (standard deviation) is greater. This is due
to the fact that price movements are more extreme during a strong
trend.

**Riding the Bands** prices usually hover between the middle and one
of the outer bands during a strong trend. When prices are consistently
near the upper Bollinger Band, the market is considered to be in a
strong upward trend. Conversely, when prices hover near the lower
Bollinger Band, a strong downward trend is implied.

**Band Squeeze** where the upper and lower bands come close together,
often precedes a breakout into a new trend. When a strong trend
follows a squeeze, it can signal that the trend is likely to continue
for some time.

**Volumn** can provide additional context to the band movements. For
example, a price touch of the upper band accompanied by strong volume
may reinforce a bullish outlook, while the same touch with weak volume
may be less convincing.

----

### Trend Reversal

**Failed Band Breakout** in Bollinger Bands occur when the price of an
  asset breaches one of the outer bands (either upper or lower) but
  reverses direction instead of sustaining the initial trend,
  effectively returning within the band's range. This phenomenon
  contradicts the traditional expectation that a breakout would lead
  to a continuation of the trend in the same direction, thereby
  serving as a potential contrarian indicator. 

**W-bottoms and M-tops** patterns occur when the price forms W-shaped
  bottoms or M-shaped tops. A W-bottom is considered a bullish
  reversal pattern that generally forms at the end of a
  downtrend. Conversely, an M-top is a bearish reversal pattern that
  typically forms at the end of an uptrend.

**Band Squeeze** or sharp changes in the width of the bands can often
signal an impending price reversal.

**Confluence with Support/Resistance** Bands sometimes align with
  support and resistance levels, amplifying the significance of a
  bounce or break.

**Countertrend Reversals** After a significant period of trending,
  prices touching the opposite band are sometimes viewed as potential
  reversal signals for short-term countertrend plays.

**Relative Length of Wick** When using candlestick charts, the
  relative length of the wick that stretches out of the band can also
  be an indicator. A longer wick that stretches out but fails to
  sustain above/below the band can sometimes signify overextension and
  potential reversal.

---

<!---

### Candlestick Patterns
Candlestick patterns like doji, hammer, or engulfing patterns can be used in conjunction with Bollinger Bands.

### Tagging vs. Penetrating Bands
Understand the difference between a "tag" and a penetration of the band.

### Gaps and Bollinger Bands
Price gaps that lead to band breakouts can signify stronger trends or reversals.

### Price and Band Crossover
Crossover of the price and the middle band can signify trend confirmation.

### Harmonics and Chart Patterns
Bollinger Bands can be combined with harmonic patterns for more refined entry and exit points.

### Bollinger Bounce and Squeeze Confirmation
Look for a confirming signal after a Bollinger Band squeeze or bounce.

### Cumulative Indicators
Adding cumulative indicators like On Balance Volume (OBV) can provide additional context.

### Correlation with Other Assets
Price action of related assets can be used in conjunction with Bollinger Bands.

### Adaptive Bollinger Bands
Adjust the settings of the bands based on market conditions for a more responsive analysis.

### Beta Adjustment
Adjust Bollinger Bands based on the stock's beta to interpret it in the context of market behavior.

### Time-Series Forecasting
Use Bollinger Bands in conjunction with time-series forecasting methods like ARIMA.

### Higher Highs and Lower Lows
Watch for higher highs or lower lows in the bands to confirm trends.

### Rate of Change
The rate of change of the band width can indicate volatility acceleration or deceleration.

---->


### How It Is Calculated

Here's how each band is calculated:

$\mathbf{\text{Middle Band}} = \frac{\text{Sum(Close Price)}}{N}$

$\mathbf{\text{Upper Band}} = \text{Middle Band} + (k \times \text{Standard Deviation})$

$\mathbf{\text{Lower Band}} = \text{Middle Band} - (k \times \text{Standard Deviation})$

Where:

- \(N\) is the number of periods (usually days).
- \(k\) is the chosen number of standard deviations (usually 2).
- \( \text{Standard Deviation} \) is calculated based on the \(N\) periods of closing prices.

---

### Concept Behind the Math

The mathematical concept behind Bollinger Bands centers around
statistical variations, encapsulated by the standard deviation
which provides an indication of volatility.

**Middle Band (SMA)**: This serves as the baseline around which the
bands are drawn and represents a rolling average of prices, smoothing
out fluctuations.
   
**Standard Deviation**: This statistic captures the volatility of
the stock price. Higher standard deviation means higher volatility,
and lower standard deviation means lower volatility.

**Upper and Lower Bands**: Adding or subtracting standard
deviations from the SMA helps to encapsulate the stock's
volatility. When prices are stable, the bands will narrow. During
times of high volatility, the bands will widen.

---

<!---
https://www.youtube.com/watch?v=AOz1YPOKvEs

uptrend
downtrend
trend change
consolidation
downward momentum gain
upward momentum gain
momentum loss

long wick candle
---->