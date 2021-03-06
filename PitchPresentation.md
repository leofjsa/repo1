Choose your car's fuel!
========================================================
author: Leonardo F. Japur de Sa
date: Jan 25th, 2015
transition: rotate
font-family: 'Calibri'
transition: rotate


*A Shiny application for the Coursera Data Science Specialization*


An alternative fuel for your car
========================================================
transition: concave

In Brazil, most cars are called "flexible" because they can use 2 kinds of fuel: *gasoline* and *ethanol*.

### Compare gasoline and ethanol:
- **Environment:** ethanol comes from a renewable source
- **Power (hp):** engines running with ethanol have a little bit more power than with gasoline
- **Price ($ per gallon):** ethanol is cheaper than gasoline
- **Consumption (mpg):** ethanol presents lower mpg than gasoline

In practice, what drivers usually look for is the **most economic!**



How to choose the most economic (example 1)
========================================================
transition: zoom

**General case: mpg(ethanol) = 70% mpg(gasoline)**  
Rule of thumb: compare the price ratio with the mpg ratio.  

An example:

```r
GasolinePrice <- 2.90   # A variable!
EthanolPrice <- 1.90    # A variable too!
PriceRatio <- EthanolPrice / GasolinePrice
mpgRatio <- 0.7         # May be a variable
Conclusion <- ifelse(PriceRatio<mpgRatio, 
                     "ethanol", "gasoline")
paste("Price ratio:", round(PriceRatio, 2), 
      "->" , Conclusion)
```

```
[1] "Price ratio: 0.66 -> ethanol"
```


How to choose the most economic (example 2)
========================================================
transition: zoom

**General case: mpg(ethanol) = 70% mpg(gasoline)**  
Rule of thumb: compare the price ratio with the mpg ratio.  

Another example:

```r
GasolinePrice <- 2.90   # A variable!
EthanolPrice <- 2.10    # A variable too!
PriceRatio <- EthanolPrice / GasolinePrice
mpgRatio <- 0.7         # May be a variable
Conclusion <- ifelse(PriceRatio<mpgRatio, 
                     "ethanol", "gasoline")
paste("Price ratio:", round(PriceRatio, 2), 
      "->" , Conclusion)
```

```
[1] "Price ratio: 0.72 -> gasoline"
```


A Shiny calculator
========================================================
transition: fade

[Click here](http://leofjsa.shinyapps.io/myShinyApp) and access a Shiny calculator.  
Or access directly:
http://leofjsa.shinyapps.io/myShinyApp

### HOW TO USE IT:  
1. Input the gasoline and ethanol prices in your region.  
2. If you wish, you can also adjust the breakeven ratio for your car (the default is 70%).  
3. The application will calculate de price ratio and recommend you the most economic fuel.

**ENJOY!**

