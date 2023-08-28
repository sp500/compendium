## Bollinger Band

### Overview


Bollinger Bands are a set of lines plotted around a moving average of
a stock's price. Developed by John Bollinger in the 1980s, these bands
are designed to adapt to price volatility in a stock (or other
financial instrument). Bollinger Bands consist of three lines:

1. **Middle Band**: This is typically a 20-day simple moving average
(SMA) of closing prices, although the time period can be adjusted.

2. **Upper Band**: This is calculated by adding a chosen number of
standard deviations (usually two) to the middle band.

3. **Lower Band**: This is calculated by subtracting a chosen number
of standard deviations (usually two) from the middle band.

---

### How It Is Calculated

Here's how each band is calculated:

1. **Middle Band**

$$
\text{Middle Band} = \frac{\text{Sum(Close Price)}}{N}
$$

2. **Upper Band**

$$
\text{Upper Band} = \text{Middle Band} + (k \times \text{Standard Deviation})
$$

3. **Lower Band**  

$$
\text{Lower Band} = \text{Middle Band} - (k \times \text{Standard Deviation})
$$

Where:

- \(N\) is the number of periods (usually days).
- \(k\) is the chosen number of standard deviations (usually 2).
- \( \text{Standard Deviation} \) is calculated based on the \(N\) periods of closing prices.

---

### Concept Behind the Math

The mathematical concept behind Bollinger Bands centers around
statistical variations, encapsulated by the standard deviation
which provides an indication of volatility.

1. **Middle Band (SMA)**: This serves as the baseline around which the
bands are drawn and represents a rolling average of prices, smoothing
out fluctuations.
   
2. **Standard Deviation**: This statistic captures the volatility of
the stock price. Higher standard deviation means higher volatility,
and lower standard deviation means lower volatility.

3. **Upper and Lower Bands**: Adding or subtracting standard
deviations from the SMA helps to encapsulate the stock's
volatility. When prices are stable, the bands will narrow. During
times of high volatility, the bands will widen.

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

**Volumn** can provide additional context to the band movements. For
example, a price touch of the upper band accompanied by strong volume
may reinforce a bullish outlook, while the same touch with weak volume
may be less convincing.

**Band Squeeze** where the upper and lower bands come close together,
often precedes a breakout into a new trend. When a strong trend
follows a squeeze, it can signal that the trend is likely to continue
for some time.


### Trend Reversal

**W-bottoms and M-tops** patterns occur when the price forms W-shaped
  bottoms or M-shaped tops. A W-bottom is considered a bullish
  reversal pattern that generally forms at the end of a
  downtrend. Conversely, an M-top is a bearish reversal pattern that
  typically forms at the end of an uptrend.

**Failed Band Breakout** in Bollinger Bands occur when the price of an
  asset breaches one of the outer bands (either upper or lower) but
  reverses direction instead of sustaining the initial trend,
  effectively returning within the band's range. This phenomenon
  contradicts the traditional expectation that a breakout would lead
  to a continuation of the trend in the same direction, thereby
  serving as a potential contrarian indicator. 

**Band Squeeze** or sharp changes in the width of the bands can often
signal an impending price reversal.

**Confluence with Support/Resistance** Bands sometimes align with
  support and resistance levels, amplifying the significance of a
  bounce or break.

**Countertrend Reversals** After a significant period of trending,
  prices touching the opposite band are sometimes viewed as potential
  reversal signals for short-term countertrend plays. However, this is
  a risky strategy and must be used carefully.

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

## Options

### Equivalent Positions in Options Trading

This table shows how equivalent positions can be structured to achieve
similar risk and reward characteristics while using different
combinations of long and short positions in options and the underlying
stock.

| Position                           | Equivalent Position                  | comments |
|------------------------------------|-------------------------------------|---|
| Long OTM call                      | Long stock + Long ITM put           ||
| Long ITM call                      | Long stock + Long OTM put           ||
| Long OTM put                       | Short stock + Long ITM call         ||
| Long ITM put                       | Short stock + Long OTM call         ||
| Covered Call                       | Cash-Secured Short Put              ||
| Long OTM call + Short ATM call      | Long ITM put + Short ATM put        |Bull call spread and bull put spread|
| Long ITM call + Short ATM call      | Long OTM put + Short ATM put        |Bear call spread and bear put spread|
| Long ITM call + Long OTM call 	| Long stock + Long OTM put + Long OTM call| Long strangle|



### Long Stocks with Options

#### Backspread

A backspread is a variation of the call ratio spread (long multiple
OTM call + short ATM calls) equivalent to a net long position in
options.

#### Diagonal Spread

A diagonal spread (long longer-dated OTM or ATM call + short
shorter-dated ATM call) uses the long call to provide upside exposure
and the short call to generate income to offset cost.

#### Synthetic Long Stock

A "synthetic" position (long ITM call + short ITM put) is essentially
bear call spread in IRA type non-margin accounts where your write OTM
call (cash-secured short ITM put) and open long ITM call

#### Collar

A "Collar" position (long stock + long OTM put + short ATM call) is
essentially bull call spread in IRA type non-margin accounts where you
cannot open spreads. 

### Reduceing Holding or Option Premium Costs

The primary goal is to reduce cost bases of holding stock positions.

Long call is necessary to establish upside exposure and the remaining
structure aims to reduce the cost of that exposure to mimic long stock
more efficiently.


#### Open, Roll or Extend Long Calls

With a long call option, you buy call options on a stock you expect to
increase in price. If the stock price goes up, the call options become
more valuable and you can sell them at a profit.

However, buying calls has a cost (the premium paid on put options for
holding long stocks) which raises your effective cost basis on the
stock. If the stock price decreases, the call options lose value but
if you keep rolling or extending the long calls, your stock cost basis
would be lower. 

??? Info "Example"

    Initial Positions
    
            - Position 1: Holding stock A at cost basis of $100
            - Position 2: Long 1 ITM call with strike $90, cost basis $13

    Stock Price Decreases
    
            - Stock A price decreases to $80
            - Position 1 cost basis remains $100
            - Position 2 call option C90 value decreases

    Rolling Long Call

            - Close call option C90 for $3
            - Open new call C70 for $13
            - If assigned stock at $70 strike, new cost basis is $93 ($70 + $13 premium + $10 )

    This demonstrates how rolling long calls on a stock to lower
    strikes when the stock price decreases can lower the effective
    cost basis compared to just holding the stock. The key is using
    some of the value of the original call to open the new lower
    strike call.




### Spreads or Shorts