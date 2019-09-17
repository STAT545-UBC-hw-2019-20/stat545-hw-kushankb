`{r load, warning=FALSE, echo=FALSE} library(gapminder) library(DT)`
\#Home work 1 with Gap minder data

    anyNA(gapminder)

Exploring the Gapminder data
----------------------------

    str(gapminder)

    summary(gapminder)

Looking at the relation between GDP per capita vs Life Expectancy
-----------------------------------------------------------------

    plot(gapminder$lifeExp,gapminder$gdpPercap)

Looking at the relation between GDP per capita vs life expectancy statistically, the correlation value is:
----------------------------------------------------------------------------------------------------------

    cor(gapminder$lifeExp,gapminder$gdpPercap, method=c("pearson","kendall","spearman"))
