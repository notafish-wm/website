---
title: "Partisan Fertility and Presidential Elections"
authors: ["Gordon B. Dahl", "Runjing Lu", "William Mullins"]
date: "December 2021"
status: "Published. This is the December 2021 working paper version."
journal: "American Economic Review: Insights, 4(4): 473–490, December 2022"
doi: "10.1257/aeri.20210485"
url: "https://www.aeaweb.org/articles?id=10.1257/aeri.20210485"
jel: ["J13", "D72"]
keywords: ["Fertility", "Partisanship", "Elections"]
conversion: "Text-only Markdown for LLM reading. Images omitted. Tables converted to semantic Markdown."
mode: "publication"
---

# Partisan Fertility and Presidential Elections

## Converter's summary

*Written by the converter to orient retrieval; contains no claims absent from the paper.*

The paper asks whether shifts in political power affect fertility, one of the most consequential and irreversible household decisions. It exploits the surprise 2016 election of Donald Trump as an unanticipated change in political power, using difference-in-differences event studies on restricted-use NCHS administrative natality data covering the universe of U.S. births (1994–2019), with the mother's last menstrual period as a proxy for conception date and the outcome measured as deseasonalized "excess" births per 1,000 women aged 15–44 in a county-month. Two designs are used: an across-county comparison of Republican- versus Democratic-leaning counties, and a within-county comparison of Hispanic versus non-Hispanic mothers, motivated by Trump's anti-immigrant rhetoric and Hispanics' roughly two-to-one support for Clinton. Fertility in Republican-leaning counties rises relative to Democratic counties by an amount equal to 1.2% of the 2015 national rate using the 2012 vote share (Table 1, column 1) and 2.2% using the 2008–2016 Republican vote shift (column 2); combining both measures to compare the partisan tails yields 3.2% (column 3). Hispanic fertility falls relative to non-Hispanics by 2.3% of the national rate (column 4), and by roughly 50% more when the comparison group is rural whites (3.3%, column 5) or evangelical whites (3.1%, column 6). Effects grow with the intensity of partisanship — more politically extreme counties, Hispanics versus rural/evangelical whites, and more polarized counties (Figure A4) — which the authors read as evidence that political sentiment drives the results. Trump's pre-election campaign visits reduce relative Hispanic fertility in a triple-difference design (Figure 4, Table A5). Placebo-style context comes from the 2000 election (some evidence of an effect, Figure 3, Table A2) and the 2008 election (no effect, confounded by the Great Recession, Figure A6). The conclusion estimates a net drop of roughly 31,000 births over nine quarters, about 20% of the decline in births over this period.

## Abstract

Changes in political leadership drive sharp changes in public policy and partisan beliefs about the future. We exploit the surprise 2016 election of Trump to identify the effects of a shift in political power on one of the most consequential household decisions: whether to have a child. Republican-leaning counties experience a sharp and persistent increase in fertility relative to Democratic counties, a shift amounting to 1.2 to 2.2% of the national fertility rate. In addition, Hispanics see fertility fall relative to non-Hispanics, especially compared to rural or evangelical whites.

**Keywords:** Fertility, Partisanship, Elections

**JEL Classification Numbers:** J13, D72

**Acknowledgments:** Gordon B. Dahl: UC San Diego, NBER, Norwegian School of Economics, CESifo, CEPR, IZA (gdahl@ucsd.edu); Runjing Lu: University of Alberta (runjing1@ualberta.ca); William Mullins: UC San Diego (wmullins@ucsd.edu). We thank Prashant Bharadwaj, Joseph Engelberg, Mark Huson, Vincent Pons, and Tom Vogl for valuable comments.

## 1. Introduction

Shifts in political power in the United States lead to sharp changes in public policy and partisan beliefs about the future. For example, the election of President Obama led to the Affordable Care Act (ACA), and President Trump enacted the Tax Cuts and Jobs Act (TCJA) and tightened immigration policy. These policy changes could affect voters' views of the future in partisan directions, along both non-economic and economic lines.

Democrats and Republicans are deeply divided on their policy priorities and worries about the future, including on topics such as the environment, inequality, moral values, and immigration (Pew, 2019b). Consistent with this, when Trump was elected, Democrats' satisfaction with "the way things are going in the United States" fell from 43 to 13%, while Republicans' surged from 12 to 46% (Gallup, 2017).

Voters also become more positive about the direction of the nation's economy when they are politically aligned with the winning president, and vice versa. These swings by partisan orientation are large, immediate, and persistent, and especially so after the unexpected victory of President Trump in the 2016 election (see Appendix Figure A1). Similarly, after the 2020 presidential election, Democratic and Republican optimism rapidly exchanged positions. The swings around these two elections are larger than the fall induced by COVID-19.

Do these sharp partisan changes in outlook result in meaningful downstream effects? This paper examines fertility choices following a presidential regime change. Fertility is an irreversible, long-horizon decision made by households, with ensuing effects on labor force participation, housing investments, and consumption choices. These effects may have distributional consequences, with groups targeted by political rhetoric or policy promises responding more to changes in national leadership.

The surprise outcome of the 2016 presidential election is especially valuable for identifying the effect of shifts in political power. Using option markets, Langer and Lemoine (2020) calculates a 12% probability of a Trump victory, while The New York Times and FiveThirtyEight's polling-based forecasts were 15% and 29%. We exploit the 2016 upset as a sharp and unexpected change in political power, using event study designs to compare fertility choices across groups likely to favor Republican or Democratic candidates.

Using administrative data for the universe of U.S. births, our first approach compares fertility across counties with low versus high Democratic vote shares, before versus after the November 2016 presidential election. Republican-leaning counties experience a marked increase in fertility relative to Democratic counties. Our difference-in-differences (DID) estimate equals 1.56 births per 1,000 women summed over nine quarters, for an annualized change equivalent to 1.2% of the 2015 U.S. fertility rate.

Trump's candidacy attracted a different set of voters compared to prior Republican coalitions (Confessore and Cohn, 2016). To capture these new Republican voters, we use the county-level change in the Republican vote share between 2008 and 2016, and classify Republican (Democratic) counties as those whose rightward shift was above (below) median. Using this second measure, we find that Trump's election caused the difference between Republican versus Democratic counties to widen by 2.79 births per 1,000 women, equivalent to 2.2% of the U.S. fertility rate.

These two measures of partisanship capture different sources of variation: the correlation between them is only 0.16. We can combine both measures to define counties in the tails of the partisan distribution. To do so, we take counties which had a high ex ante level of Republican support and shifted strongly towards Trump, and compare them to those with a high level of Democratic support and shifted less. This contrast yields a larger estimate of 3.98, driven disproportionately by rising Republican births.

Our second approach examines Hispanic fertility relative to other groups, as Hispanics were singled out by the Trump campaign and voted approximately two-to-one for Hillary Clinton in 2016.[^1] Using within-county identifying variation, we estimate a decline in the fertility rate for Hispanic mothers relative to non-Hispanics of 2.93 (2.3% of the U.S. fertility rate), largely driven by falling Hispanic births. When we contrast Hispanics to two groups that heavily supported Trump — whites in rural counties and whites in evangelical counties — we find effects that are approximately 50% larger.[^2] We further find heterogeneous effects by the degree of political polarization in a county (Autor et al., 2020): the relative fertility decline for Hispanics is more than twice as large in more versus less polarized counties.

[^1]: When launching his campaign, Trump said "When Mexico sends its people, they're not sending their best... They're sending people that have lots of problems, and they're bringing those problems with us. They're bringing drugs. They're bringing crime. They're rapists. And some, I assume, are good people... It's coming from all over South and Latin America" (Phillips, 2017).

[^2]: Papers examining fertility declines also find differences by demographic groups; see Bailey (2010), Buckles et al. (2019), Kearney et al. (2021).

Taken together, the larger effects we find as the intensity of partisanship increases — i.e., more politically extreme counties, Hispanics versus rural and evangelical whites, and more polarized counties — all point towards political sentiment driving these effects. All of our results display parallel pre-trends, each measure of partisanship is robust to alternate definitions, and effects are persistent.

There could be multiple mechanisms underlying these partisan fertility responses. For example, when presidential regime shifts occur, expected or actual policies favoring specific groups could lead to partisan changes in family size decisions. Partisans of the winning side could also become more optimistic about the direction of the economy, leading to an income effect for fertility. Further, a Trump victory could cause Republicans and Democrats to update their views about the political and social climate, thereby affecting their willingness to bring a child into the world.

To place our results in perspective, we examine the two preceding party-switching presidential elections. After George W. Bush barely won the 2000 election, we find some evidence that fertility in Democratic versus Republican counties falls, particularly for those with low evangelical population shares. For Obama's 2008 election victory, which was not a surprise, we find no partisan fertility effect; however, the Great Recession confounds this analysis.

Our estimated fertility effects are comparable to the effects of unemployment and cash transfers on fertility. For example, Dettling and Kearney (2014) and Schaller (2016) report that a 1% increase in the unemployment rate is associated with a decrease in birth rates between 1.4% and 2.2%. Similarly, Raute (2019) and Milligan (2005) find that a \$1,000 increase (in 2020 USD) in cash subsidies for a birth results in a 1.8% to 2.1% increase in fertility.

Our paper relates to a recent literature which documents rising political polarization in the United States (Autor et al., 2020, Bertrand and Kamenica, 2018, Boxell et al., 2020, Gentzkow, 2016, Pew, 2020). COVID-19 has highlighted that political polarization extends to health-seeking behaviors, such as social distancing and vaccinations (e.g. Allcott et al., 2020, Chen et al., 2020, Fridman et al., 2021, Grossman et al., 2020). A few papers report a relationship between partisanship and spending on consumer goods (Benhabib and Spiegel, 2019, Gerber and Huber, 2009, Gillitzer and Prasad, 2018), but others have challenged this link (McGrath, 2017, Mian et al., 2021). Further, a group of papers have linked partisanship with financial outcomes, such as tax evasion, stock market trading, corporate credit, and retirement investing (Cookson et al., 2020, Cullen et al., 2021, Dagostino et al., 2020, Kempf and Tsoutsoura, 2020, Meeuwis et al., 2021).[^3]

[^3]: Our paper relates to a broader literature on the economic determinants of fertility, including unemployment, income, housing prices, coal busts, fracking booms, Medicaid eligibility, COVID-19, cash transfers, and child subsidies (Aizer et al., 2020, Autor et al., 2019, Black et al., 2013, Buckles et al., 2021, Cohen et al., 2013, Currie and Schwandt, 2014, Dettling and Kearney, 2014, Duncan et al., 2017, Kearney and Levine, 2009, 2021, Lindo, 2010, Lovenheim and Mumford, 2013, McCrary and Royer, 2011, Raute, 2019, Schaller, 2016).

