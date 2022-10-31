# Exploring-the-Bitcoin-Cryptocurrency-Market
Analysis of a sample Bitcoin Cryptocurrency Market based on multiple cryptocurrency characteristics. This project is guided with the help of instruction from datacamp.com

<br />
<br />
  
### Using Cryptocurrency data to complete the following:
* Compare market capitalization of Bitcoin against other cryptocurrencies
* Improving reader usability by implementing a log^10 scale
```
# Plotting market_cap_usd as before but adding the colors and scaling the y-axis  
ax = cap10.market_cap_perc.plot.bar(title=TOP_CAP_TITLE, colors=COLORS, logy=True)
```

* Identifying volatililty (market change) amongst cryptocurrencies
* Find the distribution of coin size by splitting coins into categories of 'biggish', 'micro', and 'nano'

### Data cleaning:
* Cryptocurrencies with no value/ market capitalization are discarded
```
cap = market_cap_raw.query('market_cap_usd > 0')
```

### Techniques for visualizations:
* Matplotlib.pyplot, bar, subplots
```
import matplotlib.pyplot as plt
fig, axes = plt.subplots(nrows=1, ncols=2, figsize=(10, 6))
ax = cap10.market_cap_perc.plot.bar(title=TOP_CAP_TITLE, colors=COLORS, logy=True)
```

### Barplot examples:
<img width="622" alt="Screen Shot 2022-10-31 at 10 42 07 AM" src="https://user-images.githubusercontent.com/116219953/199074371-17ff8afc-a5bf-4134-aac4-67f9e89f501e.png">
<img width="776" alt="Screen Shot 2022-10-31 at 10 44 18 AM" src="https://user-images.githubusercontent.com/116219953/199074391-18ff202a-6aa0-474c-829c-b4a01e5bc11a.png">


