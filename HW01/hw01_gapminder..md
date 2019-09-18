---
title: "HW01_Gapminder"
output: md_document
---

```{r load, warning=FALSE, echo=FALSE}
library(gapminder)
library(DT)
```
#Home work 1 with Gap minder data
```{r}
anyNA(gapminder)
```

## Exploring the Gapminder data
```{r}
str(gapminder)

summary(gapminder)
```

## Looking at the relation between GDP per capita vs Life Expectancy
```{r}
plot(gapminder$lifeExp,gapminder$gdpPercap)
```

##Looking at the relation between GDP per capita vs life expectancy statistically, the correlation value is:
```{r}
cor(gapminder$lifeExp,gapminder$gdpPercap, method=c("pearson","kendall","spearman"))
```