Across many nations, growing political polarization and declining fertility are two fundamental challenges facing society. We estimate effects at the intersection of these two forces. Our contribution is to causally link partisan sentiment to one of the most consequential household decisions: whether to have a child (Becker, 1960). Unlike many consumption and investment choices, having a child is a long-term commitment requiring significant time and money: the USDA-estimated cost of raising a child to age 17 is \$233,000 (Lino, 2020).

Growing partisanship makes understanding the downstream effects of elections increasingly relevant. The shifts in fertility we identify have practical implications for regional public finance and population-based congressional apportionment, given partisan sorting across residential geographies (Bernstein et al., 2021, Brown and Enos, 2021, Kaplan et al., 2020).[^4] Moreover, understanding the drivers of fertility is important in light of declining and below-replacement fertility, and its structural effects on economic growth (Jones, 2020).

[^4]: For example, New York lost a congressional seat to Minnesota by 89 residents based on the 2020 Census (Goldmacher, 2021).

## 2. Data and Research Design

We begin by examining how fertility responds to the unexpected election victory of candidate Trump in 2016. We use two main strategies in a DID design: comparing fertility in Republican versus Democratic-leaning counties, and comparing Hispanic fertility to that of non-Hispanics.

### 2.1 Fertility Data

We use restricted-use U.S. administrative natality data from 1994 to 2019 from the National Center for Health Statistics (NCHS). The data covers the universe of U.S. births and provides detailed information that includes the month of birth (MOB), the month of the first day of the mother's last menstrual period (MLMP), and the mother's age, race/ethnicity, and county of residence. We restrict our attention to singleton births to U.S. resident mothers between the ages of 18 and 44.

Our main outcome of interest is the number of births conceived in a county-month per 1,000 females between 15 and 44 years old.[^5] We use mothers' reported MLMP as a proxy for conception date following the literature (e.g., Dehejia and Lleras-Muney 2004).[^6] Summary statistics for fertility are in Table A1; the mean monthly fertility rate in a county is 4.5 births per 1,000 females. We deseasonalize fertility by subtracting its county × month-of-year average using data starting from 2010, and refer to this variable as excess fertility.

[^5]: We use as the denominator the number of fertile females between 15 and 44 years old – rather than 18 and 44 – because U.S. intercensal county population estimates by age, sex, and ethnicity are reported in five-year age bins. The population estimates are from Census Bureau. We adjust births due to the extra day in February of leap years by multiplying the fertility rate in that month by 28/29. To ensure that the fertility rate is calculated based on a reasonably-sized female pool, we drop counties whose fertile female population is below the 10th percentile in 2012 (i.e., 769 women).

[^6]: We remove misreported records by requiring the difference between MOB and MLMP to be between 5 and 12 months.

The natality data only records the month of the beginning of the mother's last menstrual period. There is typically a seven-day lag between the first day of menses and the fertile period, which lasts approximately two weeks (NCHS, 2005). Thus, MLMP measures the month of conception with noise. Since the election occurred on November 8, 2016, a mother whose MLMP is in October could have conceived her child after the election. Assuming a uniform distribution of conception dates in a month, about 30% of mothers whose MLMP is in October are predicted to conceive after the election.

### Table A1: Summary Statistics for 2016 Election

- **Table type:** Summary statistics
- **Unit of observation:** county (race/ethnicity-specific means across counties)
- **Outcome definitions:** *Fertility rate* = monthly births conceived per 1,000 women aged 15–44 for each race/ethnicity in a county. *Excess fertility rate* = the fertility rate after subtracting the race/ethnicity × county × month-of-year mean using data from 2010 onward.
- **Coverage:** Panel A (election sample) covers January 2016 – December 2018; Panel B (campaign sample) covers September 2014 – September 2016.

#### Panel A: Election sample

| race | fertility_rate_mean | fertility_rate_sd | excess_fertility_mean | excess_fertility_sd |
|---|---:|---:|---:|---:|
| Total | 4.495 | 0.864 | -0.137 | 0.499 |
| Hispanic | 5.134 | 1.492 | -0.300 | 1.057 |
| Mexican | 4.726 | 1.835 | -0.182 | 1.436 |
| Non-Hispanic | 4.280 | 0.898 | -0.107 | 0.545 |
| Non-Hispanic minority | 4.699 | 1.329 | -0.111 | 0.997 |
| Non-Hispanic white | 4.266 | 1.040 | -0.104 | 0.639 |
| N counties | 2,830 | 2,830 | 2,830 | 2,830 |

#### Panel B: Campaign sample

| race | fertility_rate_mean | fertility_rate_sd |
|---|---:|---:|
| Hispanic | 5.159 | 1.064 |
| Non-Hispanic | 4.299 | 0.649 |
| Non-Hispanic white | 4.204 | 0.768 |
| N counties | 230 | 230 |

**Note:** The fertility rate corresponds to monthly births conceived per 1,000 women who are between 15 and 44 years old for each race/ethnicity in a county. The excess fertility rate is calculated by subtracting the race/ethnicity × county × month-of-year mean using data from 2010 onward. Data in panels A and B cover January 2016 - December 2018 and September 2014 - September 2016, respectively.

### 2.2 Difference-in-Differences Event Study

Our main research design is a DID event study using the 2016 presidential election as the event. Our first approach compares fertility across Democratic and Republican counties before versus after the election. To measure county partisanship, we obtain the county-level vote share in presidential elections from the MIT Election Data and Science Lab. In our first definition, counties are categorized as Democratic if their Democrat vote share in 2012 is above the median, and Republican otherwise.

To include the new Republican voters who were drawn to Trump in 2016, our second definition uses the county-level change in the Republican vote share between 2008 and 2016 and classifies counties with an above-median change (i.e., a shift of more than 5.8 percentage points) as Republican, and Democratic otherwise.

Our first regression model is:

$$Y_{ct} = \sum_{t=-3}^{8} \beta_t \times Democratic_c + \alpha_c + \alpha_t + \epsilon_{ct} \tag{1}$$

where $Y_{ct}$ is the excess fertility rate in county $c$ and time $t$, which is the number of quarters relative to the presidential elections. We use $t = -1$ as our comparison period. Our treatment variable is $Democratic_c$, which equals one if county $c$ is classified as Democratic, and zero otherwise. We include event time fixed effects $\alpha_t$ to control for national fertility trends. Including county fixed effects $\alpha_c$ is largely redundant, because our excess fertility rate already controls for county × month-of-year effects.[^7] We cluster standard errors by county.

[^7]: We obtain excess fertility by subtracting county × month-of-year means, which is not perfectly colinear with county fixed effects because it is based on a longer sample period.

While the data is monthly, for precision and ease of presentation in our main analyses we collapse the data by quarter. For the 2016 election, we define $t = 0$ as October, November, and December. As described in section 2.1, October is a partially-treated month, which is why we group it with November and December.

Our second approach compares Hispanic to non-Hispanic fertility. In contrast to our first approach, this compares Hispanic to non-Hispanic mothers within counties, rather than using an across-county design. The regression model is:

$$Y_{kct} = \sum_{t=-3}^{8} \beta_t \times Hispanic_k + \alpha_{kc} + \alpha_t + \epsilon_{kct} \tag{2}$$

where $Y_{kct}$ is the excess fertility rate for females belonging to ethnic group $k$ in county $c$ in time $t$. $Hispanic_k$ is one if the ethnic group is Hispanic, and zero otherwise. Similar to equation 1, ethnicity-specific county fixed effects $\alpha_{kc}$ are largely redundant given that excess fertility is calculated by subtracting ethnicity × county × month-of-year means for each group.

If the result of the 2016 presidential election was unanticipated, and fertility trends across counties or across different ethnic groups are parallel in the absence of the election, the $\beta_t$ vectors in equations 1 and 2 identify the impact of the presidential election on fertility decisions before and after the election. As we will show, both of these conditions appear to hold.

## 3. Results

### 3.1 Fertility Effects across Political Geographies

#### Graphical evidence

In Figure 1, we show the effects of the 2016 election on fertility in Democratic and Republican counties. In panel A1, we start by comparing the raw trend of monthly excess fertility in counties with above- or below-median Democratic vote share in the 2012 presidential election. The blue line captures the excess fertility in Democratic counties and the red in Republican counties. Both lines are normalized to be 0 in September 2016. The vertical shaded area spanning the months of October and November indicates the period immediately surrounding the election. As described in section 2.1, October represents a partially-treated month due to how conceptions are measured in our data.

The first thing to note is that the blue and red lines lie on top of each other in the pre-period, consistent with the assumption of parallel trends. Post election, looking at the time pattern of the blue and red lines separately provides suggestive evidence of each group's fertility dynamics. The red line for Republican counties spikes in November and December. While there is little evidence of an effect on Democratic fertility in these two months, over time the blue line declines steadily. This graphical evidence suggests that Republicans have an immediate jump in births post-election, while Democratic fertility appears to exhibit a trend break which becomes progressively more negative.

A key advantage of our approach is that it can account for common shocks to Republican and Democratic fertility. Panel A2 plots the $\beta_t$ coefficients from equation 1, capturing the effect of the presidential election on differential fertility across Democratic versus Republican counties. Confirming the pattern in the raw monthly data, there are no pre-trends in the quarterly event study regression coefficients. Panel A1 shows that the difference between the red and the blue lines persists through the entire post election period. The quarterly regression coefficients plotted in panel A2, which are always statistically different from zero, confirm this pattern.

The results in panels A1 and A2 use the Republican vote share before Trump was an active politician. This captures the traditional Republican coalition of voters. In 2016, Trump attracted a different set of voters, so as an alternative we use the county-level change in the Republican vote share between 2008 and 2016. This measure captures counties where new voters were most attracted to the Trump platform. These two measures of partisanship capture different sources of variation: their correlation is only 0.16.

Panel B1 plots the monthly excess fertility for counties with an above-median shift towards the Republican party (red dashed line) and counties with a below-median shift (blue line). Panel B2 plots the quarterly regression coefficients. Again there is no evidence of differential pre-trends either in the raw data or in the regression setting.

The gaps in excess fertility using the rightward shift measure (column B) are larger than those using the Republican vote share (column A). One possible explanation is that counties that swung most towards the Republican Party were the most enthused by Trump's policies.

In column C, we define extreme Republican counties (dashed red line) as those with a below-median Democratic vote share and an above-median vote shift towards Trump. We similarly define extreme Democratic counties (blue line). This interaction of our two measures results in even stronger effects, consistent with the low correlation between them. By combining them, we define treated counties as those which have both types of Trump support (traditional Republican or newly enthused), while excluding both types from the control group.

Comparing these counties in the tails of the partisan distribution yields substantially larger effects: an increase of approximately 150% compared to column A and 50% compared to column B. The stronger fertility response we find for more politically extreme counties adds credence to the idea that partisanship drives our results.[^8]

