
## Equivalent Positions in Options Trading

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



## Long Stocks with Options

### Backspread

A backspread is a variation of the call ratio spread (long multiple
OTM call + short ATM calls) equivalent to a net long position in
options.

### Diagonal Spread

A diagonal spread (long longer-dated OTM or ATM call + short
shorter-dated ATM call) uses the long call to provide upside exposure
and the short call to generate income to offset cost.

### Synthetic Long Stock

A "synthetic" position (long ITM call + short ITM put) is essentially
bear call spread in IRA type non-margin accounts where your write OTM
call (cash-secured short ITM put) and open long ITM call

### Collar

A "Collar" position (long stock + long OTM put + short ATM call) is
essentially bull call spread in IRA type non-margin accounts where you
cannot open spreads. 

## Reduceing Holding or Option Premium Costs

The primary goal is to reduce cost bases of holding stock positions.

Long call is necessary to establish upside exposure and the remaining
structure aims to reduce the cost of that exposure to mimic long stock
more efficiently.


### Open, Roll or Extend Long Calls

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

## Spreads or Shorts