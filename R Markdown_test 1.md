Markdown document test 1
========================

```{r}
library(datasets)
data("airquality")
summary(airquality)
```

###let's first make a histogram of the file.

```{r}
pairs(airquality)
```
![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2.png)

###Now we will create a regression model

```{r}
library(stats)
rm <- lm(Ozone ~ Wind + Solar.R + Temp, data = airquality)
summary(rm)
```

We are done