[^8]: In May 2016 there is a sizable jump in the dashed red line in panel C1. This was the month that Trump became the presumptive nominee of the Republican party, which may have contributed to the jump.

### Figure 1: 2016 Presidential Election and Fertility in Democratic versus Republican Counties

- **Panels A1, B1, C1 (top row):** raw monthly excess fertility by group, normalized to September 2016. Y-axis: "Excess fertility". X-axis: calendar months (2016Apr–2018Oct). Shaded band: October–November 2016 (onset of treatment).
- **Panels A2, B2, C2 (bottom row):** quarterly event-study $\beta_t$ coefficients with 95% confidence intervals. Y-axis: "Differential excess fertility". X-axis: "Quarters from election" (-3 to 8). Omitted quarter: -1.
- **Column A (A1/A2):** by 2012 Democratic vote share. Legend: "Democratic" (blue), "Republican" (red dashed).
- **Column B (B1/B2):** by 2008–2016 change in Republican vote share. Legend: "Low Rep. shift" (blue), "High Rep. shift" (red dashed).
- **Column C (C1/C2):** by vote share × Republican shift (interaction of both measures). Legend: "Dem. × Low Rep. shift" (blue), "Rep. × High Rep. shift" (red dashed).

**Note:** This figure plots effects (and 95% confidence intervals) for the excess fertility rate in Democratic-leaning relative to Republican-leaning counties around the 2016 presidential election. Fertility rates in panels A1 to C1 are normalized to September 2016. As described in section 2.2, October represents a partially-treated month, so we shade October and November to indicate the onset of treatment. Panel A1 plots the excess fertility rate in counties with above-median versus below-median Democratic vote shares in the 2012 presidential election; Panel B1 counties with below-median versus above-median change in Republican vote shares between the 2008 and 2016 presidential elections; Panel C1 counties with both above-median Democratic vote shares and below-median Republican shifts versus counties where both measures are the opposite. Panels A2 to C2 plot the interactions between quarters and an indicator for Democratic-leaning counties from equation 1. The omitted quarter is -1 (July-September 2016). Specifications correspond to Table 1 columns (1) to (3).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred. (Corresponding regression estimates are in Table 1, columns 1–3.)

#### Regression results

Regression results corresponding to Figure 1 are found in Table 1, columns (1) through (3). For example, the $Treat_0$ coefficient in column (1) represents a drop of 0.139 excess births per 1,000 women in Democratic relative to Republican counties in the quarter of the election (quarter 0). The average treatment effect in quarters 0 through 8 amounts to 0.173 excess births, a shift equivalent to 1.2% of the 2015 national fertility rate. In 2015, Republican counties already had higher quarterly fertility than Democratic ones: 14.83 versus 13.81 births per 1,000 women. Our estimates imply that Trump's election widened this gap by 17%.

Column (2) indicates a larger effect, with an average of 0.309 fewer excess births in counties with a below versus above median shift in the Republican vote share. This change corresponds to 2.2% of the 2015 national fertility rate. This widens an originally small Republican versus Democratic fertility gap of 0.18 by over 170%. Finally, column (3) shows an even larger treatment effect for the subsample comparing extreme Democratic versus extreme Republican counties. Following the election of Trump, there were 0.44 fewer excess births (amounting to 3.2% of the 2015 fertility rate for these counties), widening a preexisting gap of 0.85 by around 50%.

To aid interpretation, the sum of treatment effects in quarters 0 through 8 in column (1) translates into a fertility gap of 46,000 births (0.6% of the total number of births in 2015) between Republican and Democratic counties.[^9] Similarly, the sum of treatment effects in column (2) translates into a fertility gap of 66,000 births (0.8% of total births). Column (3) translates to 62,000 births (1% of births in this subsample).

[^9]: This translation requires an additional assumption about the counterfactual post election trend. We extrapolate the change in the total excess fertility rate over the pre-period (January 2015 to September 2016) to the post-period and calculate the deviations in the number of births from this counterfactual for each group.

In our main specification, we restrict the time window to the three quarters before the election to minimize contamination by party primaries, as these may have had direct effects on partisan fertility. Appendix Figure A2 expands the time window to seven quarters pre-election for completeness.

### Table 1: 2016 Presidential Election and Fertility

- **Table type:** Regression (DID event study)
- **Dependent variable:** excess fertility rate
- **Estimator:** OLS event study; interactions between event-time quarter and a treatment indicator
- **Standard errors:** clustered by county (reported in parentheses)
- **Omitted quarter:** -1 (July–September 2016)
- **Treatment group:** the first group named in each column header
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | comparison | treatment_indicator | identifying_variation |
|---|---|---|---|
| 1 | Dem. vs Rep. (2012 vote share) | Democratic-leaning (equation 1) | across-county |
| 2 | Low vs high Rep. shift (2008–2016) | Democratic-leaning (equation 1) | across-county |
| 3 | Vote share × shift (partisan tails) | Democratic-leaning (equation 1) | across-county |
| 4 | Hisp. vs non-Hisp. | Hispanic ethnicity (equation 2) | within-county |
| 5 | Hisp. vs rural white | Hispanic ethnicity (equation 2) | within-county |
| 6 | Hisp. vs evan. white | Hispanic ethnicity (equation 2) | within-county |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Treat−3 | coefficient | -0.038 | -0.065 | -0.092 | -0.051 | -0.010 | -0.062 |
| Treat−3 | standard_error | (0.061) | (0.061) | (0.094) | (0.059) | (0.088) | (0.075) |
| Treat−2 | coefficient | -0.018 | -0.082 | -0.105 | -0.061 | -0.071 | -0.101 |
| Treat−2 | standard_error | (0.055) | (0.058) | (0.089) | (0.050) | (0.083) | (0.069) |
| Treat0 | coefficient | -0.139** | -0.169*** | -0.267*** | -0.198*** | -0.249*** | -0.258*** |
| Treat0 | standard_error | (0.056) | (0.058) | (0.091) | (0.048) | (0.083) | (0.067) |
| Treat1 | coefficient | -0.108* | -0.207*** | -0.379*** | -0.278*** | -0.439*** | -0.379*** |
| Treat1 | standard_error | (0.060) | (0.062) | (0.088) | (0.056) | (0.089) | (0.074) |
| Treat2 | coefficient | -0.185*** | -0.306*** | -0.443*** | -0.315*** | -0.523*** | -0.430*** |
| Treat2 | standard_error | (0.067) | (0.065) | (0.094) | (0.057) | (0.089) | (0.074) |
| Treat3 | coefficient | -0.176** | -0.309*** | -0.448*** | -0.320*** | -0.548*** | -0.478*** |
| Treat3 | standard_error | (0.075) | (0.073) | (0.105) | (0.058) | (0.096) | (0.083) |
| Treat4 | coefficient | -0.131* | -0.291*** | -0.344*** | -0.342*** | -0.512*** | -0.488*** |
| Treat4 | standard_error | (0.073) | (0.072) | (0.100) | (0.067) | (0.101) | (0.090) |
| Treat5 | coefficient | -0.160** | -0.351*** | -0.509*** | -0.358*** | -0.614*** | -0.542*** |
| Treat5 | standard_error | (0.069) | (0.068) | (0.097) | (0.063) | (0.100) | (0.089) |
| Treat6 | coefficient | -0.181*** | -0.296*** | -0.423*** | -0.404*** | -0.573*** | -0.586*** |
| Treat6 | standard_error | (0.066) | (0.067) | (0.096) | (0.068) | (0.099) | (0.089) |
| Treat7 | coefficient | -0.223*** | -0.429*** | -0.596*** | -0.367*** | -0.640*** | -0.549*** |
| Treat7 | standard_error | (0.080) | (0.074) | (0.102) | (0.077) | (0.107) | (0.099) |
| Treat8 | coefficient | -0.258*** | -0.427*** | -0.570*** | -0.340*** | -0.600*** | -0.539*** |
| Treat8 | standard_error | (0.082) | (0.077) | (0.107) | (0.100) | (0.131) | (0.123) |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Avg. Treat (0 to 8) | -0.173 | -0.309 | -0.442 | -0.325 | -0.522 | -0.472 |
| 2015 avg. birth rate | 14.007 | 14.007 | 13.878 | 13.896 | 15.701 | 15.221 |
| Avg. Treat/2015 avg. | -1.2% | -2.2% | -3.2% | -2.3% | -3.3% | -3.1% |
| 2015 avg. Treat-Control gap | -1.018 | -.181 | -.848 | 2.994 | 1.925 | 2.308 |
| Avg. Treat/2015 avg. gap | 17% | 171% | 52% | -11% | -27% | -20% |
| Observations | 33,756 | 33,756 | 19,608 | 67,920 | 53,052 | 50,904 |
| R-squared | 0.367 | 0.369 | 0.394 | 0.314 | 0.247 | 0.272 |
| County FE | Y | Y | Y | N | N | N |
| County×Ethnicity FE | N | N | N | N | N | N |
| Quarter event FE | Y | Y | Y | Y | Y | Y |
| N cluster county | 2,813 | 2,813 | 1,634 | 2,830 | 2,830 | 2,830 |

**Note:** This table reports the estimates depicted in panels A2 to C2 in both Figures 1 and 2. The dependent variable is the excess fertility rate. The treatment group is the first group named in each column header. Columns (1) to (3) report interactions between quarters and a Democratic-leaning indicator from equation 1. Column (1) compares counties with above-median to those with below-median Democratic vote shares in the 2012 Presidential election; column (2) counties with below-median to above-median change in Republican vote shares between the 2008 and 2016 Presidential elections; column (3) counties with both above-median Democratic vote shares and below-median Republican shifts to counties where both measures are the opposite. Columns (4) to (6) report interactions between quarters and an indicator for Hispanic ethnicity from equation 2. Column (4) compares Hispanics to non-Hispanics; column (5) versus non-Hispanic whites living in rural counties; column (6) versus non-Hispanic whites living in counties with above-median evangelical share. The omitted quarter is -1 (July-September of 2016). Standard errors are clustered by county. *** 1%, ** 5%, * 10% significance level

### Figure A2: 2016 Presidential Election and Fertility in Democratic versus Republican Counties (Longer Pre-period)

- Extends Figure 1 panels A1–C1 to start in January 2015, and panels A2–C2 to start in quarter -7.
- **Panels A1, B1, C1 (top row):** raw monthly excess fertility by group. Y-axis: "Excess fertility". X-axis: 2015Apr–2018Oct. Two shaded bands mark the New Hampshire primary (January–February 2016, labeled "Trump presumptive nominee") and the presidential election (October–November 2016, labeled "Election").
- **Panels A2, B2, C2 (bottom row):** quarterly event-study coefficients with 95% confidence intervals. Y-axis: "Differential excess fertility". X-axis: "Quarters from election" (-7 to 8).
- Columns and legends as in Figure 1 (A: by vote share; B: by Republican shift; C: by vote share × Rep. shift).

