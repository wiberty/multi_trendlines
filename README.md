# multi_trendlines
The Multi Trendlines indicator automatically draws the dominant trendlines on the current chart.

The indicator looks for the 5 best Up trends and the 5 best Down trends as at the current price, drawing each trendline if filter conditions are met.

The trendlines are named "Trendline"+[Direction]+Symbol()+TrendlineSequenceNumber

For example:

The second Up trendline on a EURUSD chart would be named "TrendlineUpEURUSD2". To get its current value would be: ObjectGet("TrendlineUpEURUSD2",OBJPROP_PRICE2)

The first Down trendline on a USDJPY chart would be named "TrendlineDownUSDJPY1". To get its current value would be: ObjectGet("TrendlineDownUSDJPY1",OBJPROP_PRICE2)

Potential EA use:

Trade bounce-back or break-out when the price is within material range of a trendline. Note that a trendline clears and recalculates if the price breaks through the trendline, so the EA would need to trigger a signal before the trendline level is crossed by the current price.
