# Exploring-the-Bitcoin-Cryptocurrency-Market
Analysis of a sample Bitcoin Cryptocurrency Market based on multiple cryptocurrency characteristics
<br />
<br />
  
### Using Cryptocurrency data to complete the following:
* Compare market capitalization of Bitcoin against other cryptocurrencies
* Improving reader usability by implementing a log^10 scale
```
# Plotting market_cap_usd as before but adding the colors and scaling the y-axis  
ax = cap10.market_cap_perc.plot.bar(title=TOP_CAP_TITLE, colors=COLORS, logy=True)
```

* Identifying volatililty (change) amongst cryptocurrencies
* Find the distribution of coin size by splitting coins into categories of 'biggish', 'micro', and 'nano'

### Data cleaning:
* Cryptocurrencies with no value/ market capitalization are discarded
```
cap = market_cap_raw.query('market_cap_usd > 0')
```