**Note:** This figure extends Figure 1 panels A1 to C1 to start in January 2015, and extends panels A2 to C2 to start in quarter -7. The shaded areas, which account for partially treated months (see section 2.2), indicate the periods immediately surrounding the New Hampshire primary (January-February 2016) and the presidential election (October-November 2016). See note to Figure 1 for specifications.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### 3.2 Fertility Effects by Ethnicity

As a different measure of political partisanship, we compare Hispanics to non-Hispanics. This split is motivated by Trump's rhetoric towards the Hispanic population, beginning with his first campaign speech in which he compared Mexican immigrants to rapists and criminals. Moreover, Hispanics have historically backed Democratic candidates by a wide margin, voting two-to-one for Hillary Clinton in 2016.

Figure 2 plots excess fertility surrounding the 2016 election. Panel A1 shows similar pre-trends for Hispanic and non-Hispanic women. Following the election, non-Hispanic fertility rises for two months while that of Hispanics falls markedly over time; the gap between the two persists in every month in the post-election period. Panel A2 plots the quarterly regression estimates for equation 2; note that all identifying variation in this regression is within-county. There are no differential pre-trends, but there are large and consistent negative fertility effects. Corresponding quarterly estimates are reported in Table 1. Over the post-treatment period, the average quarterly effect is 0.325 fewer Hispanic versus non-Hispanic births per 1,000 women. This shift is equivalent to 2.3% of the U.S. 2015 birth rate.

Given the strong support for Trump among whites in rural areas, in column B we replace the control group with non-Hispanic whites in predominantly rural counties. Panel B1 shows an immediate and dramatic rise in rural non-Hispanic white fertility, contrasting sharply with the large drop in Hispanic fertility. Trump also had strong support from evangelical whites, so in column C we use counties with an above-median evangelical share as the control. These evangelical counties have weak correlation with rural counties (0.17), yet also exhibit strong differential fertility relative to Hispanics. Using these alternative comparison groups yields an average effect size which is roughly 50% larger.

Hispanics have a higher baseline fertility rate compared to non-Hispanics, rural whites, and evangelical whites. Trump's election victory narrowed the fertility gaps by 11, 27, and 20%, respectively.

### Figure 2: 2016 Presidential Election and Hispanic versus Non-Hispanic Fertility

- **Panels A1, B1, C1 (top row):** raw monthly excess fertility by group, normalized to September 2016. Y-axis: "Excess fertility". X-axis: 2016Apr–2018Oct. Shaded band: October–November 2016.
- **Panels A2, B2, C2 (bottom row):** quarterly event-study coefficients with 95% confidence intervals (equation 2). Y-axis: "Differential fertility rate". X-axis: "Quarters from election" (-3 to 8). Omitted quarter: -1.
- **Column A:** Hispanic vs non-Hispanic. Legend: "Hispanic" (solid), "Non-Hispanic" (dashed).
- **Column B:** Hispanic vs rural white. Legend: "Hispanic" (solid), "Rural white" (dashed).
- **Column C:** Hispanic vs evangelical white. Legend: "Hispanic" (solid), "Evangelical white" (dashed).

**Note:** See note to Figure 1. This figure plots effects (and 95% confidence intervals) for the excess fertility rate of Hispanics versus other groups around the 2016 presidential election. Panel A1 plots the excess fertility rate of Hispanics versus non-Hispanics; Panel B1 versus non-Hispanic whites living in rural counties (using the Census Bureau definition); Panel C1 versus non-Hispanic whites living in counties with above-median evangelical share (excluding historically Black protestant churches). The data is from the Association of Religion Data Archives. Panels A2 to C2 plot the interactions between quarters and an indicator for Hispanic ethnicity from equation 2. Specifications correspond to Table 1 columns (4) to (6).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred. (Corresponding regression estimates are in Table 1, columns 4–6.)

### 3.3 Results from the 2000 Presidential Election

To place our results in perspective, we examine the close election between George W. Bush and Al Gore in 2000. Bush barely won the election, with the Supreme Court determining the final outcome in December. During this election period, the level of polarization in U.S. politics and across candidates was substantially lower than in 2016 (Enke, 2020, Pew, 2014).

When we compare Republican to Democratic-leaning counties in Figure 3 we find some evidence that relative Democratic fertility falls, with an average quarterly effect of 0.087 births per 1,000 women (0.6% of the 1999 average birth rate). Bush had particularly strong support among evangelical voters (Niebuhr, 2000). Comparing counties with low and high evangelical shares, we also find sizable drops in relative fertility for less evangelical counties in the three quarters after the election (0.090 births per 1,000 women, or 0.6% of the average birth rate).[^10] Corresponding regression results are reported in Table A2.

[^10]: We limit the analysis to the three quarters post election because the NCHS began a staggered revision process for birth data collection starting in 2003 (NCHS, 2017). In Appendix Figure A5, we extend the pre-period, which is possible with this data.

Obama's 2008 election victory was not a surprise and the Great Recession confounds any analysis. However, for completeness we present results in Appendix Figure A6.

### Figure 3: 2000 Presidential Election and Fertility

- **Panels A1, B1 (top row):** raw monthly excess fertility by group, normalized to October 2000. Y-axis: "Excess fertility". X-axis: 2000Apr–2001Oct. Shaded band: November–December 2000 ("Election decided by court"). Panel A1 legend: "Democratic" (blue), "Republican" (red dashed). Panel B1 legend: "Low evangelical" (solid), "High evangelical" (dashed).
- **Panels A2, B2 (bottom row):** quarterly event-study coefficients with 95% confidence intervals (equation 1). Y-axis: "Differential excess fertility". X-axis: "Quarters from election" (-3 to 4). Omitted quarter: -1.

**Note:** This figure plots effects (and 95% confidence intervals) for the 2000 presidential election. Excess fertility rates in panels A1 and B1 are normalized to October 2000. The election was decided in December 2000 by the Supreme Court. As described in section 2.2, November represents a partially-treated month, so we shade November and December to indicate the onset of treatment. Panel A1 plots the excess fertility rate in counties with above-median versus below-median Democratic vote shares in the 1996 presidential election; Panel B1 counties with below-median versus above-median evangelical population share. Panels A2 and B2 plot the interactions between quarters and indicators for Democratic-leaning counties or evangelical counties (equation 1). The omitted quarter is -1 (August-October 2000). Specifications correspond to Table A2 columns (1) and (2).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred. (Corresponding regression estimates are in Table A2.)

### Table A2: 2000 Presidential Election and Fertility

- **Table type:** Regression (DID event study)
- **Dependent variable:** excess fertility rate
- **Standard errors:** clustered by county (reported in parentheses)
- **Omitted quarter:** -1 (August–October 2000)
- **Treatment group:** the first group named in each column header
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | comparison | partisanship_measure |
|---|---|---|
| 1 | Dem. vs Rep. | above- vs below-median Democratic vote share, 1996 election |
| 2 | Low vs high evangelical | below- vs above-median evangelical share |

#### Estimates

| variable | statistic | model_1 | model_2 |
|---|---|---:|---:|
| Treat−3 | coefficient | -0.089 | -0.055 |
| Treat−3 | standard_error | (0.057) | (0.061) |
| Treat−2 | coefficient | -0.038 | -0.054 |
| Treat−2 | standard_error | (0.052) | (0.053) |
| Treat0 | coefficient | -0.004 | -0.014 |
| Treat0 | standard_error | (0.048) | (0.052) |
| Treat1 | coefficient | -0.129** | -0.123** |
| Treat1 | standard_error | (0.058) | (0.059) |
| Treat2 | coefficient | -0.069 | -0.186** |
| Treat2 | standard_error | (0.066) | (0.072) |
| Treat3 | coefficient | -0.165** | -0.179** |
| Treat3 | standard_error | (0.065) | (0.080) |
| Treat4 | coefficient | -0.066 | 0.052 |
| Treat4 | standard_error | (0.053) | (0.061) |

#### Model statistics

| statistic | model_1 | model_2 |
|---|---:|---:|
| Avg. Treat (0 to 4) | -0.087 | -0.090 |
| 1999 avg. birth rate | 14.311 | 14.315 |
| Avg. Treat/1999 avg. | 0.6% | 0.6% |
| 1999 avg. Treat-Control gap | -.822 | -.357 |
| Avg. Treat/1999 avg. gap | 11% | 25% |
| Observations | 22,496 | 22,632 |
| R-squared | 0.487 | 0.487 |
| County FE | Y | Y |
| Quarter event FE | Y | Y |
| N cluster (counties) | 2,812 | 2,829 |

**Note:** This table reports the estimates depicted in panels A2 and B2 in Figure 3. The dependent variable is the excess fertility rate. The treatment group is the first group named in each column header. Columns (1) and (2) report interactions between quarters and a Democratic-leaning indicator from equation 1. Column (1) compares counties with above-median versus below-median Democratic vote shares in the 1996 Presidential election; column (2) counties with below-median versus above-median evangelical share. The omitted quarter is -1 (August-October 2000). Standard errors are clustered by county. *** 1%, ** 5%, * 10% significance level

### Figure A5: 2000 Presidential Election and Fertility (Longer Pre-period)

- Extends Figure 3 panels A1 and B1 to start in January 1999, and panels A2 and B2 to start in quarter -7.
- **Panels A1, B1 (top row):** raw monthly excess fertility, normalized to October 2000. Y-axis: "Excess fertility". X-axis: 1999Apr–2001Oct. Shaded band: November–December 2000 ("Election decided by court"). Legends as in Figure 3.
- **Panels A2, B2 (bottom row):** quarterly event-study coefficients with 95% confidence intervals. Y-axis: "Differential excess fertility". X-axis: "Quarters from election" (-7 to 4).

**Note:** This figure extends Figure 3 panels A1 and B1 to start in January 1999, and extends panels A2 and B2 to start in quarter -7. Excess fertility rates in panels A1 and B1 are normalized to October 2000. The election was decided in December 2000 by the Supreme Court. As described in section 2.2, November represents a partially-treated month, so we shade November and December to indicate the onset of treatment.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A6: 2008 Presidential Election and Fertility

- **Panels A1, B1 (top row):** raw monthly excess fertility by group, normalized to November 2007. Y-axis: "Excess fertility". X-axis: 2007Apr–2009Oct. Two shaded bands mark the Iowa Caucus (December 2007–January 2008, labeled "Obama presumptive nominee") and the presidential election (October–November 2008, labeled "Election"). Panel A1 legend: "Democratic" (blue), "Republican" (red dashed). Panel B1 legend: "Black" (solid), "Non-black" (dashed).
- **Panels A2, B2 (bottom row):** quarterly event-study coefficients with 95% confidence intervals. Y-axis: "Differential excess fertility" (A2) / "Differential fertility rate" (B2). X-axis: "Quarters from election" (-7 to 4). Omitted quarter: -4.

