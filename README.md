# Momentum-scan-plan

In this project the aim is to get update the allocation on  monthly list of top 20 stocks showing momentum in Nifty 500. The stock list is fetched manually from Definedge securities platform and used Momentum investing scanner. Next based on the available amount the positions in each stock is calculated. If the stock is still in top 40 list, there is no change in position but if it has rank>40, we will exit from stock. Next we have setup a hard limit of 10% on each position. Again if we do not have enough capital to buy a single stock then we will ignore the stocks.

Next if we increase the allocation in a month, then the new capital will be used in new position. Further the aim is to monitor the performance monthly.

Exit: Rank>40 or (-)10% loss on invested amount.
Entry: Equal weighted index of top 20 stocks.
