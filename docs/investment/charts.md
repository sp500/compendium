<script type="text/javascript" src="https://s3.tradingview.com/tv.js"></script>
<script type="text/javascript">
function widget(symbol) {
  new TradingView.widget(
  {
  "height": 610,
  "width": "100%",
  "symbol": symbol,
  "timezone": "Etc/UTC",
  "theme": "light",
  "style": "2",
  "locale": "en",
  "toolbar_bg": "#f1f3f6",
  "enable_publishing": true,
  "withdateranges": true,
  "range": "3M",
  "hide_side_toolbar": false,
  "allow_symbol_change": true,
  "studies": [
    "STD;Bollinger_Bands",
    "STD;MACD",
    "STD;RSI"
  ],
  "show_popup_button": true,
  "popup_width": "1000",
  "popup_height": "950",
  "container_id": symbol
  }
  );
}
</script>

## Financials

## SW
  <div id="ADSK"></div>
  <div id="VRSN"></div>

## Semiconductor
  <div id="ASML"></div>

<script type="text/javascript">
widget("VRSN")
widget("ADSK")
widget("ASML")
</script>