**Note:** This figure plots effects (and 95% confidence intervals) for the 2008 presidential election. Fertility rates in panels A1 and B1 are normalized to November 2007. Obama became the presumptive nominee after the Iowa Caucus. The shaded areas, which account for partially treated months (see section 2.2), indicate the periods immediately surrounding the Iowa Caucus (December 2007-January 2008) and the presidential election (October-November 2008). Panel A1 plots the excess fertility rate in counties with above-median versus below-median Democratic vote shares in the 2004 presidential election; Panel B1 the excess fertility rate for Black versus non-Black mothers (within county). Panels A2 and B2 plot the interactions between quarters and indicators for Democratic-leaning counties (equation 1) and Black mothers (equation 2). The omitted quarter is -4 (October-December 2007). Specifications mirror those in Table 1, columns (1) and (4).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### 3.4 Robustness

Appendix Table A3 provides robustness results for the 2016 election. Columns (1) to (6) conduct a mediation analysis, adding controls for county income, income squared, and 2-digit NAICS employment shares to the specifications used in Table 1. Columns (7) and (8) modify the vote share cutoffs and base year used for our two county partisanship measures. The resulting estimates are similar.

Column (9) replaces the Hispanic treatment group with Mexicans (the largest Hispanic group) and finds similar effects. While Trump targeted Hispanic immigration in particular, it is possible that African-American and other minorities' fertility was affected. However, as we show in column (10), we find limited evidence for this: there is a reduction in non-Hispanic minority versus white fertility in the first post election quarter, but no significant effect thereafter.

In Appendix Figures A2 and A3 we expand the time window to two years before the election so as to include the primary nominations. After Trump became the presumptive Republican nominee there was an immediate drop in relative Hispanic fertility.[^11] There is not a similar effect by partisan affiliation; this may reflect that Trump winning the nomination was viewed as, if anything, increasing the probability of a Democratic victory.

[^11]: We determine the timing using the Iowa Electronic Markets (RCONV16).

Next, we replace the dependent variable with the Google search index for the term "pregnancy test." Consistent with our main results, Appendix Table A4 shows that Democratic-leaning designated marketing areas (DMAs) and those with a high proportion of Hispanics both see relative declines in this search following the 2016 election.

As a final exercise, we explore whether more politically polarized counties experience larger effects. We take advantage of the arguably exogenous shock to local economic conditions caused by the China trade shock. Autor et al. (2020) show that trade-exposed counties became more polarized, both on the left and right of the political spectrum; we use their proxy for county-level polarization.

We create two interaction terms, multiplying $\beta_t$ in equation 2 with whether a county is above or below the median of the instrumented China trade shock of Autor et al. (2020). Results are plotted in Appendix Figure A4. The difference in the gap between Hispanics and non-Hispanics in more versus less polarized counties, summed over the nine quarters after the election, is statistically significant (p value = 0.005). The post-election percentage point difference between Hispanics and non-Hispanics is more than twice as large (214%) in more versus less polarized counties.

### Table A3: Robustness - 2016 Presidential Election and Fertility

- **Table type:** Regression (DID event study)
- **Dependent variable:** excess fertility rate
- **Standard errors:** clustered by county (reported in parentheses)
- **Omitted quarter:** -1 (July–September 2016)
- **Treatment group:** the first group named in each column header
- **Controls:** all columns add county income, income squared, and county monthly two-digit NAICS employment share (the "Income & industry share" row)
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | header | description |
|---|---|---|
| 1 | Dem. vs Rep. | Table 1 col 1 specification + income/industry controls |
| 2 | L vs H Rep. shift | Table 1 col 2 specification + income/industry controls |
| 3 | Share × shift | Table 1 col 3 specification + income/industry controls |
| 4 | HP vs non-HP | Table 1 col 4 specification + income/industry controls |
| 5 | HP vs rural WH | Table 1 col 5 specification + income/industry controls |
| 6 | HP vs evan. WH | Table 1 col 6 specification + income/industry controls |
| 7 | Dem. vs Rep. p60/p40 | partisanship = above 60th vs below 40th percentile of 2012 Democratic vote share |
| 8 | L vs H Rep. shift 12-16 | Republican vote-share shift measured 2012–2016 instead of 2008–2016 |
| 9 | Mexican vs non-HP | treatment group is Mexicans (largest Hispanic group) |
| 10 | Minority vs WH | non-Hispanic minorities vs non-Hispanic whites (WH) |

Abbreviations: HP = Hispanic; WH = white.

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 | model_10 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Treat−3 | coefficient | -0.038 | -0.064 | -0.092 | -0.051 | -0.010 | -0.062 | 0.004 | 0.016 | 0.039 | 0.025 |
| Treat−3 | standard_error | (0.061) | (0.061) | (0.094) | (0.059) | (0.088) | (0.075) | (0.072) | (0.061) | (0.094) | (0.074) |
| Treat−2 | coefficient | -0.017 | -0.081 | -0.105 | -0.061 | -0.071 | -0.101 | -0.003 | -0.022 | -0.051 | 0.083 |
| Treat−2 | standard_error | (0.055) | (0.058) | (0.090) | (0.050) | (0.083) | (0.069) | (0.061) | (0.056) | (0.070) | (0.055) |
| Treat0 | coefficient | -0.139** | -0.169*** | -0.267*** | -0.198*** | -0.249*** | -0.258*** | -0.123** | -0.172*** | -0.218*** | 0.045 |
| Treat0 | standard_error | (0.056) | (0.058) | (0.091) | (0.048) | (0.083) | (0.067) | (0.061) | (0.057) | (0.055) | (0.053) |
| Treat1 | coefficient | -0.098* | -0.198*** | -0.363*** | -0.275*** | -0.450*** | -0.379*** | -0.128** | -0.243*** | -0.315*** | -0.142** |
| Treat1 | standard_error | (0.059) | (0.061) | (0.087) | (0.055) | (0.087) | (0.072) | (0.063) | (0.063) | (0.066) | (0.056) |
| Treat2 | coefficient | -0.175*** | -0.297*** | -0.427*** | -0.312*** | -0.535*** | -0.430*** | -0.237*** | -0.267*** | -0.324*** | -0.087 |
| Treat2 | standard_error | (0.065) | (0.064) | (0.092) | (0.055) | (0.085) | (0.070) | (0.070) | (0.068) | (0.064) | (0.062) |
| Treat3 | coefficient | -0.165** | -0.299*** | -0.433*** | -0.318*** | -0.559*** | -0.478*** | -0.184** | -0.314*** | -0.355*** | -0.042 |
| Treat3 | standard_error | (0.073) | (0.071) | (0.102) | (0.057) | (0.094) | (0.082) | (0.083) | (0.074) | (0.066) | (0.065) |
| Treat4 | coefficient | -0.121* | -0.282*** | -0.329*** | -0.340*** | -0.524*** | -0.487*** | -0.159** | -0.356*** | -0.264*** | -0.262*** |
| Treat4 | standard_error | (0.071) | (0.069) | (0.097) | (0.064) | (0.097) | (0.087) | (0.078) | (0.072) | (0.071) | (0.069) |
| Treat5 | coefficient | -0.136** | -0.336*** | -0.469*** | -0.356*** | -0.657*** | -0.546*** | -0.195** | -0.346*** | -0.145* | -0.422*** |
| Treat5 | standard_error | (0.068) | (0.067) | (0.097) | (0.061) | (0.100) | (0.088) | (0.076) | (0.066) | (0.085) | (0.067) |
| Treat6 | coefficient | -0.157** | -0.281*** | -0.383*** | -0.402*** | -0.616*** | -0.590*** | -0.195*** | -0.290*** | -0.040 | -0.242*** |
| Treat6 | standard_error | (0.066) | (0.067) | (0.096) | (0.067) | (0.101) | (0.089) | (0.071) | (0.065) | (0.114) | (0.068) |
| Treat7 | coefficient | -0.199** | -0.414*** | -0.555*** | -0.366*** | -0.683*** | -0.552*** | -0.250*** | -0.470*** | 0.019 | -0.201*** |
| Treat7 | standard_error | (0.079) | (0.074) | (0.102) | (0.076) | (0.108) | (0.098) | (0.088) | (0.075) | (0.176) | (0.069) |
| Treat8 | coefficient | -0.234*** | -0.411*** | -0.530*** | -0.338*** | -0.643*** | -0.543*** | -0.309*** | -0.516*** | -0.011 | -0.222*** |
| Treat8 | standard_error | (0.080) | (0.075) | (0.105) | (0.097) | (0.128) | (0.120) | (0.091) | (0.076) | (0.212) | (0.076) |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 | model_10 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Avg. Treat (0 to 8) | -0.158 | -0.299 | -0.417 | -0.323 | -0.546 | -0.474 | -0.198 | -0.331 | -0.184 | -0.175 |
| 2015 avg. birth rate | 14.007 | 14.007 | 13.878 | 13.896 | 15.701 | 15.221 | 13.887 | 14.007 | 13.518 | 13.612 |
| Avg. Treat/2015 avg. | -1.1% | -2.1% | -3.0% | -2.3% | -3.5% | -3.1% | -1.4% | -2.4% | -1.4% | -1.3% |
| 2015 avg. Treat-Control gap | -1.018 | -.181 | -.848 | 2.994 | 1.925 | 2.308 | -1.156 | .092 | 1.627 | 1.169 |
| Avg. Treat/2015 avg. gap | 16% | 165% | 49% | -11% | -28% | -21% | 17% | -359% | -11% | -15% |
| Observations | 33,744 | 33,744 | 19,596 | 67,896 | 53,028 | 50,892 | 27,000 | 33,756 | 67,692 | 67,920 |
| R-squared | 0.369 | 0.370 | 0.397 | 0.315 | 0.248 | 0.273 | 0.372 | 0.370 | 0.290 | 0.269 |
| County FE | Y | Y | Y | N | N | N | Y | Y | N | N |
| County × ethnicity FE | N | N | N | Y | Y | Y | N | N | Y | Y |
| Quarter event FE | Y | Y | Y | Y | Y | Y | Y | Y | Y | Y |
| Income & industry share | Y | Y | Y | Y | Y | Y | Y | Y | Y | Y |
| N clusters (counties) | 2,812 | 2,812 | 1,633 | 2,829 | 2,829 | 2,829 | 2,250 | 2,813 | 2,830 | 2,830 |

**Note:** Columns (1) to (6) parallel the specifications in Table 1 but add controls for county income, income squared, and county monthly two-digit NAICS employment share. The treatment group is the first group named in each column header. Column (7) categorizes county partisanship by whether they are above the 60th or below the 40th percentile in the 2012 Democratic vote share. Column (8) uses the shift in Republican vote share between 2012-2016 instead of 2008-2016. Column (9) replaces Hispanics (HP) as the treatment group with Mexicans, while column (10) compares non-Hispanic minorities to non-Hispanic whites (WH). The omitted quarter is -1 (July-September 2016). Standard errors are clustered by county. *** 1%, ** 5%, * 10% significance level

### Figure A3: 2016 Presidential Election and Hispanic versus Non-Hispanic Fertility (Longer Pre-period)

- Extends Figure 2 panels A1–C1 to start in January 2015, and panels A2–C2 to start in quarter -7.
- **Panels A1, B1, C1 (top row):** raw monthly excess fertility by group. Y-axis: "Excess fertility". X-axis: 2015Apr–2018Oct. Two shaded bands mark the New Hampshire primary (January–February 2016, "Trump presumptive nominee") and the election (October–November 2016, "Election").
- **Panels A2, B2, C2 (bottom row):** quarterly event-study coefficients with 95% confidence intervals. Y-axis: "Differential fertility rate". X-axis: "Quarters from election" (-7 to 8).
- Columns and legends as in Figure 2 (A: vs non-Hispanic; B: vs rural white; C: vs evangelical white).

**Note:** This figure extends Figure 2 panels A1 to C1 to start in January 2015 and extends panels A2 to C2 to start in quarter -7. The shaded areas, which account for partially treated months (see section 2.2), indicate the periods immediately surrounding the New Hampshire primary (January-February 2016) and the presidential election (October-November 2016). See note to Figure 2 for specifications.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Table A4: 2016 Presidential Election and Google Searches for "Pregnancy Test"

- **Table type:** Regression (DID event study)
- **Dependent variable:** weekly percentage of Google searches for "pregnancy test" (from a random sample of total searches, scaled by the highest weekly search rate in the same DMA over the entire extraction period; averaged across 15 extractions taken November 2020–January 2021)
- **Unit of observation:** DMA × quarter
- **Standard errors:** clustered by DMA (reported in parentheses)
- **Omitted quarter:** -1 (July–September 2016)
- **Treatment group:** the first group named in each column header
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | header | treatment_indicator |
|---|---|---|
| 1 | Dem. vs Rep. | DMA above-median Democratic vote share in 2012 |
| 2 | Low vs high Rep. shift | DMA below-median change in Republican vote share, 2012–2016 |
| 3 | High vs low Hisp. | DMA above-median Hispanic population percentage |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 |
|---|---|---:|---:|---:|
| Treat−3 | coefficient | -3.587 | 0.628 | 3.322 |
| Treat−3 | standard_error | (3.483) | (3.114) | (2.851) |
| Treat−2 | coefficient | -2.514 | -0.226 | -0.155 |
| Treat−2 | standard_error | (2.842) | (2.925) | (2.648) |
| Treat0 | coefficient | -5.709* | -7.443*** | -6.320** |
| Treat0 | standard_error | (2.899) | (2.818) | (2.813) |
| Treat1 | coefficient | -3.589 | -6.193** | -5.425* |
| Treat1 | standard_error | (3.109) | (2.683) | (2.834) |
| Treat2 | coefficient | -1.992 | -2.560 | -2.241 |
| Treat2 | standard_error | (3.506) | (3.253) | (3.235) |
| Treat3 | coefficient | -0.424 | -5.333 | -4.427 |
| Treat3 | standard_error | (4.146) | (3.604) | (3.485) |

#### Model statistics

| statistic | model_1 | model_2 | model_3 |
|---|---:|---:|---:|
| Sum Treat (0 to 3) | -11.714 | -21.529 | -18.413 |
| p value | 0.343 | 0.048 | 0.086 |
| Observations | 1,435 | 1,435 | 1,456 |
| R-squared | 0.490 | 0.497 | 0.498 |
| DMA FE | Y | Y | Y |
| Quarter event FE | Y | Y | Y |
| N clusters (DMAs) | 201 | 201 | 203 |

**Note:** This table reports the effects of the 2016 Presidential election on Google searches for "pregnancy test." The dependent variable is the weekly percentage of Google searches taken from a random sample of total searches and scaled by the highest weekly search rate in the same DMA during the entire extraction period. The treatment group is the first group named in each column header. Since each extraction is based on a random sample, we use the average Google search rate across 15 extractions taken between November 2020 and January 2021 as our outcome. Columns (1) through (3) report interactions between quarters and an indicator for DMAs having above-median Democratic vote shares in the 2012 election, an indicator for DMAs having an below-median change in Republican vote share from the 2012 to the 2016 election, and an indicator for having above-median Hispanic population percentage, respectively. The omitted quarter is -1 (July-September 2016). Standard errors are clustered by DMA. *** 1%, ** 5%, * 10% significance level

### Figure A4: 2016 Presidential Election and Fertility in More versus Less Polarized Counties

- Plots heterogeneous quarterly event-study effects (with 95% confidence intervals) on the excess fertility rate of Hispanic versus non-Hispanic women, split by county polarization.
- Y-axis: "Differential fertility rate". X-axis: "Quarters from election" (-3 to 8). Omitted quarter: -1.
- Legend: "More polarized" (solid), "Less polarized" (dashed). Coefficients are slightly staggered for visual clarity.

**Note:** This figure plots heterogeneous effects (and 95% confidence intervals) of the 2016 presidential election on the excess fertility rate among Hispanic versus non-Hispanic women in more versus less polarized counties. A county is defined as more polarized if the county experienced an above-median level of instrumented China trade shock between 2000 and 2008 following Autor et al. (2020). The omitted quarter is -1 (July-September 2016). The specification is described in section 3.4. Coefficients are slightly staggered for visual clarity.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

## 4. Mechanisms

This section considers possible mechanisms for the effect of Trump's victory on fertility. We recognize that multiple forces could be in play simultaneously and discuss several below. There could also be differential changes along other dimensions, such as the composition of migrants (e.g., Pew, 2019a), within-household dynamics due to the gender gap in voting (since women favor Democratic candidates, e.g., CAWP (2020)), and misinformation in a polarized environment (e.g., Allcott and Gentzkow, 2017).

#### Policy changes

Democrats and Republicans favor different policies, and when presidential regime shifts occur, policies change. According to a 2018 Pew survey, the top three issues for Republicans – reducing undocumented immigration, cutting the national debt, and avoiding tax increases – do not overlap with those of Democrats (Pew, 2019b). Likewise, three of the top five Democrat priorities (dealing with climate change, reducing inequality, and increasing spending on Social Security, Medicare and Medicaid) are not in the Republican top five. This divergence in policy priorities, coupled with a shift in control of the executive branch, could lead to changes in family size decisions. Among young adults who had or expected to have fewer children than their ideal number, a large fraction cite reasons which could be affected by policy (NYT, 2018). The top reason is the cost of childcare (64%), followed closely by a lack of family leave (39%). Additionally, respondents cite worries about domestic politics (36%), climate change (33%), and global instability (37%) as reasons for not having children. This suggests that either actual or expected policy changes could drive differential partisan fertility.[^12]

[^12]: Supreme Court nominations from Trump could also have been pivotal for reproductive rights and the possible repeal of the ACA.

Immigration policy could be especially salient for Hispanics, since it is an important point of divergence between the two parties. To examine whether the Democratic versus Republican results are driven by Hispanic fertility, we exclude Hispanic births, and continue to find sizeable effects.[^13] So, while changes to immigration policy may reduce relative Hispanic fertility, this cannot be the only explanation for the county-level political party results.[^14]

[^13]: The new coefficients summed over the post-election period are 52, 84, and 85 percent of the estimates in columns (1) to (3) in Table 1, respectively.

[^14]: A related mechanism for the Hispanic effect is that newly arrived immigrants have higher fertility, and Hispanic immigration fell after Trump's victory. However, this does not explain the rise in fertility for rural whites and evangelical whites or our results for Republican counties.

#### Economic optimism

Another possible mechanism is that fertility responds to changes in economic optimism.[^15] As documented in the literature, partisans of the winning side in a presidential election become more optimistic about the direction of the economy (Bartels, 2002, Evans and Andersen, 2006, Mian et al., 2021). Appendix Figure A1 plots the percentage of positive minus negative responses (labeled "net better") to the question "Do you think the nation's economy is getting better or worse?" Republican voters became immediately more optimistic following Trump's election, with the net better fraction rising from -63 to +63% over four months. In contrast, for Democrats this falls from +52 to -4%, after which it continues to erode. Similar swings in optimism, but in the opposite direction, occurred after the 2020 presidential election.

[^15]: Shifts in optimism may reflect general expectations, or beliefs about specific policies that could economically impact an individual's group. For example, the TCJA capped the SALT tax deduction, disproportionately impacting voters in Democratic states.

The partisan patterns in optimism, where Republicans' economic outlook improved almost instantly post election, while Democrats' sentiment worsened much more gradually, line up with the dynamics we find for fertility. One interpretation is that fertility responds to people's perceptions about the direction of the economy: Democrats were worried after the election, and their worldview worsened steadily throughout the Trump administration.

### Figure A1: Economic Outlook by Party Affiliation

- Plots the percentage of positive minus negative responses ("net better") to the question "Do you think the nation's economy is getting better or worse?" among registered voters.
- Y-axis: "Net better (%)". X-axis: monthly, 2016Jan–2021Jul. Vertical reference lines mark the 2016 Election, the COVID Stock Crash, and the 2020 Election.
- Legend: "Democrat" (blue solid), "Republican" (red dashed).

**Note:** This figure plots the percentage of positive minus negative responses ("net better") to the question "Do you think the nation's economy is getting better or worse?" among registered voters. The survey is administered by CIVIQS, which uses a list-based sampling methodology to select panelists to receive online polls. They use dynamic Bayesian multilevel regression with post-stratification weights to adjust the demographics of the sample to those of the U.S. population and to smooth out day-to-day sampling variability.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

#### Updating beliefs about the political and social climate

We examine Trump's pre-election campaign visits to provide additional insight into possible mechanisms. Individuals may update their probabilities of a Trump victory when he makes a campaign stop, affecting both expected policy and economic optimism. However, after the Iowa prediction market reveals Trump as the clear favorite to win the nomination in February 2016, the market's probability of a Democratic victory in the election begins a rising trend. This suggests that Republicans should become less optimistic about future policy and economic conditions, and so reduce their fertility (and vice versa for Democrats).

A mechanism that predicts an opposite-signed effect is that campaign stops cause people to update their view of other Americans' values. Views about the political and social climate could affect individuals' willingness to bring a child into the world, even absent a policy channel. In particular, Trump rallies could lead Republicans to think their worldview has broader local support than they previously believed. Likewise, this could be a surprise to Democrats. We can test this for Hispanics, who are disproportionately Democratic voters. When a Hispanic couple sees the enthusiasm generated by Trump's visit and his anti-immigrant rhetoric, they might update beliefs about their acceptance in the community.

To test this, we use Trump's campaign visits, which attracted local attention, as indicated by spikes in Google searches (see Appendix Figure A7). We use a triple DID dynamic event study comparing fertility between Hispanic and non-Hispanic females in counties before and after Trump's first visit, using counties he will visit later as controls (see Sun and Abraham (2020); implementation details are in Appendix 1). The dynamic event study design accounts for potential heterogeneous effects across counties visited at different times as Trump's campaign strategy and rhetoric evolved.

Figure 4 plots the estimated treatment effects; corresponding regression estimates are in Appendix Table A5. The Hispanic fertility rate relative to non-Hispanics in the same county starts to decrease in month -1, which is when partial treatment of mothers begins, and continues through month 2. By month 4 differential fertility has dissipated, with suggestive evidence of harvesting in month 5. Following a campaign visit, the monthly average fertility rate for Hispanics falls relative to non-Hispanics by 1.5% of the mean.

A similar updating process at a more aggregate level could contribute to our national fertility results for Hispanics. Updating could also occur for non-Hispanics, as they revise their view of the political climate (including immigration policy, but also on other dimensions), but we cannot identify Republicans and Democrats at the individual level in fertility data.

### Figure 4: Trump Campaign Visits and Relative Hispanic Fertility

- Plots dynamic event-study coefficients (with 95% confidence intervals) from the triple-difference design.
- Y-axis: "Differential excess fertility". X-axis: "Month of last menstrual period from 1st Trump visit" (-7 to 5). Shaded band: months -1 and 0 (onset of treatment). Omitted period: month -3.

**Note:** This figure plots dynamic event study coefficients (and 95% confidence intervals) that compare fertility between Hispanic and non-Hispanic females (difference 1), in counties visited by Trump before and after his first campaign visit (difference 2), using counties he will visit later as controls (difference 3). Month -1 represents a partially-treated month, so we shade both months -1 and 0 to indicate the onset of treatment. The omitted period is month -3. See Appendix 1 for further implementation details; the specification corresponds to Table A5 column (1).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred. (Corresponding regression estimates are in Table A5, column 1.)

### Table A5: Trump Campaign Visits and Relative Hispanic Fertility

- **Table type:** Regression (triple-difference dynamic event study)
- **Dependent variable:** fertility rate (excess fertility for ethnicity group × county × month)
- **Standard errors:** clustered by county (reported in parentheses); computed via the delta method (see Appendix 1)
- **Omitted period:** -3 (month of last menstrual period relative to first Trump visit)
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | header | aggregation_weight |
|---|---|---|
| 1 | Baseline | Hispanic female population in treated counties |
| 2 | Alternative weight | total female population in treated counties |

#### Estimates

| variable | statistic | model_1 | model_2 |
|---|---|---:|---:|
| Treat−7M | coefficient | -0.021 | -0.068 |
| Treat−7M | standard_error | (0.055) | (0.062) |
| Treat−6M | coefficient | -0.018 | -0.070 |
| Treat−6M | standard_error | (0.053) | (0.062) |
| Treat−5M | coefficient | 0.031 | 0.047 |
| Treat−5M | standard_error | (0.050) | (0.062) |
| Treat−4M | coefficient | -0.040 | -0.018 |
| Treat−4M | standard_error | (0.053) | (0.063) |
| Treat−2M | coefficient | 0.040 | 0.042 |
| Treat−2M | standard_error | (0.051) | (0.058) |
| Treat−1M | coefficient | -0.127*** | -0.108* |
| Treat−1M | standard_error | (0.048) | (0.059) |
| Treat0M | coefficient | -0.093 | -0.073 |
| Treat0M | standard_error | (0.065) | (0.068) |
| Treat1M | coefficient | -0.166*** | -0.154** |
| Treat1M | standard_error | (0.056) | (0.069) |
| Treat2M | coefficient | -0.177** | -0.157* |
| Treat2M | standard_error | (0.077) | (0.083) |
| Treat3M | coefficient | -0.060 | -0.029 |
| Treat3M | standard_error | (0.077) | (0.091) |
| Treat4M | coefficient | -0.004 | 0.009 |
| Treat4M | standard_error | (0.083) | (0.087) |
| Treat5M | coefficient | 0.140 | 0.123 |
| Treat5M | standard_error | (0.100) | (0.110) |

#### Model statistics

| statistic | model_1 | model_2 |
|---|---:|---:|
| Observations | 129,872 | 129,872 |
| R-squared | 0.412 | 0.412 |
| Outcome mean | 4.540 | 4.540 |
| N clusters (counties) | 230 | 230 |

**Note:** This table presents dynamic event study coefficients that compare fertility between Hispanic and non-Hispanic females (difference 1), in counties visited by Trump before and after his first campaign visit (difference 2), using counties he will visit later as controls (difference 3). The omitted period is -3. Column (1) uses the Hispanic female population in treated counties as the aggregation weight, while column (2) uses the total female population in treated counties. See Appendix 1 for implementation details; the specification corresponds to Figure 4.

### Figure A7: Google Search Index for "Trump" around Campaign Visits

- Plots dynamic treatment effects (with 95% confidence intervals) for Trump's first campaign visit to a DMA on the weekly Google search index for "Trump", relative to DMAs with later visits.
- Y-axis: "Differential Google searches for Trump". X-axis: "Weeks from 1st Trump visit" (-9 to 9). Omitted period: -3.

**Note:** This figure plots dynamic treatment effects (and 95% confidence intervals) for Trump's first campaign visit to a Designated Market Area (DMA) on the weekly Google search index for "Trump" relative to DMAs with later visits (the omitted period is -3). This figure shows that the Google search index for "Trump" starts to rise about two weeks before Trump's first campaign visit to a DMA, peaking in the week of the visit.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

## 5. Conclusion

This paper documents a new consequence of elections and a new determinant of fertility. We are the first to causally link political partisanship to fertility choices. Unlike many household decisions, this is a long-term commitment, requiring significant time and money. We compare Republican to Democratic-leaning counties, before and after the 2016 presidential election. We find a change in fertility rates between Democratic and Republican counties amounting to 1.2 to 2.2% of the overall U.S. fertility rate. We likewise find a disparate and negative impact on relative Hispanic fertility (2.3 to 3.3% of the fertility rate).

The larger effects we find as the intensity of partisanship increases point towards political sentiment driving these effects. Several partisan mechanisms could be at work, including changes to expected and actual policy, economic optimism, and beliefs about the political and social climate. In other words, our findings could be due to affordability concerns, but also the quality of a potential child's life.

With an additional assumption about the counterfactual trend (see footnote 9), we estimate that Trump's victory led to over 7,000 additional births in Republican counties and 38,000 fewer Democratic births over nine quarters. Using our alternative measure based on the rightward vote shift instead of the vote share, we estimate 18,000 more Republican and 48,000 fewer Democratic births. The net effect using either measure is a drop of approximately 31,000 births, which can account for 20% of the decline in births over this period. A similar exercise focused on Hispanic fertility yields 10,000 fewer Hispanic births, corresponding to 37% of this group's decline post election. A caveat of estimating group-specific fertility is that we cannot difference out common time-varying factors, as we can with our DID estimates.

Growing political polarization and declining fertility are two challenges facing society. By estimating effects at the intersection of the two, this paper opens up several avenues for future research. These include disentangling mechanisms, the role of partisanship in interpreting information and in selective exposure, and whether growing polarization amplifies partisan effects on household decisions.

## References

Aizer, A., Eli, S., and Lleras-Muney, A. (2020). The incentive effects of cash transfers to the poor. NBER Working Paper.

Allcott, H., Boxell, L., Conway, J., Gentzkow, M., Thaler, M., and Yang, D. (2020). Polarization and public health: Partisan differences in social distancing during the coronavirus pandemic. Journal of Public Economics, 191:104254.

Allcott, H. and Gentzkow, M. (2017). Social media and fake news in the 2016 election. Journal of Economic Perspectives, 31(2):211–36.

Autor, D., Dorn, D., Hanson, G., et al. (2019). When work disappears: Manufacturing decline and the falling marriage market value of young men. American Economic Review: Insights, 1(2):161–78.

Autor, D., Dorn, D., Hanson, G., Majlesi, K., et al. (2020). Importing political polarization? The electoral consequences of rising trade exposure. American Economic Review, 110(10):3139–83.

Bailey, M. J. (2010). "Momma's got the pill": How Anthony Comstock and Griswold v. Connecticut shaped US childbearing. American Economic Review, 100(1):98–129.

Bartels, L. M. (2002). Beyond the running tally: Partisan bias in political perceptions. Political Behavior, 24(2):117–150.

Becker, G. S. (1960). An economic analysis of fertility. In Demographic and Economic Change in Developed Countries, pages 209–240. Columbia University Press.

Benhabib, J. and Spiegel, M. M. (2019). Sentiments and economic activity: Evidence from US states. The Economic Journal, 129(618):715–733.

Bernstein, A., Billings, S. B., Gustafson, M. T., and Lewis, R. (2021). Partisan residential sorting on climate change risk. Working Paper.

Bertrand, M. and Kamenica, E. (2018). Coming apart? Cultural distances in the United States over time. NBER Working Paper.

Black, D. A., Kolesnikova, N., Sanders, S. G., and Taylor, L. J. (2013). Are children "normal"? The Review of Economics and Statistics, 95(1):21–33.

Boxell, L., Gentzkow, M., and Shapiro, J. M. (2020). Cross-country trends in affective polarization. NBER Working Paper.

Brown, J. R. and Enos, R. D. (2021). The measurement of partisan sorting for 180 million voters. Nature Human Behaviour, pages 1–11.

Buckles, K., Guldi, M. E., and Schmidt, L. (2019). Fertility trends in the United States, 1980-2017: The role of unintended births. NBER Working Paper.

Buckles, K., Hungerman, D., and Lugauer, S. (2021). Is fertility a leading economic indicator? The Economic Journal, 131(634):541–565.

CAWP (2020). Center for American Women and Politics, The gender gap: Presidential vote choice.

Chen, M. K., Zhuo, Y., de la Fuente, M., Rohla, R., and Long, E. F. (2020). Causal estimation of stay-at-home orders on SARS-CoV-2 transmission. Working Paper.

Cohen, A., Dehejia, R., and Romanov, D. (2013). Financial incentives and fertility. Review of Economics and Statistics, 95(1):1–20.

Confessore, N. and Cohn, N. (2016). Donald Trump's victory was built on unique coalition of white voters. New York Times, November 9, 2016.

Cookson, J. A., Engelberg, J. E., and Mullins, W. (2020). Does partisanship shape investor beliefs? Evidence from the COVID-19 pandemic. The Review of Asset Pricing Studies, 10(4):863–893.

Cullen, J. B., Turner, N., and Washington, E. L. (2021). Political alignment, attitudes toward government and tax evasion. American Economic Journal: Economic Policy, (Forthcoming).

Currie, J. and Schwandt, H. (2014). Short-and long-term effects of unemployment on fertility. Proceedings of the National Academy of Sciences, 111(41):14734–14739.

Dagostino, R., Gao, J., and Ma, P. (2020). Partisanship in loan pricing. Working Paper.

Dehejia, R. and Lleras-Muney, A. (2004). Booms, busts, and babies' health. The Quarterly Journal of Economics, 119(3):1091–1130.

Dettling, L. J. and Kearney, M. S. (2014). House prices and birth rates: The impact of the real estate market on the decision to have a baby. Journal of Public Economics, 110:82–100.

Duncan, B., Mansour, H., and Rees, D. I. (2017). It's just a game: The Super Bowl and low birth weight. Journal of Human Resources, 52(4):946–978.

Enke, B. (2020). Moral values and voting. Journal of Political Economy, 128(10):3679–3729.

Evans, G. and Andersen, R. (2006). The political conditioning of economic perceptions. The Journal of Politics, 68(1):194–207.

Fridman, A., Gershon, R., and Gneezy, A. (2021). Covid-19 and vaccine hesitancy: A longitudinal study. PloS one, 16(4):e0250123.

Gallup (2017). Americans' satisfaction with U.S. same in 2017 as in 2016.

Gentzkow, M. (2016). Polarization in 2016. Working Paper.

Gerber, A. S. and Huber, G. A. (2009). Partisanship and economic behavior: Do partisan differences in economic forecasts predict real economic behavior? American Political Science Review, pages 407–426.

Gillitzer, C. and Prasad, N. (2018). The effect of consumer sentiment on consumption: Cross-sectional evidence from elections. American Economic Journal: Macroeconomics, 10(4):234–69.

Goldmacher, S. (2021). New York loses house seat after coming up 89 people short on Census. New York Times, April 26, 2021.

Grossman, G., Kim, S., Rexer, J. M., and Thirumurthy, H. (2020). Political partisanship influences behavioral responses to governors' recommendations for COVID-19 prevention in the United States. Proceedings of the National Academy of Sciences, 117(39):24144–24153.

Hungerman, D., Rinz, K., Weninger, T., and Yoon, C. (2018). Political campaigns and church contributions. Journal of Economic Behavior & Organization, 155:403–426.

Jones, C. I. (2020). The end of economic growth? Unintended consequences of a declining population. NBER Working Paper.

Kaplan, E., Spenkuch, J., and Sullivan, R. (2020). Partisan spatial sorting in the United States: A theoretical and empirical overview. Working Paper.

Kearney, M. and Levine, P. (2021). Will births in the US rebound? Probably not. Brookings.

Kearney, M. S., Levine, P., and Pardue, L. (2021). Why is the birth rate falling in the United States? Journal of Economic Perspectives, (Forthcoming).

Kearney, M. S. and Levine, P. B. (2009). Subsidized contraception, fertility, and sexual behavior. The Review of Economics and Statistics, 91(1):137–151.

Kempf, E. and Tsoutsoura, M. (2020). Partisan professionals: Evidence from credit rating analysts. NBER Working Paper.

Langer, A. and Lemoine, D. (2020). What were the odds? Estimating the market's probability of uncertain events. NBER Working Paper.

Lindo, J. M. (2010). Are children really inferior goods? Evidence from displacement-driven income shocks. Journal of Human Resources, 45(2):301–327.

Lino, M. (2020). The cost of raising a child. U.S. Department of Agriculture.

Lovenheim, M. F. and Mumford, K. J. (2013). Do family wealth shocks affect fertility choices? Evidence from the housing market. Review of Economics and Statistics, 95(2):464–475.

McCrary, J. and Royer, H. (2011). The effect of female education on fertility and infant health: Evidence from school entry policies using exact date of birth. American Economic Review, 101(1):158–95.

McGrath, M. C. (2017). Economic behavior and the partisan perceptual screen. Quarterly Journal of Political Science, 11(4):363–83.

Meeuwis, M., Parker, J. A., Schoar, A., and Simester, D. I. (2021). Belief disagreement and portfolio choice. Working Paper.

Mian, A. R., Sufi, A., and Khoshkhou, N. (2021). Partisan bias, economic expectations, and household spending. The Review of Economics and Statistics, (Forthcoming).

Milligan, K. (2005). Subsidizing the stork: New evidence on tax incentives and fertility. Review of Economics and Statistics, 87(3):539–555.

NCHS (2017). Revisions of the U.S. standard certificates and reports.

Niebuhr, G. (2000). The 2000 campaign: The Christian right; Evangelicals found a believer in Bush. New York Times, February 21, 2000.

Novgorodsky, D. and Setzler, B. (2019). Practical guide to event studies.

NYT (2018). Americans are having fewer babies. They told us why.

Pew (2014). Political polarization in the American public. Pew Research Center Report.

Pew (2019a). Facts on Latinos in the U.S.

Pew (2019b). Looking to the future, public sees an America in decline on many fronts.

Pew (2020). America is exceptional in the nature of its political divide. Pew Research Center Report.

Phillips, A. (2017). 'They're rapists.' President Trump's campaign launch speech two years later, annotated. Washington Post, June 16, 2017.

Raute, A. (2019). Can financial incentives reduce the baby gap? Evidence from a reform in maternity leave benefits. Journal of Public Economics, 169:203–222.

Schaller, J. (2016). Booms, busts, and fertility testing the Becker model using gender-specific labor demand. Journal of Human Resources, 51(1):1–29.

Sun, L. and Abraham, S. (2020). Estimating dynamic treatment effects in event studies with heterogeneous treatment effects. Journal of Econometrics.

## Appendix 1. Implementation for Pre-Election Campaign Visits

We collect Trump's campaign visits between January 2015 and November 2016 from the National Journal's Travel Tracker.[^A1] The data contains date, time, and city information for each visit. We map city names to county. Trump visited a total of 230 counties during his campaign; the mean and variance of these counties' fertility are reported in Table A1.

[^A1]: Original footnote 1 (Appendix). Travel Tracker compiles information from candidates' public campaign schedules and excludes events that candidates hold in their home states. This data is similar to that collected by Hungerman et al. (2018).

While we have the actual date of Trump's campaign visit, the natality data only records the month of the first day of a mother's last menstrual period (MLMP). This means that women whose menses occur in the second half of the month preceding a visit may be fertile when a visit occurs. Likewise, women whose menses begin in the month of a visit may not be fertile until the following month. This implies that women whose MLMP is in month -1 can also be treated by Trump's campaign visit. Similarly, women whose MLMP is in month 0 may not have been treated.[^A2]

[^A2]: Original footnote 2 (Appendix). The predicted percentage of fertile days in the month of a campaign visit (month 0) for women whose MLMP occurs in month -1, is approximately two thirds that of women whose MLMP occurs in month 0. This calculation assumes a uniform distribution of conception dates and visits throughout a month. Moreover, Google searches in Figure A7 suggest some anticipation of the campaign visit. Including anticipation would increase the percentage of fertile days for women whose MLMP occurs in month -1 to over 90% that of women whose MLMP occurs in month 0.

We use a triple DID dynamic event study comparing fertility between Hispanic and non-Hispanic females in counties before and after Trump's first visit, using counties he will visit later as controls. We focus on Trump's first campaign visit to a county so as not to contaminate our estimate with the effects from prior visits. We use counties that Trump will visit in the future as controls, rather than counties he will never visit, because unvisited counties are considerably different. To implement the dynamic event study we stack our panel data as a series of 4×2 matrices (Hispanics/non-Hispanics in treatment/control counties × pre/post), and adapt the R package from Novgorodsky and Setzler (2019) to allow the triple difference.

We define counties visited in month $g$ as cohort $g$ and cohort-specific event time in calendar month $m$ as $e_g = m - g$. We run the following regression:

$$
\begin{aligned}
Y_{kcm} = \sum_{g \in G} \mathbb{1}\{cohort = g\} * \Big\{ &\sum_{e \neq -3} \beta^{H}_{eg} * Hispanic_k * Treat_{c,g} * \mathbb{1}\{e = m-g\} \\
&+ \sum_{e \neq -3} \beta^{T}_{eg} * Treat_{c,g} * \mathbb{1}\{e = m-g\} + \sum_{e \neq -3} \gamma_{eg} * Hispanic_k * \mathbb{1}\{e = m-g\} \\
&+ \sum_{e \neq -3} \delta_{eg} * \mathbb{1}\{e = m-g\} + \delta_g * Hispanic_k * Treat_{c,g} + \pi_g * Treat_{c,g} \Big\} + \epsilon_{kcm},
\end{aligned}
\tag{3}
$$

where $Y_{kcm}$ is the fertility rate among women in ethnicity group $k$ in county $c$ in month $m$. $G$ is the set of all months that Trump had any campaign visits. $Hispanic_k$ is one if the ethnicity is Hispanic, and zero otherwise. $Treat_{c,g}$ is one if county $c$ belongs to cohort $g$ and when cohort $g$ is the treatment cohort (i.e., when $\mathbb{1}\{cohort = g\} = 1$). We define the omitted period as month -3, because women whose MLMP occurs in month -1 may also be treated, and to allow for potential anticipation one month before the actual visit.

Under the assumption that earlier visited and later visited counties share similar fertility trends absent Trump campaign visits, we can identify the treatment effect on the fertility of Hispanics versus others in treated cohort $g$ in event time $e_g$, which we label as $\beta^{H}_{eg}$. Following Sun and Abraham (2020), we define the average treatment effect for event time $e$ as:

$$\beta^{H}_e = \sum_{g \in G} \beta^{H}_{eg} \times w_g \tag{4}$$

where $w_g$ (the aggregation weight) is the Hispanic female population in counties belonging to cohort $g$. For robustness, we also use the total female population in cohort $g$ as $w_g$, and results are similar. We calculate clustered standard errors for $\beta^{H}_e$ via the delta method.

All counties in our sample experience their first Trump visit by November 2016. As a result, restricting controls to be eventually-visited counties forces us to trade off the number of post periods with the number of cohorts we can estimate treatment effects for. We estimate effects for event times from -7 to +5 months. This implies that the last cohort we can estimate effects for have their first Trump visits in April 2016.[^A3]

[^A3]: Original footnote 3 (Appendix). Since control counties must be visited by November 2016 and there is one month of anticipation, treatment effects can only be estimated up to September 2016. Five months before September 2016 is April 2016.
