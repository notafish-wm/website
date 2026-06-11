---
title: "Political Sentiment and Innovation: Evidence from Patenters"
authors: ["Joseph Engelberg", "Runjing Lu", "William Mullins", "Richard Townsend"]
date: "2024-09-15"
status: "Published"
journal: "Review of Financial Studies, 2025"
doi: "10.1093/rfs/hhaf029"
url: "https://doi.org/10.1093/rfs/hhaf029"
jel: ["O31", "J24", "M5", "D72"]
keywords: ["Patents", "Partisanship", "Productivity"]
conversion: "Text-only Markdown for LLM reading. Images omitted. Tables converted to semantic Markdown."
mode: "publication"
---

# Political Sentiment and Innovation: Evidence from Patenters

Joseph Engelberg (UC San Diego), Runjing Lu (U. of Toronto), William Mullins (UC San Diego), Richard Townsend (UC San Diego & NBER)

*Review of Financial Studies (accepted), September 15, 2024.*

We thank our Editor, Lauren Cohen, for his comments and clear guidance, as well as our referees for their helpful suggestions. Engelberg, jengelberg@ucsd.edu; Lu, runjing.lu@utoronto.ca; Mullins, wmullins@ucsd.edu; Townsend, rrtownsend@ucsd.edu.

## Converter's summary

This summary was written by the converter and is not part of the paper. The paper asks whether party-changing U.S. presidential elections affect worker productivity through political sentiment, using inventors as the setting because their output (patent applications) is directly observable. The authors match USPTO inventors to the L2 registered-voter database, identifying 376,000 Democratic or Republican inventors, and run difference-in-differences event studies around the 2008 (Obama) and 2016 (Trump) elections. Democratic inventors' annual likelihood of patenting rises by 2.1% of the mean relative to Republicans by three years after 2008 and falls by 3.8% of the mean after 2016 (Figure 2; Table 2, column 4 reports DID estimates of 0.24 and -0.38 percentage points). Effects are two to seven times larger among politically active Democrats, identified via voting history (Table 3), and survive Firm × Post and Firm × Technology (sub)class × Post fixed effects (Tables 4 and 5), which argues against policy-based explanations. Survey microdata from Gallup, Bloomberg, and Michigan show partisan swings in economic optimism and mood among graduate-educated and professional respondents (Figures 4, 5, A1), and citation patterns (Table 8) suggest the economic-optimism channel dominates mood. The paper also documents substantial and increasing political segregation across technologies, firms, and patenting teams (Table 9, Figure 6), so individual effects aggregate: Democratic technology subclasses gain roughly one standard deviation more granted patents than Republican subclasses by 2010 following the 2008 election (Figure 7, Table A9).

## Abstract

We document political sentiment effects on U.S. inventors. Democratic inventors are more likely to patent (relative to Republicans) after the 2008 election of Obama but less likely after the 2016 election of Trump. These effects are at least twice as strong among politically active Democrats and are present even within firms and within firm×technology. We also show that partisans tend to cluster in technologies (e.g., Democrats in Biotechnology and Republicans in Weapons), so that sentiment effects aggregate up to more patents in the technologies dominated by the winning party.

**Keywords:** Patents, Partisanship, Productivity

**JEL Classification Numbers:** O31, J24, M5, D72

## 1. Introduction

U.S. presidential elections are perceived by many to be life-changing events. Voters whose candidate lost the election report sharp decreases in their economic expectations and subjective well-being (e.g., Mian, Sufi, and Khoshkhou, 2023, Di Tella and MacCulloch, 2005). For example, Republicans went from being one standard deviation less optimistic than Democrats immediately before the 2016 election to a standard deviation more optimistic in the first quarter of 2017.[^1] This paper asks whether Americans bring these feelings and expectations to work: do party-changing elections affect worker productivity?

[^1]: Source: Bloomberg Consumer Comfort Index; standard deviation is calculated using data from June 1990 through October 2016, see Figure A1.

Election-driven changes in sentiment could affect both workers' willingness and their ability to be productive. First, workers who become less optimistic about the economy and who share in the rents created by their labor may exert less effort after their party loses because they anticipate a lower return. Second, because mood affects productivity (Banerjee and Mullainathan, 2008, Oswald, Proto, and Sgroi, 2015), workers who become less happy as the result of an election loss may experience a decline in their productive capacity. Regardless of the mechanism, political cycles coupled with increasing partisanship may have important downstream effects on productivity.

We focus on innovative workers who produce patents. These workers are particularly important because the productivity of U.S.-based patenters is a major driver of technological innovation, thus constituting a critical determinant of long-run economic growth (Romer, 1990, Aghion and Howitt, 1992, Mokyr, 1992, Kogan et al., 2017, Bloom et al., 2020, Liu and Ma, 2021), international competitiveness (Hombert and Matray, 2018), and startup activity (Farre-Mensa, Hegde, and Ljungqvist, 2020).[^2] These workers also provide an advantageous setting to examine the effects of political sentiment on worker productivity for two reasons. First, their productive output is directly observable via the U.S. Patent and Trademark Office (USPTO) patent database. Second, innovative workers' income is tied to the success of their patents (Kline, Petkova, Williams, and Zidar, 2019), which allows for economic expectations to naturally feed back into their productivity decisions.

[^2]: A series of papers link sharply declining innovative productivity (e.g., Kortum, 1997, Jones, 2009, Bloom et al., 2020) with declining growth rates in economies at the technological frontier (e.g., Cowen, 2011, Gordon, 2016), underscoring the importance of understanding the patent production function.

We investigate productivity effects on patenters around the party-changing presidential elections of 2008 (Barack Obama) and 2016 (Donald Trump), comparing party-identified individual patenters in the same geographic area, technology, and firm before vs. after each election. To do this, we match USPTO inventors to a database of all registered voters in the U.S., identifying 376,000 inventors who are either Democrats or Republicans.

We begin the analysis by exploring whether party-changing elections affect the relative productivity of individuals who identify with the winning or losing side. Specifically, we examine Republicans' and Democrats' patenting probability after removing the quarterly or yearly average by technology class. The two groups' likelihood of patenting is indistinguishable in the two years before each election, as well as during the election year and even in the first year post-election (Figure 1). However, clear partisan trends emerge by the second year post-election, with the winning side's relative patenting probability rising above the pre-period level.

While Figure 1 shows group averages over time, we also use a difference-in-differences event study approach that controls for individual characteristics and includes fixed effects for geography and technology-by-time. We continue to find an increase in productivity for Democratic patenters (relative to Republicans) after the 2008 election, and a relative decline in productivity after the 2016 election. Specifically, Democratic inventors' annual likelihood of patenting is 2.1% of the mean higher than that of Republicans by the third year after the 2008 election (see Figure 2). However, their relative productivity drops by 3.8% of the mean by the third year after the 2016 election. There are no discernible pretrends before each election.

To sharpen the evidence that it is the political orientation of inventors that mediates the effect of election outcomes on productivity, we examine politically active partisans. Specifically, we use the voting history – in general and primary elections – of each inventor to separate active partisans from less-committed ones. The intuition is straightforward: an individual who is more involved in political elections is more likely to be affected by a regime switch than someone who is not. If this is true, we should find stronger effects among the set of politically active patenters. This is precisely what we find: effect sizes for politically active Democratic patenters are two to seven times larger than those for politically inactive ones. A similar pattern emerges when we use inventors' history of voting in primary elections to capture political activeness, with the idea that primary voters are especially active partisans.

While our baseline results are consistent with party-based sentiment changes around elections, they could also be consistent with party-based policy changes around elections, where the winning party promotes certain technologies it favors. Specifically, we may observe an increase in patenting productivity among patenters aligned with the winning party because they work at firms that specialize in technologies favored by that party.

To address this issue, we repeat our main analysis within firms, comparing the differential change in patenting activity before vs. after political regime shifts between Republicans and Democrats working at the same firm. Specifically, we add Firm × Post fixed effects to our main specification and find similar results: within a firm, active Democrats are 2.6% of the mean more likely to patent than Republicans after the 2008 election and 1.5% less likely after the 2016 election.

However, it remains possible that looking within firms is not sufficient to account for policy effects if firms work on multiple technologies. In this case, firms could tilt their patenting activity towards areas favored by the policies of the newly elected president. To address this issue, we utilize the USPTO's measure of patent technologies, which sorts patents in our data into 123 technology classes and 625 technology subclasses. Our most demanding specifications include Firm × Technology class × Post fixed effects or Firm × Technology subclass × Post fixed effects, so that the effect is estimated within each firm-technology cell. Our main effect continues to hold with comparable magnitudes in these specifications.

We also perform a variety of tests to better understand the channel which generates our results. First, we test two underlying assumptions of the within-firm version of the policy channel: (1) that Democrat and Republican patenters specialize in different technologies within firms, and (2) that firms shift their investment in these technologies based on the outcomes of elections. The evidence we find is inconsistent with both of these assumptions.

As supporting evidence of a political sentiment channel, we examine survey microdata from Gallup, Bloomberg, and the University of Michigan. The surveys show large swings along party lines in both optimism about the economy and mood following party-changing elections. These partisan differences persist throughout presidential administrations and hold when we focus on respondents who are professionals and those with a graduate degree, as most patenters are in these groups.

To further explore whether our results are consistent with a political sentiment channel, we examine the effect of party-changing elections on the quality of the patents produced by Democrats and Republicans. If there are political sentiment effects tied to economic optimism, we would expect patenters aligned with the losing side to focus their efforts only on the most promising ideas, which would be robust to the poor economic conditions they expect. Thus, while their likelihood of patenting would decline, the average quality of submitted patents should increase. We generally find evidence consistent with this hypothesis. Specifically, patents produced by Democrats shortly after the election of Barack Obama have fewer citations (compared to Republicans) while those produced after the election of Donald Trump have relatively more citations.

Our baseline results are also robust to alternative specifications and sample restrictions. For example, our results hold when we partition partisans into finer groups: active Democrats, inactive Democrats, active Republicans, and a baseline group of inactive Republicans. In particular, we find that active Democrats are the most responsive to party-changing presidential elections in our sample. Results continue to hold when we control for a variety of patenter team characteristics. We also find similar effects when we focus on patenters who remain in the profession through the election post-period, indicating that patenter exit is not driving the results we find.

Next, we investigate the aggregate implications of the individual-level productivity effects we have documented. If, following an election, some inventors become less productive and some become more productive, it is possible that these effects offset in the aggregate. However, to the extent that certain technologies or firms are heavily skewed toward one party, offsetting effects will not occur. For example, if Technology X was populated by only Republican inventors and those inventors became less productive following Obama's election in 2008, then we would expect Technology X to lag in its rate of progress following 2008. Motivated by this observation, we examine the extent of political segregation in our setting.

We find evidence of significant political segregation among patenters both across firms and across technological areas (Figure 6). Specifically, the dissimilarity index (measuring segregation) increased by 10% or more for technologies starting around 2016, with a similar pattern among firms. As an illustration, Republicans outnumber Democrats 3-to-1 in weapons patenting, but are outnumbered by Democrats 5-to-1 at Google. Moreover, we find increasing segregation among patenting teams, which are critical to knowledge production (Jaravel, Petkova, and Bell, 2018). Beginning in 2004, we show a strong downward trend in patent applications from mixed-party teams (i.e., teams with both Democrats and Republicans). The likelihood of a mixed team submitting a patent fell by 14% from 2004 to 2019.

Given the evidence of political segregation among patenters, we would expect partisan sentiment shocks to have aggregate effects on technological progress. To directly examine this, we study technology-level patenting patterns around the 2008 election.[^3] We find that Democrat-dominated technologies display a steadily increasing innovative advantage relative to Republican technologies following the election, with no discernible difference beforehand. Specifically, Democratic technology subclasses have one standard deviation more granted patents than Republican ones in 2010, with the difference growing to 1.5 standard deviations by 2015.

[^3]: For this exercise we focus on granted patents because these are the innovations that matter for technological progress, and on the 2008 election because our data run through 2019, making the data on granted patents following the 2016 election too sparse.

**Contribution to the literature.** This paper is at the intersection of two growing literatures: the effects of partisanship on real outcomes and the determinants of innovation. First, our paper contributes to a new literature on the economic effects of partisanship. Most of this literature tests a joint hypothesis: (1) that elections lead to changes in political sentiment among partisans and (2) that these sentiment changes have downstream effects on behavior. Evidence for the first leg of the hypothesis is well established via survey and expectations data (e.g., Bartels, 2002, Di Tella and MacCulloch, 2005, Evans and Andersen, 2006, Mian, Sufi, and Khoshkhou, 2023, Meeuwis et al., 2022). We also provide confirmatory evidence using Gallup microdata (Figures 4 and 5). Evidence of the effects of political sentiment on economic decisions include decisions taken by households (Meeuwis et al., 2022, Cookson, Engelberg, and Mullins, 2020, Cullen, Turner, and Washington, 2021, Dahl, Lu, and Mullins, 2022, Bernstein et al., 2022a, McCartney, Orellana-Li, and Zhang, 2024), financial professionals (Dagostino, Gao, and Ma, 2023, Kempf and Tsoutsoura, 2021), and firms (Colonnelli, Neto, and Teso, 2022, Fos, Kempf, and Tsoutsoura, 2023, Engelberg et al., 2024). To the best of our knowledge, this is the first paper to examine partisan effects on worker productivity and technological progress. We document effects for a uniquely important class of workers for which we can observe a major output measure.

Second, our paper contributes to the literature on the determinants of innovation. Most of this literature takes a "top-down" view, in which firms invest in innovation based on expected profits, and employees simply execute these plans. Accordingly, the work in this area has focused on firm-level and market-level drivers of innovative output (e.g., Manso, 2011, Nanda and Rhodes-Kropf, 2013, Bernstein, 2015, Krieger, Li, and Papanikolaou, 2022, Bena and Simintzi, 2023). In contrast, our findings highlight a "bottom-up" view of innovation, wherein innovative workers are not interchangeable parts, but instead play an important role as individuals. Specifically, we explore whether political sentiment shocks to workers affect their innovative output and team formation. In this sense our work is similar in spirit to Bernstein, McQuade, and Townsend (2021) and Babina, Bernstein, and Mezzanotti (2023), who explore the effects of financial shocks on worker-level innovation.

The paper proceeds as follows. Section 2 describes the data and sample, Section 3 the empirical strategy and results, and Section 4 concludes.

## 2. Data and Sample

### 2.1 Patent data

We measure individual productivity via patenting output. We obtain patent data directly from the United States Patent and Trademark Office (USPTO). These data cover all patent applications and grants published from 2001 through 2019. For most of our analysis we focus on patent applications rather than patent grants to measure productivity. We do this to minimize truncation issues at the end of our sample period stemming from the lag between an application and a grant. Patent applications have two additional advantages relative to grants: (i) applications appear sooner than grants, allowing us to better match the event to its response, and (ii) they measure innovative effort rather than quality. As is standard in the literature, we limit attention to utility patents and exclude design patents from our analysis. The USPTO provides information on: the date a patent was applied for and ultimately granted (if applicable); the individuals credited as the patent's inventors along with the zip code of their residence; the firm to which the patent was originally assigned (if applicable); other patents cited as prior work; and the technology area that the patent falls under.

We define a patent's technology class based on its primary Cooperative Patent Classification (CPC) code. The U.S. switched to classifying patents using the CPC scheme at the start of 2015. For patents granted before 2015, we obtain a CPC classification from the USPTO's back-filled classifications (using the CPC Master Classification File for U.S. Patent Grants).

A challenge that the data presents is that it lacks consistent identifiers for patent inventors and firms: they are identified primarily by their names, which may not be unique. In addition, even for the same firm or individual there can be slight variation in how their name is listed due to differing conventions or recording errors. Therefore, we create inventor and firm identifiers for our sample following Balsmeier et al. (2015). Our procedure is detailed in Appendix A.

### 2.2 Voter data

We obtain data on the universe of registered voters, including their partisan affiliation, as of October 2020 from L2, a non-partisan data provider used by political groups and academics (e.g., Allcott, Braghieri, Eichmeyer, and Gentzkow, 2020, Brown and Enos, 2021, Billings, Chyn, and Haggag, 2021, Bernstein, Billings, Gustafson, and Lewis, 2022a, Spenkuch, Teso, and Xu, 2023). For 42 states (including DC), L2 assigns political affiliation using voters' self-identification from voter registrations or from party-specific primary participation. For 7 states, where voters do not self-identify, L2 infers party identification using a variety of data sources, including demographics, exit polling, and commercial lifestyle data. For the final 2 states, primary voting information was available for some periods but not others. Therefore, self-identified party is used when available and modeled party is used otherwise.[^4] Only 18% of inventors in our sample reside in states with some modeling.[^5] L2 also provides voters' addresses and demographic variables, such as birth year, gender, race/ethnicity, and education. We include these demographic variables, fully interacted, as controls in our main specifications.

[^4]: L2's data is subject to repeated testing by political campaigns in the field. Academic work has also verified the accuracy of voter file partisanship measures: Bernstein, Billings, Gustafson, and Lewis (2022a) validates the accuracy of L2 partisanship by comparing 2012 partisanship in state files to 2018 L2 data; Brown and Enos (2021) runs a survey to verify L2 partisanship; Pew (2018) compares voter file data to Pew national survey microdata.

[^5]: The 9 states with some party modeling are: Alabama, Hawaii, Michigan, Minnesota, Missouri, Montana, North Dakota, Vermont, Washington. L2's party inference varies according to data availability in each state. We later verify the robustness of our results to excluding these states.

Among registered voters, we identify those who are more politically active in two ways. First, we use voting history data from previous general and primary elections.[^6] For each election, we define individuals as politically active if they have voted in more than their party's median share of general and primary elections, out of all the elections that they were eligible for in the recent past (2000-2008 for the 2008 election; 2008-2016 for the 2016 election). We exclude consolidated general elections, which combine local and general elections and occur in odd years. Voting in primary elections likely indicates greater interest and attention to politics relative to voting in general elections. With this in mind, we construct an analogous, second measure of political activeness based only on participation in primaries.

[^6]: We use the 2020 voter roll and party affiliations because earlier versions of the data do not contain voting history, which is needed to construct our main activeness measure. We examine robustness to using the 2014 voter roll (the earliest available data) in Section 3.2.

As an additional way of identifying politically active individuals, we use data on political donations. The Federal Election Commission (FEC) records individuals' cumulative donations in excess of \$200 per election cycle, and L2 has linked these data to their voter registrations. We define inventors as politically active around the 2016 election if they made a political donation by 2016. For the 2008 election, we define inventors as politically active if they donated by 2014 (as far back as the L2 data go). If donation status as of 2014 or 2016 is unavailable for an individual, we use donation status as of 2020 instead. Around 9% of inventors in our sample are politically active (see Table 1) under this donation-based measure, which means we have only limited statistical power in specifications with many fixed effects (such as Firm × Post fixed effects). As a result, we use voting history as our main political activeness measure.

### 2.3 Sample construction

To construct our sample of patenters who are registered voters, we match the names in the voter database to the names of patenters in the USPTO database by name and address using an iterative algorithm. Specifically, we first match by name and state. A patenter is coded as matched to a voter if the patenter matches one and only one voter in the voter database. For the remaining unmatched patenters, we next match by name and county, followed by name and city. This matching procedure yields roughly 1.2 million patenter-voter matches, approximately 46% of U.S. patenters. Unmatched inventors are either (1) not a registered voter (either not a U.S. citizen or a citizen who is not registered to vote), or (2) do not have a name that is unique within their geographic area (i.e., it matches to multiple registered voters). We further require patenters to be between the ages of 18 and 70 during our sample period (2005 - 2019). To capture career patenters, we restrict our sample to those who submitted at least one granted patent in years t-4 to t-10 before an election year t (i.e., in a window before the pre-period in our analyses; hereafter referred to as the "pre pre-period").[^7] For example, we only include patenters who submitted at least one subsequently granted patent between 2006 and 2012 for the 2016 election. For our main analysis we focus on Democrats and Republicans; the resulting sample is a patenter-year panel with 224,000 to 235,000 individual inventors per year. The patents produced by these inventors over the sample period span 123 CPC technology classes and 625 subclasses.

[^7]: They span 1998-2004 and 2006-2012 for the 2008 and 2016 elections, respectively. Because we use granted patents to select the sample we can use data before 2001, as the granted patent data begins earlier. We assign patenters to their modal firm in this pre pre-period, as the firms they work for in later periods may be endogenous to the effects we examine.

### 2.4 Descriptive statistics

Table 1 reports statistics from our sample of Democrats and Republicans. Recall from Section 2.3 that our voter sample is composed of registered voters who are also patenters around the 2008 and 2016 elections. Table 1 combines the samples from both elections, and a disaggregated version is reported in Appendix Table A1.

Panel A indicates that approximately half the sample of patenters are Republicans (52%) and half are Democrats (48%). Moreover, consistent with the innovation literature, our sample is disproportionately male (89%, third column), college educated (84%), and has patents assigned to a firm (86%). Comparing Democrats and Republicans, there are a few clear differences. For example, among Democrats the sample is 15% female, while among Republicans it is only 8% (last column). Similarly, 90% of Republican inventors are white, compared to 75% among Democrats.

The annual likelihood of an inventor patenting is 18.1% (first column). The number is higher for Democrats (19.6%) than Republicans (16.6%). While patenting likelihood is relatively stable across most individual characteristics, this is not true for firm affiliation: inventors affiliated with a firm are much more likely in any given year to file for a patent (20%) than those who are not (6%).

Panel B reports the sample mean, median, and standard deviations for the voting and donation propensities underlying our three political activeness measures. Median voting propensities are around 50% for general elections and 17%-27% for primaries; approximately 9% of patenters in our sample have a recorded FEC donation.

### Table 1: Sample Statistics

- **Table type:** Summary statistics
- **Sample:** Patenter-year panel of Democratic and Republican inventors, 2005-2019, combining the 2008 and 2016 election samples
- **Units:** All units are in percentage points (pp)

#### Panel A: Summary statistics

For each characteristic row, `mean` is the average annual probability of submitting a patent (Pr(patent) in pp) conditional on the characteristic, `sd` the corresponding sample standard deviation, and `pct_sample` the fraction of patenters with that characteristic.

| characteristic | full_mean | full_sd | full_pct_sample | dem_mean | dem_sd | dem_pct_sample | rep_mean | rep_sd | rep_pct_sample |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| All | 18.07 | 38.48 | 100 | 19.60 | 39.70 | 100 | 16.64 | 37.24 | 100 |
| Male | 18.50 | 38.83 | 88.72 | 20.25 | 40.19 | 85.33 | 16.97 | 37.54 | 91.90 |
| Female | 14.74 | 35.45 | 11.28 | 15.83 | 36.51 | 14.67 | 12.89 | 33.51 | 8.10 |
| College+ | 18.82 | 39.09 | 84.24 | 20.46 | 40.34 | 85.72 | 17.35 | 37.87 | 82.95 |
| High school– | 14.53 | 35.24 | 15.76 | 15.79 | 36.46 | 14.28 | 13.61 | 34.29 | 17.05 |
| White | 17.61 | 38.09 | 82.84 | 19.42 | 39.56 | 74.62 | 16.26 | 36.90 | 90.28 |
| Black | 11.99 | 32.48 | 2.99 | 11.80 | 32.26 | 5.79 | 14.15 | 34.86 | 0.45 |
| Hispanic | 16.43 | 37.05 | 3.78 | 17.61 | 38.09 | 5.08 | 14.34 | 35.05 | 2.60 |
| Asian | 21.94 | 41.39 | 10.40 | 22.37 | 41.67 | 14.52 | 21.10 | 40.80 | 6.67 |
| Age 18-29 | 16.05 | 36.71 | 5.08 | 16 | 36.66 | 6.60 | 16.14 | 36.79 | 3.64 |
| Age 30-39 | 22.26 | 41.60 | 14.76 | 23.28 | 42.26 | 16.48 | 21.05 | 40.77 | 13.14 |
| Age 40-49 | 20.22 | 40.17 | 28.61 | 21.89 | 41.35 | 27.84 | 18.74 | 39.02 | 29.33 |
| Age 50-59 | 17.53 | 38.02 | 31.59 | 19.34 | 39.50 | 29.87 | 15.99 | 36.66 | 33.20 |
| Age 60-70 | 13.29 | 33.94 | 19.97 | 14.77 | 35.48 | 19.21 | 11.99 | 32.48 | 20.68 |
| With a firm | 20.02 | 40.02 | 86.44 | 21.36 | 40.98 | 88.66 | 18.71 | 39 | 84.35 |
| Without a firm | 5.65 | 23.09 | 13.56 | 5.90 | 23.56 | 11.34 | 5.49 | 22.77 | 15.65 |
| Active voter (all elections) | 18.02 | 38.44 | 54.06 | 19.82 | 39.86 | 54.38 | 16.31 | 36.95 | 53.77 |
| Active voter (primaries) | 17.85 | 38.30 | 55.55 | 19.74 | 39.80 | 55.09 | 16.11 | 36.76 | 55.99 |
| Active donor | 22.01 | 41.43 | 8.72 | 23.73 | 42.54 | 11 | 19.30 | 39.47 | 6.59 |

Sample counts:

| count | full_sample | democrats | republicans |
|---|---:|---:|---:|
| N patenters × year | 5,291,640 | 2,562,831 | 2,728,809 |
| N patenters | 375,857 | 181,673 | 194,184 |
| N states | 51 | 51 | 51 |

#### Panel B: Political activeness

| election | variable | full_mean | full_median | full_sd | dem_mean | dem_median | dem_sd | rep_mean | rep_median | rep_sd |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 2008 | Voting propensity (all elections) | 52.36 | 50 | 26.23 | 54.78 | 53.85 | 26.97 | 50.24 | 50 | 25.37 |
| 2008 | Voting propensity (primaries) | 30.98 | 25 | 31.33 | 35.17 | 25 | 32.19 | 27.37 | 16.67 | 30.12 |
| 2008 | Donation indicator | 8.73 | 0 | 28.23 | 11.02 | 0 | 31.31 | 6.60 | 0 | 24.83 |
| 2016 | Voting propensity (all elections) | 54.48 | 53.85 | 26.38 | 54.38 | 53.85 | 26.83 | 54.56 | 53.85 | 25.96 |
| 2016 | Voting propensity (primaries) | 36.10 | 25 | 32.09 | 36.76 | 27.27 | 31.99 | 35.50 | 25 | 32.16 |
| 2016 | Donation indicator | 8.76 | 0 | 28.28 | 11.05 | 0 | 31.35 | 6.63 | 0 | 24.88 |

**Note:** This table reports summary statistics between 2005 and 2019. All units are in percentage points (pp). In panel A, the first column in each grouping (Mean) displays the the average annual probability of submitting a patent, conditional on the patenter characteristic in each row. The SD column displays the corresponding sample standard deviation. The %Sample column displays the fraction of patenters with each characteristic in the sample. Columns 1-3, 4-6, and 7-9 are calculated based on both Democrats and Republicans, only Democrats, and only Republicans, respectively. Male is an indicator for being male, College+ (High school–) is an indicator for having a college or higher degree (having a completed high school or lower degree), Age xx-yy is an indicator for being between xx and yy years old, and With a firm (Without a firm) is an indicator for a patenter being affiliated with a firm (or not). Active voter (all elections), active voter (primaries), and active donor are indicators for having an above-median voting propensity in all non-consolidated general and primary elections that they were eligible for in the recent past (2000-2008 for the 2008 election; 2008-2016 for the 2016 election), in primaries, and having at least one recorded FEC donation, respectively (see Section 2.2). "States" corresponds to 50 states plus DC. In panel B, we report the sample mean, median, and standard deviations for the voting and donation propensities underlying the three political activeness measures in panel A. [Conversion note: "displays the the average" duplication appears in the original note and is preserved.]

## 3. Empirical Strategy and Results

### 3.1 Election event study

Our first approach is a difference-in-differences (DID) event study design contrasting individuals of different political parties, within the same geographic area and technology, around presidential elections. We estimate the following regression:

$$
Y_{it} = \sum_{\tau=-3,\tau\neq-1}^{3} \beta_\tau \mathbb{1}\{EventYear_t = \tau\} \times Dem_i + \gamma Dem_i + \delta' X_{it} + \alpha_{zip(i)} + \alpha_{technology(i),t} + \epsilon_{it} \tag{1}
$$

where $Y_{it}$ is an indicator for individual $i$ submitting a patent application in year $t$. Event time $t$ indexes the number of years relative to the elections we examine (2008 and 2016). We define $t = 0$ as the year of a presidential election (2008 and 2016) and omit $t = -1$ as the reference period. We focus our attention on years $-3$ through $+3$ to include only one presidential election in each regression. Our treatment variable is $Dem_i$, which equals one if individual $i$ is a Democrat and zero if they are Republican (see Section 2.2 for definitions of partisanship). We include inventor zip code fixed effects $\alpha_{zip(i)}$ and inventor technology-by-year fixed effects $\alpha_{technology(i),t}$ to control for average patenting activity in a zip code (Ganguli, Lin, and Reynolds 2020) and time-varying technology-specific average patenting. We define a patenter's technology as the technology class in which they most frequently patented in the pre pre-period.[^8] We also control for individual characteristics $X_{it}$, which are fully saturated interactions between gender, education, race/ethnicity, and age group bins. To allow for arbitrary cross-inventor correlation by geographic area, we cluster standard errors by zip code.

[^8]: Specifically, a patenter is assigned the technology in which they submitted the most applications in years $t-10$ to $t-4$, counting only granted patents.

A key assumption of the DID event study methodology is that patenting trends for Democratic and Republican inventors (within the same zip code and the same technology-year) would have been parallel in the absence of a presidential election. In this case, the $\beta_\tau$ vector in equation 1 identifies the causal impact of an election outcome on the productivity of Democratic vs. Republican inventors.

Starting with the raw data, Figure 1 plots the probability of submitting a patent, separately for Democratic and Republican inventors, after removing quarterly or yearly technology class averages. The top panels plot these probabilities at a quarterly frequency for the 2008 and 2016 elections, while the bottom panels do so yearly, which reduces the impact of noise in the data. For both elections, the figure shows that before the election, Republican and Democratic inventors' average probabilities of patenting within technology classes are very similar. After the election we see divergence in the expected directions. For 2008, Democratic inventors appear to increase their likelihood of submitting a patent application relative to Republicans (and to the pre-period) starting six quarters after the election, while in 2016 the divergence begins around four quarters after, with Republican patent applications appearing at higher rates.[^9]

[^9]: The main takeaway from Figure 1 is that the Democratic (blue) line rises after 2008 (i.e., Democrats' patenting likelihood is higher than the technology class average) and falls after 2016. The Republican (red) line moves in the opposite direction because for Democrats' patenting probability to be above the mean in a technology class, the Republicans' probability must be below the mean. The lines are not fully symmetric because the share of Republicans and Democrats in each technology class by time cell is not equal.

### Figure 1: Residualized Probability of Submitting a Patent Application — Democratic vs. Republican Inventors

- **Panels:** (a) 2008 election, quarterly; (b) 2016 election, quarterly; (c) 2008 election, annual; (d) 2016 election, annual
- **Axes:** y-axis "Residualized Pr(patent)"; x-axis calendar quarters (panels a-b: 2005q1-2012, 2013q1-2020) or calendar years (panels c-d: 2005-2011, 2013-2019)
- **Legend:** Democrat (solid, blue); Republican (dashed, red); vertical dashed line marks the election

**Note (verbatim):** This figure plots the (residualized) probability of submitting a patent application for Democratic and Republican inventors, at annual and quarterly frequencies. Residualized probability is the residual obtained from regressing the raw probability on technology class-by-quarter (panels a and b) or class-by-year (panels c and d) fixed effects. Units are in percentage points. Levels are normalized to 2007q4 and 2015q4 in panels (a) and (b), and to 2007 and 2015 in panels (c) and (d), respectively.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

In Figure 2, we plot the estimated $\beta_\tau$ coefficients from equation 1, capturing how the 2008 and 2016 elections changed the likelihood of patenting for Democrats relative to Republicans. Appendix Table A2 reports the regression estimates. There are no pre-trends leading up to either election, but we observe large and statistically significant effects in years two and three post-election.[^10] It makes sense that the effect only appears with a lag, as patent applications are likely a lagging measure of innovative activity, i.e., there is some time between when projects are initiated and when they generate patent applications. Other papers which examine shocks to innovation generally find effects within a similar time frame.[^11] Following the election of President Obama in 2008, we observe a relative increase in Democrats' annual patenting probability, converging to approximately 2.1% of the mean by year three. In contrast, following the 2016 election, Democrats' patenting probability decreased by 3.8% of the mean relative to Republicans by year three.

[^10]: A potential concern for election analyses is that the effect of one party-changing election could extend into the pre-period of another, potentially generating differential pre-trends. For the 2008 and 2016 elections we estimate event-study DID coefficients for a three year pre-period in Figure 2 and find no evidence of differential pre-trends. This indicates, for example, that the 2008 effect we document stabilizes by 2013, when the pre-period of the 2016 analysis begins.

[^11]: For example, Bernstein (2015) studies the impact on innovation of IPOs, Bloom, Davis, and Zhestkova (2021) the effect of the COVID-19 pandemic, Bernstein, McQuade, and Townsend (2021) the 2008-2009 U.S. real estate crash, and Bena and Simintzi (2023) the 1999 U.S.-China trade agreement. These papers show effects on patent applications manifesting within 1-5 years.

### Figure 2: Political Mismatch and the Probability of Submitting a Patent Application — Democratic vs. Republican Inventors

- **Panels:** (a) 2008 election; (b) 2016 election
- **Axes:** y-axis "Pr(patent): Dem - Rep" (range -1.5 to 1.5); x-axis "Years from 2008" / "Years from 2016" (-3 to 3); vertical dashed line at event time 0

**Note (verbatim):** This figure plots the estimated annual probability (and 90% confidence intervals) of submitting a patent application for Democratic inventors relative to Republican inventors around the 2008 and 2016 elections. Units are in percentage points, and the reference group is Republican inventors. Event time 0 refers to the year of a presidential election. Event time -1 is the reference period. All regressions control for zip code fixed effects, technology class × event-year fixed effects, and fully interacted voter characteristics (gender, education, age groups, race). Standard errors are clustered by zip code. Regression results are reported in Table A2.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred. The underlying point estimates are reported in Table A2.

### 3.2 Difference-in-differences analysis

#### 3.2.1 Democratic vs. Republican patenters

To summarize the DID event study coefficients into an average treatment effect over the years following each election, we estimate the following:

$$
Y_{it} = \beta Dem_i \times Post_t + \gamma Dem_i + \delta' X_{it} + \alpha_{zip(i)} + \alpha_{technology(i),t} + \epsilon_{it} \tag{2}
$$

where $Y_{it}$ is individual $i$'s patent activity in year $t$. Similar to equation 1, we focus on the three years before and the three years after party-switching presidential elections. We exclude the election year to avoid potential anticipation effects. The variable $Post_t$ is one for the three years following the election year, and zero otherwise. In our basic specification, we include zip code fixed effects $\alpha_{zip(i)}$ and technology × post fixed effects $\alpha_{technology(i),t}$. In more demanding specifications, we add individual fixed effects $\alpha_i$, geographic area × post fixed effects $\alpha_{geo(i),t}$, firm × post fixed effects $\alpha_{firm(i),t}$, and even firm × technology × post fixed effects $\alpha_{firm(i),technology(i),t}$. The geographic fixed effects include state, county, and zip code. By including these additional fixed effects, we can further absorb time-invariant inventor traits that matter for patenting and time-varying patent activity within a geographic area or even within a firm and technology. All else is the same as in equation 1.

Our coefficient of interest is $\beta$, which identifies the average impact of party-changing presidential elections on the patenting likelihood of Democrats relative to Republicans living in the same area, patenting in the same technology, and working at the same firm. The DID estimates relative effects, which may be driven by a decrease in patenting likelihood among those aligned with the losing side, an increase in patenting among those aligned with the winning party, or both.

Table 2 reports the estimates from equation 2. We include increasingly demanding fixed effects moving from columns 1 to 8. Consistent with the patterns revealed by the DID event study, coefficients on $Dem_i \times Post_t$ are positive and generally statistically significant for the 2008 election and negative for the 2016 election. Column 4, which is analogous to the specification used in the event study figures and includes Zip code and Technology × Post fixed effects, reports point estimates of 0.24 and -0.38 for the 2008 and 2016 elections, respectively. In other words, Democratic patenters are 0.24 percentage points more likely than their Republican counterparts to submit patent applications in a given year following the election of President Obama but 0.38 percentage points less likely following the election of President Trump. This is a sizeable effect, representing 1.2% and 1.7% of the sample means for the 2008 and the 2016 elections, respectively. Columns 5 and 6 change zip to county fixed effects or add State × Post fixed effects. To check whether these changes in patenting productivity around elections occur within individual inventors, columns 7 and 8 include individual fixed effects. We find similar results, although with weaker statistical significance for 2016.[^12] As we discuss next, we find strong within-individual effects once we focus on politically active partisans.

[^12]: Throughout, we focus on inventors who appear in the 2020 voter roll and use their party registrations as of 2020. Table A3 panel A shows that results are very similar for the 2016 election if we use patenters who appear in the 2014 voter roll and their 2014 party affiliations. We cannot do this for the 2008 election because we do not have access to voter rolls before 2014.

### Table 2: Election DID Analysis: Democratic vs. Republican Inventors

- **Table type:** Regression
- **Dependent variable (all columns):** 1(Apply for patent)×100 — an indicator for submitting a patent application in a year; units in percentage points
- **Unit of observation:** Patenter-year
- **Standard errors:** Clustered by zip code, in parentheses
- **Demographic controls:** Fully interacted inventor characteristics (gender, education, age groups, race), included in all regressions
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | County FE | Zip FE | Person FE | State×Post FE | Technology Class×Post FE |
|---:|---|---|---|---|---|
| 1 | Yes | No | No | Yes | No |
| 2 | No | Yes | No | Yes | No |
| 3 | Yes | No | No | No | Yes |
| 4 | No | Yes | No | No | Yes |
| 5 | Yes | No | No | Yes | Yes |
| 6 | No | Yes | No | Yes | Yes |
| 7 | No | No | Yes | No | Yes |
| 8 | No | No | Yes | Yes | Yes |

#### Estimates — Panel A: 2008 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Dem×Post | coefficient | 0.055 | 0.068 | 0.226* | 0.236* | 0.268** | 0.279** | 0.306** | 0.336** |
| Dem×Post | standard_error | 0.131 | 0.130 | 0.134 | 0.134 | 0.131 | 0.131 | 0.135 | 0.132 |
| Dem | coefficient | 2.539*** | 2.310*** | 1.666*** | 1.580*** | 1.645*** | 1.558*** | not applicable | not applicable |
| Dem | standard_error | 0.148 | 0.154 | 0.145 | 0.152 | 0.146 | 0.152 | not applicable | not applicable |

#### Model statistics — Panel A: 2008 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Observations | 1,307,930 | 1,309,566 | 1,307,612 | 1,309,242 | 1,307,612 | 1,309,242 | 1,309,242 | 1,309,242 |
| R-squared | 0.032 | 0.063 | 0.049 | 0.078 | 0.049 | 0.078 | 0.484 | 0.485 |
| Outcome mean | 19.69 | 19.69 | 19.69 | 19.69 | 19.69 | 19.69 | 19.69 | 19.69 |
| N clusters (zip) | 18,549 | 18,562 | 18,548 | 18,561 | 18,548 | 18,561 | 18,561 | 18,561 |

#### Estimates — Panel B: 2016 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Dem×Post | coefficient | -0.540*** | -0.531*** | -0.377*** | -0.375*** | -0.253** | -0.247* | -0.243* | -0.135 |
| Dem×Post | standard_error | 0.128 | 0.128 | 0.126 | 0.126 | 0.129 | 0.129 | 0.126 | 0.130 |
| Dem | coefficient | 2.507*** | 2.141*** | 1.915*** | 1.678*** | 1.856*** | 1.616*** | not applicable | not applicable |
| Dem | standard_error | 0.154 | 0.160 | 0.152 | 0.158 | 0.152 | 0.159 | not applicable | not applicable |

#### Model statistics — Panel B: 2016 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Observations | 1,356,239 | 1,358,125 | 1,355,588 | 1,357,474 | 1,355,588 | 1,357,474 | 1,357,474 | 1,357,474 |
| R-squared | 0.030 | 0.059 | 0.047 | 0.075 | 0.047 | 0.075 | 0.501 | 0.501 |
| Outcome mean | 22.13 | 22.12 | 22.13 | 22.12 | 22.13 | 22.12 | 22.12 | 22.12 |
| N clusters (zip) | 17,651 | 17,665 | 17,649 | 17,663 | 17,649 | 17,663 | 17,663 | 17,663 |

**Note:** This table reports estimates of equation 2, corresponding to difference in differences (DID) analyses comparing the likelihood of a Democratic inventor applying for a patent relative to a Republican one around the 2008 and 2016 presidential elections. The outcome is an indicator for submitting a patent application in a year, and units are in percentage points. Dem equals one for Democrats and zero for Republicans. Post is one for the first through third years after a presidential election. For example, for the 2016 election, Post refers to 2017, 2018, and 2019. The year of a presidential election is excluded. Note that Post by itself is not reported because it is absorbed by State×Post and/or Technology Class×Post fixed effects. Demographic controls correspond to fully interacted inventor characteristics (gender, education, age groups, race) and are included in all regressions. "FE" denotes fixed effects. Standard errors in parentheses are clustered by zip code. *** 1%, ** 5%, * 10% significance level. [Conversion note: in models 7-8 the Dem coefficient is absorbed by person fixed effects and the original cells are blank; marked "not applicable".]

#### 3.2.2 Political activeness

To sharpen the evidence that it is the political orientation of inventors that mediates the effect of election outcomes on productivity, we examine politically active partisans (as defined in Section 2.2). Specifically, we use the voting history of each inventor to distinguish an active partisan from a less-committed one. Shifts in political power should have a stronger impact on the productivity of politically active inventors vs. less committed partisans if the effect operates via partisanship. To test this, we estimate the following model:

$$
\begin{aligned}
Y_{it} = \; & \beta_1 Active\,Dem_i \times Post_t + \beta_2 Inactive\,Dem_i \times Post_t + \gamma_1 Active\,Dem_i \\
& + \gamma_2 Inactive\,Dem_i + \delta' X_{it} + \alpha_{zip(i)} + \alpha_{technology(i),t} + \epsilon_{it}
\end{aligned} \tag{3}
$$

where $Active\,Dem_i$ ($Inactive\,Dem_i$) equals one if individual $i$ is a politically (in)active Democrat, and zero otherwise. Republicans are the reference group. All variable definitions follow those in equation 2.

Table 3 reports the estimates using voting history to define the intensity of partisanship. We identify politically active partisans using the two approaches in Section 2.2: one based on their voting histories in general and primary elections and one based on primaries alone. Because voting in primaries is less common, it constitutes a more discriminating measure of activeness relative to voting in any elections (general and primaries). This table estimates all of the specifications of Table 2 with either zip code or person fixed effects, splitting Democrats into active and inactive groups using both definitions of political activeness. Across all specifications, active voter Democrats experience a significant increase in patenting likelihood relative to Republicans following the 2008 election, while inactive Democrats do not. In column 1, which includes Zip code and Technology × Post fixed effects, active voter Democrats are 0.52 percentage points less likely to submit patent applications in a given year compared to Republicans after the 2008 election, which is over seven times larger than the effect among inactive Democrats. An analogous relative decrease in patent likelihood also appears after the 2016 election. In columns 3 and 4, we add individual fixed effects; the point estimates remain strongly significant with similar magnitudes. Using the definition of active voters based on primaries (columns 5-8), estimates are slightly smaller for 2008 and slightly larger for 2016.[^13]

[^13]: In Appendix Table A4 panel B we use the specifications in Tables 2 and 3, but use political donations to measure activeness; results are similar or stronger, albeit with larger standard errors.

### Table 3: Election DID Analysis by Voting Activeness

- **Table type:** Regression
- **Dependent variable (all columns):** 1(Apply for patent)×100; units in percentage points
- **Unit of observation:** Patenter-year
- **Reference group:** Republican inventors
- **Standard errors:** Clustered by zip code, in parentheses
- **Demographic controls:** Included in all columns (as in Table 2)
- **Technology Class×Post FE:** Included in all columns
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | activeness_definition | Zip FE | Person FE | State×Post FE |
|---:|---|---|---|---|
| 1 | General & primary voting | Yes | No | No |
| 2 | General & primary voting | Yes | No | Yes |
| 3 | General & primary voting | No | Yes | No |
| 4 | General & primary voting | No | Yes | Yes |
| 5 | Primary voting only | Yes | No | No |
| 6 | Primary voting only | Yes | No | Yes |
| 7 | Primary voting only | No | Yes | No |
| 8 | Primary voting only | No | Yes | Yes |

#### Estimates — Panel A: 2008 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Active Dem×Post | coefficient | 0.520*** | 0.523*** | 0.511*** | 0.485*** | 0.496*** | 0.519*** | 0.479*** | 0.473*** |
| Active Dem×Post | standard_error | 0.172 | 0.174 | 0.173 | 0.175 | 0.174 | 0.176 | 0.175 | 0.177 |
| Inactive Dem×Post | coefficient | 0.069 | 0.129 | 0.145 | 0.206 | 0.047 | 0.074 | 0.125 | 0.155 |
| Inactive Dem×Post | standard_error | 0.169 | 0.167 | 0.169 | 0.167 | 0.174 | 0.173 | 0.174 | 0.173 |
| Active Dem | coefficient | 1.235*** | 1.232*** | not applicable | not applicable | 1.241*** | 1.228*** | not applicable | not applicable |
| Active Dem | standard_error | 0.201 | 0.202 | not applicable | not applicable | 0.203 | 0.205 | not applicable | not applicable |
| Inactive Dem | coefficient | 1.733*** | 1.703*** | not applicable | not applicable | 1.771*** | 1.758*** | not applicable | not applicable |
| Inactive Dem | standard_error | 0.191 | 0.190 | not applicable | not applicable | 0.194 | 0.194 | not applicable | not applicable |

#### Model statistics — Panel A: 2008 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Observations | 1,176,486 | 1,176,486 | 1,176,486 | 1,176,486 | 1,145,554 | 1,145,554 | 1,145,554 | 1,145,554 |
| R-squared | 0.079 | 0.079 | 0.480 | 0.481 | 0.080 | 0.080 | 0.480 | 0.480 |
| Outcome mean | 19.39 | 19.39 | 19.39 | 19.39 | 19.36 | 19.36 | 19.36 | 19.36 |
| N clusters (zip) | 17,988 | 17,988 | 17,988 | 17,988 | 17,845 | 17,845 | 17,845 | 17,845 |

#### Estimates — Panel B: 2016 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Active Dem×Post | coefficient | -0.565*** | -0.396** | -0.658*** | -0.526*** | -0.633*** | -0.450*** | -0.709*** | -0.566*** |
| Active Dem×Post | standard_error | 0.166 | 0.170 | 0.167 | 0.172 | 0.162 | 0.167 | 0.163 | 0.169 |
| Inactive Dem×Post | coefficient | -0.260* | -0.161 | -0.029 | 0.060 | -0.206 | -0.117 | 0.025 | 0.105 |
| Inactive Dem×Post | standard_error | 0.149 | 0.152 | 0.150 | 0.153 | 0.156 | 0.159 | 0.156 | 0.159 |
| Active Dem | coefficient | 1.950*** | 1.869*** | not applicable | not applicable | 1.903*** | 1.815*** | not applicable | not applicable |
| Active Dem | standard_error | 0.202 | 0.203 | not applicable | not applicable | 0.199 | 0.200 | not applicable | not applicable |
| Inactive Dem | coefficient | 1.528*** | 1.480*** | not applicable | not applicable | 1.524*** | 1.482*** | not applicable | not applicable |
| Inactive Dem | standard_error | 0.189 | 0.190 | not applicable | not applicable | 0.197 | 0.197 | not applicable | not applicable |

#### Model statistics — Panel B: 2016 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Observations | 1,299,929 | 1,299,929 | 1,299,929 | 1,299,929 | 1,279,202 | 1,279,202 | 1,279,202 | 1,279,202 |
| R-squared | 0.076 | 0.076 | 0.500 | 0.500 | 0.076 | 0.076 | 0.500 | 0.500 |
| Outcome mean | 22.04 | 22.04 | 22.04 | 22.04 | 22 | 22 | 22 | 22 |
| N clusters (zip) | 17,467 | 17,467 | 17,467 | 17,467 | 17,408 | 17,408 | 17,408 | 17,408 |

**Note:** This table reports estimates of equation 3, corresponding to DID analyses comparing the likelihood of politically active and inactive Democratic inventors applying for a patent relative to Republicans around the 2008 and 2016 presidential elections. The outcome is an indicator for submitting a patent application in a year, and units are in percentage points. Active Dem is an indicator for a politically active Democrat based on voting history; columns 1-4 define political activeness using voting in both primary and general elections while columns 5-8 use only primary elections (see note to Table 1 for political activeness measures). Inactive Dem is defined similarly. Post and demographic controls are defined as in Table 2. Standard errors in parentheses are clustered by zip code. *** 1%, ** 5%, * 10% significance level. [Conversion note: in person-FE columns (3, 4, 7, 8) the level terms Active Dem and Inactive Dem are absorbed and the original cells are blank; marked "not applicable".]

#### 3.2.3 Within firms

While the results thus far are consistent with party-based sentiment changes around election outcomes, an alternative explanation is that regime switches lead to policy changes promoting technologies favored by the party in power. As a result, we may see an increase in patenting productivity among patenters aligned with the winning party because they work on these favored technologies. For example, recent Democratic administrations have favored renewable energy technologies, while Republican administrations have favored traditional energy sources. Therefore, if Democratic patenters tend to work at renewable energy firms, they may become more productive when President Obama is elected in 2008 as a result of government incentives and subsidies for their firms. A similar process could occur for traditional energy after the election of President Trump.

In the above example, we should not see differential productivity changes between Republicans and Democrats working at the same energy firm around the 2008 or 2016 elections. Therefore, as a first attempt to examine the policy channel, we check whether our results hold within firms. Column 1 of Table 4 adds Firm × Post fixed effects to our main specification (i.e., Table 3 column 2).[^14] This means we are comparing Democrats to Republicans within the same firms across a political regime change.

[^14]: We do not control for Geography × Post fixed effects as they are largely co-linear with Firm × Post.

However, it remains possible that looking within firms is not sufficient to account for policy effects because some firms may work on multiple technologies. Returning to our example, an energy firm may have one division that works on renewable energy and another that works on traditional energy, with Democrats more likely to be working in the renewable energy division and Republicans in the traditional energy division. Within this firm, aligned patenters could become more productive because of the matching between partisans and the technologies favored by government incentives.

To address this possibility, we employ an even more demanding specification that estimates effects within firm and technology. Specifically, columns 2 and 3 add Firm × Technology class × Post fixed effects and Firm × Technology subclass × Post fixed effects, respectively, which effectively forces the comparison within the same firm and technology class (123 classes) or subclass (625 subclasses). All three columns produce results consistent with column 2 of Table 3.

We note that including such high dimensional fixed effects demands a lot of data. As a result, in a few cases the estimated coefficients become less statistically significant. To increase statistical power, in columns 4-6 of Table 4 we use an expanded dataset that adds back in patenters who we could not match to the L2 voter database, as well as registered political independents.[^15] While some variables are missing for these additional inventors (demographics and partisanship for non-L2 inventors), we have firm, technology, and geographic information for them, so they can be used in the estimation of the key fixed effects. Specifically, we fully interact the non-fixed-effect regressors in columns 1-3 with an indicator for being in the main sample and with an indicator for not being in the main sample, and report the former coefficients. As columns 4-6 show, the results are similar using this expanded sample. Columns 7-9 of Table 4 repeat the analysis of columns 4-6 using our other measure of political activeness based on primary voting and find similar results.[^16]

[^15]: We add back around 460,000 (580,000) independent patenters and 1,040,000 (1,500,000) un-matched patenters for the 2008 (2016) election.

[^16]: As discussed in Section 2.1, the USPTO switched from the USPC to the CPC technology classification scheme at the start of 2015 and retroactively reclassified all previous patents. While we use the CPC technology classification throughout, results are robust to using USPC classifications instead: see Appendix Table A5.

In general, Table 4 provides evidence inconsistent with policy-based explanations because our main effect continues to exist within narrowly defined firm-technology groups that should be affected similarly by policy.

### Table 4: Election DID Analysis within Firm and Technology by Voting Activeness

- **Table type:** Regression
- **Dependent variable (all columns):** 1(Apply for patent)×100; units in percentage points
- **Unit of observation:** Patenter-year (firm-affiliated inventors)
- **Standard errors:** Clustered by zip code, in parentheses
- **Demographics and Zip FE:** Included in all columns
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | activeness_definition | sample | fixed_effects (beyond Zip) |
|---:|---|---|---|
| 1 | General & primary voting | Main sample | Technology Class×Post; Firm×Post |
| 2 | General & primary voting | Main sample | Firm×Technology Class×Post |
| 3 | General & primary voting | Main sample | Firm×Technology Subclass×Post |
| 4 | General & primary voting | FEs estimated with expanded sample | Technology Class×Post; Firm×Post |
| 5 | General & primary voting | FEs estimated with expanded sample | Firm×Technology Class×Post |
| 6 | General & primary voting | FEs estimated with expanded sample | Firm×Technology Subclass×Post |
| 7 | Primary voting only | FEs estimated with expanded sample | Technology Class×Post; Firm×Post |
| 8 | Primary voting only | FEs estimated with expanded sample | Firm×Technology Class×Post |
| 9 | Primary voting only | FEs estimated with expanded sample | Firm×Technology Subclass×Post |

#### Estimates — Panel A: 2008 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Active Dem×Post | coefficient | 0.563*** | 0.512** | 0.444* | 0.593*** | 0.567*** | 0.461** | 0.529*** | 0.528** | 0.417** |
| Active Dem×Post | standard_error | 0.209 | 0.224 | 0.232 | 0.198 | 0.207 | 0.208 | 0.199 | 0.207 | 0.209 |
| Inactive Dem×Post | coefficient | 0.051 | 0.082 | -0.024 | 0.059 | 0.080 | -0.054 | 0.029 | 0.024 | -0.078 |
| Inactive Dem×Post | standard_error | 0.204 | 0.217 | 0.224 | 0.192 | 0.197 | 0.200 | 0.200 | 0.207 | 0.211 |
| Active Dem | coefficient | 1.243*** | 1.226*** | 1.277*** | 1.294*** | 1.260*** | 1.336*** | 1.340*** | 1.297*** | 1.386*** |
| Active Dem | standard_error | 0.236 | 0.252 | 0.262 | 0.238 | 0.239 | 0.245 | 0.241 | 0.243 | 0.242 |
| Inactive Dem | coefficient | 1.717*** | 1.719*** | 1.716*** | 1.837*** | 1.785*** | 1.771*** | 1.854*** | 1.815*** | 1.775*** |
| Inactive Dem | standard_error | 0.227 | 0.242 | 0.249 | 0.235 | 0.242 | 0.242 | 0.242 | 0.252 | 0.259 |

#### Model statistics — Panel A: 2008 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Observations | 1,007,287 | 1,007,287 | 1,007,305 | 1,007,287 | 1,007,287 | 1,007,305 | 980,793 | 980,793 | 980,805 |
| R-squared | 0.200 | 0.258 | 0.291 | 0.231 | 0.270 | 0.293 | 0.232 | 0.272 | 0.294 |
| Outcome mean | 21.69 | 21.69 | 21.69 | 21.69 | 21.69 | 21.69 | 21.65 | 21.65 | 21.65 |

#### Estimates — Panel B: 2016 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Active Dem×Post | coefficient | -0.351* | -0.428** | -0.352* | -0.441** | -0.489** | -0.489** | -0.545*** | -0.584*** | -0.604*** |
| Active Dem×Post | standard_error | 0.193 | 0.205 | 0.212 | 0.195 | 0.197 | 0.201 | 0.194 | 0.194 | 0.195 |
| Inactive Dem×Post | coefficient | -0.122 | -0.036 | 0.024 | -0.206 | -0.192 | -0.187 | -0.126 | -0.107 | -0.081 |
| Inactive Dem×Post | standard_error | 0.179 | 0.189 | 0.197 | 0.180 | 0.188 | 0.189 | 0.185 | 0.194 | 0.197 |
| Active Dem | coefficient | 1.693*** | 1.764*** | 1.654*** | 1.664*** | 1.707*** | 1.723*** | 1.633*** | 1.665*** | 1.684*** |
| Active Dem | standard_error | 0.236 | 0.253 | 0.261 | 0.234 | 0.232 | 0.238 | 0.232 | 0.230 | 0.236 |
| Inactive Dem | coefficient | 1.093*** | 0.995*** | 0.912*** | 1.284*** | 1.204*** | 1.215*** | 1.291*** | 1.209*** | 1.215*** |
| Inactive Dem | standard_error | 0.220 | 0.232 | 0.242 | 0.238 | 0.233 | 0.243 | 0.243 | 0.237 | 0.247 |

#### Model statistics — Panel B: 2016 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Observations | 1,159,878 | 1,159,878 | 1,159,784 | 1,159,878 | 1,159,878 | 1,159,784 | 1,141,165 | 1,141,165 | 1,141,072 |
| R-squared | 0.204 | 0.258 | 0.290 | 0.247 | 0.281 | 0.301 | 0.248 | 0.281 | 0.302 |
| Outcome mean | 23.84 | 23.84 | 23.84 | 23.84 | 23.84 | 23.84 | 23.8 | 23.8 | 23.8 |

**Note:** This table reports estimates of equation 3 as in Table 3, with the addition of Firm×Post, or Firm×Technology×Post fixed effects. Thus, these DID analyses compare the likelihood of Democratic inventors applying for a patent relative to Republicans in the same firm (and same technology) around the 2008 and 2016 presidential elections. The outcome is an indicator for submitting a patent application in a year, and units are in percentage points. Active Dem is an indicator for a politically active Democrat based on voting in both general and primary elections (columns 1-6) or only primary elections (columns 7-9); Inactive Dem is defined correspondingly. In columns 1-3, we include all inventors in our main sample affiliated with a firm; in columns 4-9, we use an expanded dataset that adds back in patenters affiliated with a firm but whom we could not match to L2 voter database or who are registered political independents. Note that "observations" denotes the number of patenter-year observations in the non-expanded sample (i.e., those in columns 1-3) rather than the total patenter-year observations in the regression, and "outcome mean" is calculated using the former. In columns 4-9, we fully saturate the non-fixed-effect regressors in columns 1-3 with indicators for being in the main sample and with an indicator for not being in the main sample, and report the former coefficients. By adopting this saturated model, we use only patenters in the main sample to estimate the reported coefficients, while using all patenters to estimate the fixed effects. Standard errors in parentheses are clustered by zip code. *** 1%, ** 5%, * 10% significance level.

Thus far, we have split Democrats into active and inactive, leaving all Republicans as the comparison group. This leaves open the possibility that our estimates reflect an "active voter effect" rather than an active Democrat effect. To examine this, we partition the sample into four groups – active Democrats, inactive Democrats, active Republicans, and a baseline category of inactive Republicans – and re-estimate Table 4. The results are reported in Table 5. The coefficients show that the productivity of active Democrats changes in the predicted direction around each election, regardless of whether we partition Republicans into two groups or not (i.e., comparing Table 4 to Table 5). This suggests that the effect is not merely an active voter effect, as there is no statistically significant effect among active Republicans. The table also shows that active Democrats are substantially more responsive than the other groups.

### Table 5: Election DID Analysis within Firm and Technology by Voting Activeness × Partisanship

- **Table type:** Regression
- **Dependent variable (all columns):** 1(Apply for patent)×100; units in percentage points
- **Unit of observation:** Patenter-year (firm-affiliated inventors)
- **Reference group:** Inactive Republicans
- **Standard errors:** Clustered by zip code, in parentheses
- **Demographics and Zip FE:** Included in all columns
- **Column structure:** Identical to Table 4 (see Table 4 column metadata): columns 1-3 main sample with general & primary voting activeness; columns 4-6 expanded-sample FEs; columns 7-9 expanded-sample FEs with primary-only activeness; fixed effects rotate across Technology Class×Post + Firm×Post (cols 1, 4, 7), Firm×Technology Class×Post (cols 2, 5, 8), and Firm×Technology Subclass×Post (cols 3, 6, 9)
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Estimates — Panel A: 2008 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Active Dem×Post | coefficient | 0.652*** | 0.628** | 0.531** | 0.699*** | 0.698*** | 0.601*** | 0.586*** | 0.620*** | 0.510** |
| Active Dem×Post | standard_error | 0.231 | 0.245 | 0.255 | 0.222 | 0.230 | 0.233 | 0.227 | 0.231 | 0.237 |
| Inactive Dem×Post | coefficient | 0.136 | 0.191 | 0.057 | 0.163 | 0.207 | 0.083 | 0.084 | 0.113 | 0.012 |
| Inactive Dem×Post | standard_error | 0.225 | 0.239 | 0.247 | 0.213 | 0.219 | 0.222 | 0.225 | 0.234 | 0.237 |
| Active Rep×Post | coefficient | 0.192 | 0.250 | 0.188 | 0.232 | 0.287 | 0.309 | 0.106 | 0.172 | 0.175 |
| Active Rep×Post | standard_error | 0.216 | 0.231 | 0.241 | 0.209 | 0.211 | 0.220 | 0.206 | 0.211 | 0.216 |
| Active Dem | coefficient | 1.194*** | 1.187*** | 1.300*** | 1.208*** | 1.156*** | 1.268*** | 1.203*** | 1.120*** | 1.246*** |
| Active Dem | standard_error | 0.267 | 0.284 | 0.297 | 0.252 | 0.255 | 0.260 | 0.263 | 0.269 | 0.270 |
| Inactive Dem | coefficient | 1.672*** | 1.681*** | 1.733*** | 1.755*** | 1.687*** | 1.705*** | 1.729*** | 1.653*** | 1.646*** |
| Inactive Dem | standard_error | 0.249 | 0.267 | 0.274 | 0.242 | 0.249 | 0.249 | 0.256 | 0.269 | 0.276 |
| Active Rep | coefficient | -0.103 | -0.085 | 0.041 | -0.185 | -0.223 | -0.149 | -0.248 | -0.323 | -0.256 |
| Active Rep | standard_error | 0.245 | 0.265 | 0.273 | 0.236 | 0.246 | 0.250 | 0.233 | 0.240 | 0.245 |

#### Model statistics — Panel A: 2008 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Observations | 1,007,287 | 1,007,287 | 1,007,305 | 1,007,287 | 1,007,287 | 1,007,305 | 980,793 | 980,793 | 980,805 |
| R-squared | 0.200 | 0.258 | 0.291 | 0.231 | 0.270 | 0.293 | 0.232 | 0.272 | 0.294 |
| Outcome mean | 21.69 | 21.69 | 21.69 | 21.69 | 21.69 | 21.69 | 21.65 | 21.65 | 21.65 |

#### Estimates — Panel B: 2016 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Active Dem×Post | coefficient | -0.455** | -0.557** | -0.483** | -0.498** | -0.558*** | -0.554** | -0.550** | -0.610*** | -0.638*** |
| Active Dem×Post | standard_error | 0.215 | 0.227 | 0.236 | 0.212 | 0.214 | 0.216 | 0.218 | 0.217 | 0.217 |
| Inactive Dem×Post | coefficient | -0.223 | -0.160 | -0.103 | -0.262 | -0.260 | -0.251 | -0.132 | -0.133 | -0.114 |
| Inactive Dem×Post | standard_error | 0.202 | 0.212 | 0.221 | 0.200 | 0.206 | 0.205 | 0.210 | 0.217 | 0.218 |
| Active Rep×Post | coefficient | -0.228 | -0.284 | -0.288 | -0.123 | -0.151 | -0.140 | -0.008 | -0.053 | -0.071 |
| Active Rep×Post | standard_error | 0.214 | 0.227 | 0.234 | 0.201 | 0.207 | 0.208 | 0.204 | 0.209 | 0.211 |
| Active Dem | coefficient | 2.023*** | 2.155*** | 2.072*** | 1.914*** | 1.974*** | 2.012*** | 1.745*** | 1.787*** | 1.815*** |
| Active Dem | standard_error | 0.262 | 0.281 | 0.291 | 0.248 | 0.248 | 0.253 | 0.252 | 0.253 | 0.256 |
| Inactive Dem | coefficient | 1.393*** | 1.352*** | 1.294*** | 1.518*** | 1.455*** | 1.486*** | 1.393*** | 1.322*** | 1.338*** |
| Inactive Dem | standard_error | 0.244 | 0.260 | 0.270 | 0.249 | 0.245 | 0.251 | 0.260 | 0.257 | 0.263 |
| Active Rep | coefficient | 0.734*** | 0.874*** | 0.935*** | 0.567** | 0.609** | 0.658** | 0.233 | 0.256 | 0.277 |
| Active Rep | standard_error | 0.255 | 0.273 | 0.283 | 0.239 | 0.248 | 0.256 | 0.237 | 0.241 | 0.248 |

#### Model statistics — Panel B: 2016 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Observations | 1,159,878 | 1,159,878 | 1,159,784 | 1,159,878 | 1,159,878 | 1,159,784 | 1,141,165 | 1,141,165 | 1,141,072 |
| R-squared | 0.204 | 0.258 | 0.290 | 0.247 | 0.281 | 0.302 | 0.248 | 0.281 | 0.302 |
| Outcome mean | 23.84 | 23.84 | 23.84 | 23.84 | 23.84 | 23.84 | 23.8 | 23.8 | 23.8 |

**Note:** This table mirrors Table 4 but adds Active Rep × Post and Active Rep (and their interactions with sample indicators where applicable); as a result, inactive Republicans become the baseline comparison group. Standard errors in parentheses are clustered by zip code. *** 1%, ** 5%, * 10% significance level.

**Robustness**

While we interpret our main effect as resulting from the difference between Republican and Democrat patenters, it is possible that it actually arises from their patenting teammates. For example, if Democrat patenters are more likely to co-patent with women than men, and productivity for women falls following the 2016 election, then this would appear to be a Democrat vs. Republican patenter effect when it is in reality a Democrat vs. Republican team effect. To address this issue, in Table A6, we reproduce Table 5 column 2 with a series of team composition controls and their interactions with the Post indicator, leaving out the focal inventor when calculating these characteristics. Specifically, columns 1 and 4 include team size controls: average team size and the fraction of team members matched to our political affiliation data. Columns 2 and 5 add team partisanship variables: the average share of teammates that are politically active Democrats and Republicans, and an indicator for working on a team with members of the opposite party. Finally, columns 3 and 6 add team demographic controls: the average age of teammates, the share that have a college degree or higher, and the shares of immigrants, men, Asian, African American, or Hispanic patenters.[^17] Across all specifications, the coefficients on Active Dem × Post are qualitatively unchanged when adding team controls in either the 2008 or 2016 elections, suggesting that our main result is unlikely to be driven by a Democrat vs. Republican team effect. In Table A7, we reproduce Table 5 column 3 (with Firm × Technology Subclass × Post fixed effects) and find similar results.

[^17]: Our data on immigrants come from Infutor, a commercial consumer identification provider. Their data includes social security numbers (SSNs) and year of birth for 187 million individuals who received their U.S. SSNs before the early 2000s. Following the procedure in Bernstein, Diamond, Jiranaphawiboon, McQuade, and Pousada (2022b), we use the first 5 digits of an individual's SSN to identify the year in which a number was assigned, and then use each person's year of birth to determine the age at which they received their SSN. An individual is classified as an immigrant if they were 21 or older when they received their SSN because native born citizens receive them at earlier ages. Using this approach, we identify approximately 23.5 million immigrants (12.6% of individuals in the Infutor data with SSN and birthyear information).

Recall from Section 2.2 that in many states registered voters identify themselves as Republican or Democrat – either through voter registration or participation in a primary election – while in other states our data provider, L2, uses models to predict the party affiliation of voters. As a robustness check, in Table A8 we drop states where all voters are modeled ("pure modeling," columns 1-3) or states where some of the voters are modeled ("any modeling," columns 4-6). The results are generally robust across specifications, albeit with larger standard errors in columns 4-6.

**Are the effects driven by exit?**

The effects we have estimated thus far combine the consequences of patenters leaving the profession with the effects of lower productivity among those remaining in the profession. However, identifying the precise timing of exit from our data is difficult, because we only observe individuals when they patent. Thus, we examine the complement: individuals that stay in the profession following an election. If our effects were entirely driven by exit, we should see no effects among those that remain.

Table 6 defines "non-exit" inventors in two ways. First, we consider individuals who submit at least one patent application after the post-period of the 2008 election, i.e., from 2012 through 2019. These patenters appear to have stayed in the profession during the post-period because we see activity from them after this period. Second, using LinkedIn data from Revelio Labs, we consider individuals who report no changes in job title, seniority, or company on LinkedIn during the post-period, i.e., from 2009 through 2011.[^18] The logic behind this definition is that patenters who are promoted or change jobs may either be exiting, or have moved into management positions that do not require patenting. By contrast, those remaining in the same job are likely still required to produce patents. In addition to using each definition of "non-exit" separately, we also consider the union of the two. We only analyze the 2008 election because we lack a sufficiently long post period to define non-exit patenters for the 2016 election.

[^18]: We match inventors to 2022 LinkedIn profiles based on a combination of their names and the names of the companies they have worked for, resulting in a match rate of approximately 33%.

Because these analyses are for sub-populations, we face statistical power challenges. To mitigate this problem, we include all other patenters in our main sample in the regression to help estimate the fixed effects, while using only the non-exit subsample to estimate the reported coefficients (by interacting all non-fixed-effect regressors with a non-exit sample indicator and with an indicator for the complement of this sample). The pattern of coefficients is similar when we do not use all inventors in our main sample to estimate the fixed effects, but standard errors are substantially larger.

Columns 1-3 of Table 6 show that our effects persist for patenters who continue to patent after 2011, with somewhat larger effects. For example, the effect size for Active Democrats in column 2 is 4.4% of the mean, which is larger than the 2.9% effect size in column 2 of Table 5. If we consider the non-exit definition based on LinkedIn data, the corresponding effect size is 7.5% (column 5); the combined definition (column 8) has an effect size of 4.4%. Overall, the effects are at least as strong in the non-exit sample, suggesting that our main results are not exclusively driven by patenter exit.

### Table 6: 2008 Election DID Analysis: Non-Exit Inventors

- **Table type:** Regression
- **Dependent variable (all columns):** 1(Apply for patent)×100; units in percentage points
- **Election:** 2008 only
- **Unit of observation:** Patenter-year
- **Reference group:** Inactive Republicans
- **Standard errors:** Clustered by zip code, in parentheses
- **Demographics and Zip FE:** Included in all columns
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | non_exit_definition | fixed_effects (beyond Zip) |
|---:|---|---|
| 1 | Continue patenting (application in 2012 onwards) | Technology Class×Post; Firm×Post |
| 2 | Continue patenting | Firm×Technology Class×Post |
| 3 | Continue patenting | Firm×Technology Subclass×Post |
| 4 | No change on LinkedIn (2009-2011) | Technology Class×Post; Firm×Post |
| 5 | No change on LinkedIn | Firm×Technology Class×Post |
| 6 | No change on LinkedIn | Firm×Technology Subclass×Post |
| 7 | Combined definition (union) | Technology Class×Post; Firm×Post |
| 8 | Combined definition | Firm×Technology Class×Post |
| 9 | Combined definition | Firm×Technology Subclass×Post |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Active Dem×Post | coefficient | 1.022** | 0.949** | 1.078** | 1.401* | 1.622** | 1.085 | 0.935** | 0.945** | 1.040** |
| Active Dem×Post | standard_error | 0.444 | 0.463 | 0.482 | 0.735 | 0.771 | 0.797 | 0.404 | 0.421 | 0.434 |
| Inactive Dem×Post | coefficient | 0.778* | 0.839* | 0.770 | 0.657 | 0.595 | 0.183 | 0.662 | 0.733* | 0.646 |
| Inactive Dem×Post | standard_error | 0.447 | 0.465 | 0.479 | 0.710 | 0.748 | 0.764 | 0.406 | 0.424 | 0.435 |
| Active Rep×Post | coefficient | 0.034 | 0.087 | 0.444 | -0.128 | 0.500 | 0.157 | 0.045 | 0.192 | 0.457 |
| Active Rep×Post | standard_error | 0.449 | 0.473 | 0.486 | 0.732 | 0.781 | 0.805 | 0.406 | 0.429 | 0.441 |
| Active Dem | coefficient | 0.373 | 0.284 | 0.479 | 0.991 | 0.844 | 0.737 | 0.707* | 0.590 | 0.759* |
| Active Dem | standard_error | 0.436 | 0.458 | 0.469 | 0.785 | 0.836 | 0.857 | 0.407 | 0.426 | 0.439 |
| Inactive Dem | coefficient | 1.389*** | 1.285*** | 1.293*** | 1.056 | 1.388* | 1.468* | 1.504*** | 1.498*** | 1.495*** |
| Inactive Dem | standard_error | 0.429 | 0.459 | 0.465 | 0.739 | 0.773 | 0.795 | 0.401 | 0.427 | 0.434 |
| Active Rep | coefficient | -0.646 | -0.635 | -0.736 | -0.092 | -0.359 | -0.128 | -0.518 | -0.509 | -0.565 |
| Active Rep | standard_error | 0.444 | 0.475 | 0.489 | 0.803 | 0.852 | 0.872 | 0.417 | 0.447 | 0.462 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 | model_9 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Observations | 359,784 | 359,784 | 359,778 | 103,241 | 103,241 | 103,241 | 411,989 | 411,989 | 411,977 |
| R-squared | 0.284 | 0.329 | 0.355 | 0.201 | 0.259 | 0.292 | 0.267 | 0.314 | 0.341 |
| Outcome mean | 21.69 | 21.69 | 21.69 | 21.69 | 21.69 | 21.69 | 21.69 | 21.69 | 21.69 |
| N clusters (zip) | 16,215 | 16,215 | 16,216 | 16,215 | 16,215 | 16,216 | 16,215 | 16,215 | 16,216 |

**Note:** This is a variant of Table 5 columns 1-3 focusing on "non-exit" patenters, i.e., those who remain in the patenting profession after the 2008 election. Columns 1-3 define non-exit patenters as those who submit at least one patent application in 2012 and onwards (i.e., in the years following the 3-year post period of the 2008 election); columns 4-6 those who report no changes in job title, seniority, or company on LinkedIn from 2009 through 2011 (i.e., during the 3-year post period); and columns 7-9 the union of the prior two definitions. We only analyze the 2008 election because we lack a sufficiently long post period to define non-exit patenters for the 2016 election. We include all other patenters in our main sample from Table 2 in the regression to increase statistical power; "observations" denotes the number of patenter-year observations in the non-exit sample. We fully saturate the non-fixed-effect regressors in Table 5 columns 1-3 with an indicator for being in the non-exit sample and with an indicator for being in the complement (i.e., the likely exit sample), and report the former coefficients. By adopting this saturated model, we use only non-exit patenters to estimate the reported coefficients, while using all patenters in our main sample (i.e., the sample used in Table 5 columns 1-3) to estimate the fixed effects. Standard errors in parentheses are clustered by zip code. *** 1%, ** 5%, * 10% significance level.

### 3.3 Examining channels: policy vs. political sentiment

In this section, we explore potential channels for the main effects. We begin by further exploring the policy channel and then discuss the political sentiment channel. We finish by comparing two manifestations of political sentiment – economic optimism and mood – via patent citations.

#### 3.3.1 Policy channel: additional evidence

In Section 3.2, we included Firm × Post fixed effects as a first approach to address the possibility that policy drives our results. The idea is that, if a firm specializes in a Democratic or Republican-favored technology – such as renewable energy or traditional energy – by including Firm × Post fixed effects, we are comparing Democrats and Republicans within the same firm. However, it is still possible that a firm could work with multiple technologies, and so could choose to pivot to Republican-favored technologies when a Republican comes to power, and towards Democrat-favored technologies when a Democrat comes to power. In Section 3.2, we addressed this alternative by including Firm × Technology × Post fixed effects.

Here we address the within-firm version of the policy channel in a different way: by testing whether there is evidence supporting its underlying assumptions. These assumptions are that (1) Democrat and Republican patenters specialize in different technologies within firms and (2) firms shift their investment in these technologies based on the outcomes of elections.

We begin in Table 7 by investigating the assumption that inventors sort across different technologies within firms based on their political affiliation. We do this by starting with the sample of all patenters working at firms with less than 1,000 patenters.[^19] We then create a dataset consisting of all possible pairs of patenters working at the same firm and predict whether a pair sharing the same political affiliation is more likely to patent in the same technology class (columns 1-2) or technology subclass (columns 4-5). When Republican, Democrat and Independent investors are paired, there are six possibilities. We call (Republican, Republican), (Democrat, Democrat) and (Independent, Independent) an "Party Match." We call (Democrat, Independent) and (Republican, Independent) a "Match with Independent." Mismatch (i.e., Republican, Democrat) is the reference group. Columns 1 and 2, which include firm fixed effects and demographic controls, indicate no predictability of party affiliation for technology class: the coefficients on Party Match and Match with Independent are economically small and statistically insignificant for both elections. Columns 4 and 5 lead to the same conclusion when predicting technology subclass. However, in columns 3 and 6 – where pairs are not forced to be from the same firm – being affiliated with the same party does predict a pair patenting in the same technology class and subclass. This will lead to aggregation effects which we explore in Section 3.4.

[^19]: We exclude firms with 1,000 or more patenters because the number of all possible pairs of patenters working at the same firm expands beyond computational feasibility.

### Table 7: Predicting whether Inventor-Pairs Patent in the Same Technology

- **Table type:** Regression
- **Unit of observation:** Patenter pair
- **Outcome:** Indicator for whether patenters in a pair share the same most frequently patented technology class (columns 1-3) or subclass (columns 4-6) in the 4-10 years before an election, and zero otherwise
- **Reference group:** Pairs where one is Democrat and the other is Republican (mismatch)
- **Standard errors:** Clustered by firm in columns 1-2 and 4-5; double clustered by firm of each patenter in the pair in columns 3 and 6
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | dependent_variable | pairing | Demographics pair partial | Demographics pair full | Zip pair FE | Firm FE |
|---:|---|---|---|---|---|---|
| 1 | 1(Patent in same class) | Within firm | Yes | No | Yes | Yes |
| 2 | 1(Patent in same class) | Within firm | No | Yes | Yes | Yes |
| 3 | 1(Patent in same class) | Random (regardless of firm) | No | No | No | No |
| 4 | 1(Patent in same subclass) | Within firm | Yes | No | Yes | Yes |
| 5 | 1(Patent in same subclass) | Within firm | No | Yes | Yes | Yes |
| 6 | 1(Patent in same subclass) | Random (regardless of firm) | No | No | No | No |

#### Estimates — Panel A: 2008 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Party match (DD,RR,II) | coefficient | 0.0018 | 0.0017 | 0.0050*** | 0.0018 | 0.0017 | 0.0025*** |
| Party match (DD,RR,II) | standard_error | 0.0015 | 0.0014 | 0.0007 | 0.0014 | 0.0014 | 0.0003 |
| Match with Ind. (DI,RI) | coefficient | -0.0002 | -0.0003 | 0.0070*** | -0.0012 | -0.0013 | 0.0033*** |
| Match with Ind. (DI,RI) | standard_error | 0.0027 | 0.0026 | 0.0011 | 0.0017 | 0.0018 | 0.0004 |

#### Model statistics — Panel A: 2008 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Observations | 15,791,361 | 15,791,361 | 15,122,250 | 15,791,361 | 15,791,361 | 15,122,250 |
| R-squared | 0.5529 | 0.5542 | 0.0002 | 0.4973 | 0.4987 | 0.0001 |
| Outcome mean | .31 | .31 | .04 | .18 | .18 | .01 |

#### Estimates — Panel B: 2016 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Party match (DD,RR,II) | coefficient | 0.0019 | 0.0020 | 0.0048*** | 0.0021 | 0.0022 | 0.0022*** |
| Party match (DD,RR,II) | standard_error | 0.0017 | 0.0017 | 0.0010 | 0.0019 | 0.0019 | 0.0004 |
| Match with Ind. (DI,RI) | coefficient | 0.0001 | 0.0002 | 0.0048*** | -0.0008 | -0.0007 | 0.0023*** |
| Match with Ind. (DI,RI) | standard_error | 0.0018 | 0.0018 | 0.0014 | 0.0016 | 0.0016 | 0.0006 |

#### Model statistics — Panel B: 2016 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Observations | 18,395,607 | 18,395,607 | 15,122,250 | 18,395,607 | 18,395,607 | 15,122,250 |
| R-squared | 0.5526 | 0.5536 | 0.0001 | 0.5054 | 0.5064 | 0.0000 |
| Outcome mean | .36 | .36 | .06 | .22 | .22 | .01 |

**Note:** This table estimates whether the likelihood of two randomly paired patenters working in the same technology class or subclass can be predicted by their respective parties. In columns 1-2 and 4-5, we randomly pair patenters (Democratic, Republican, or Independent) within a firm; for computational tractability, we exclude firms with more than 1,000 patenters. In columns 3 and 6, we randomly select 5,500 patenters from the sample in columns 1-2 and 4-5 respectively, and randomly pair them (regardless of firm affiliation). We only use a subset of patenters for computational tractability: if we had used all patenter pairs from columns 1-2 and 4-5, we would have approximately 1.54 x 10^11 observations. 5,500 is chosen so the number of pairs in columns 3 and 6 approximate those in columns 1-2 and 4-5 in the 2008 election; results are similar had we chosen 6,000 to approximate those in the 2016 election. The outcome is an indicator for whether patenters in a pair share the same most frequently patented technology class (columns 1-3) or subclass (columns 4-6) in the 4-10 years before an election, and zero otherwise. Party match (DD,RR,II) is an indicator for patenters in a pair sharing the same party affiliation, either both Democrats, both Republicans, or both Independents. Match with Ind. (DI,RI) is an indicator for one in a pair being a Democrat or a Republican and the other one being an Independent. The baseline comparison group consists of pairs where one is Democrat and the other is Republican. Columns 1 and 4 control for the inner product of (birth cohort, gender, race, education status) of each patenter in the pair, zip code pair fixed effects, and firm fixed effects; columns 2 and 5 control for the fully interacted characteristics (birth cohort, gender, race, education status) of each patenter in the pair, zip code pair fixed effects, and firm fixed effects; columns 3 and 5 include no controls. Standard errors are clustered by firm in columns 1-2 and 4-5, and double clustered by firm of each patenter in the pair in columns 3 and 6. *** 1%, ** 5%, * 10% significance level. [Conversion note: the original note says "columns 3 and 5 include no controls"; based on the table layout and surrounding text this appears to refer to columns 3 and 6. Preserved as printed and flagged.]

Next, we investigate the assumption that firms adjust their technology focus in response to the policies of the new regime in power. For example, if a Democratic administration comes to power, we should see energy firms patent more in renewable energy and less in fossil-fuel technologies. Figure 3 tests this hypothesis by plotting yearly average firm-year technological similarity, measured at the class and subclass levels. Specifically, for each year, we calculate the cosine similarity between the technology distribution of the firm's patent applications that year and the technology distribution from the prior 5 years. Firms that meaningfully change their patenting technologies around an election year (vs. the preceding five years) will display a drop in measured similarity.

The figure demonstrates no substantive change in the mixture of technologies around elections. Indeed, for both the 2008 and 2016 elections, there is no statistically significant decrease in similarity from the year before the election to the year after. The only trend break we observe is in 2015, when the USPTO moved from using the USPC technology classification system to the CPC system. As noted in Section 2.1, when the USPTO switched to the CPC system, it retroactively reclassified previous patents according to the new system. While we use CPC classifications throughout our analyses, the reclassification is likely imperfect, which accounts for the break in measured similarity around the time of the switch. The fact that we observe a decline in similarity around the change in the classification system suggests that this test would detect a decline in similarity around elections if one had occurred.

### Figure 3: Technological Similarity in Firms' Patent Applications Across Years

- **Panels:** (a) Technology class; (b) Technology subclass
- **Axes:** y-axis "Cosine similarity" (0.5 to 1); x-axis years 2006-2019; vertical lines mark the 2008 and 2016 elections
- **Legend:** Unweighted (solid); Weighted by patents (dashed)

**Note (verbatim):** This figure plots firms' average technology similarity by year, measured by the cosine similarity between the technologies of a firm's patent applications in the prior five years and those in the current year. The similarity value ranges from 0 (completely different) to 1 (identical). The patent application data start in 2001, so we calculate technology similarity starting in 2006. Panel (a) plots the similarity at the technology class level and (b) at the technology subclass level. The solid line represents the unweighted annual average while the dashed line represents the average weighted by a firm's annual number of patent applications. Only firm-year observations with at least three patent applications are included. The USPTO moved from using the USPC technology classification system to the CPC system in 2015, retroactively reclassifying previous patents. We use CPC classifications throughout our analyses, but the reclassification is likely imperfect, which could explain the trend break between 2014 and 2015. We represent this change in the figure by connecting the transition years with a short dashed line.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

Overall, we do not find evidence for a within-firm policy channel generating our findings. First, there is no evidence to support the two key assumptions of the within-firm policy channel: (1) we do not find differences between Republicans and Democrats in the technologies they work on within the same firm, and (2) we do not find evidence of firms differentially changing their mix of technologies around party-switching elections. In addition, our main effects continue to hold when we include high-dimensional fixed effects, such as Firm × Technology (sub)class × Post (see Tables 4 and 5), which compare the productivity of partisans at the same firm working on the same narrowly-defined technology.

#### 3.3.2 Political sentiment channel

Absent a policy channel, the most likely explanation for our results is that Democratic and Republican patenters experience changes in political sentiment around party-changing elections, which in turn affects their productivity. Such changes in sentiment could take two forms: economic optimism and general mood. While these are difficult to distinguish empirically and are not mutually exclusive, our goal is to show that our results are consistent with some type of political sentiment effect on productivity. Below we discuss each channel in turn and provide supporting evidence from surveys. We conclude by analyzing patent citations to provide suggestive evidence distinguishing the channels.

**Economic Optimism.** First, following an election, patenters politically aligned with the losing side may become more pessimistic about economic conditions relative to those on the winning side (Bartels, 2002, Evans and Andersen, 2006, Mian, Sufi, and Khoshkhou, 2023). Because patenters have been shown to capture significant rents from their inventions (Kline et al., 2019), declines in their economic optimism may lead them to exert less effort, in anticipation of lower returns on that effort. One question with this channel is whether it is realistic that long-lasting decisions would be affected by party-changing elections, given that the party in power tends to alternate back and forth. The literature provides some answer to this question, finding that party-changing elections do affect long-lasting decisions such as fertility, entrepreneurship, and firm investment (Dahl, Lu, and Mullins, 2022, Engelberg et al., 2024, Rice, 2023). One reason may be that parties tend to remain in power for a fairly long time. Since 1953 (President Eisenhower), the average length of time a party has stayed in power is 7.6 years, or nearly two election cycles. Given this time horizon, it is plausible that, with reasonable discount rates, long-term decisions will be affected by changes in economic optimism due to the party in power. This is even more true if decision makers are myopic. Indeed, myopia is often pointed to as an explanation for responsiveness to transitory government policies more generally (e.g., Gabaix, 2020).

To explore whether there is evidence for party-based economic optimism, we turn to survey data. Gallup elicits the views of up to 1,000 U.S. adults daily from 2008 to 2018 on topics related to the economy, politics and their well-being. Importantly, respondents identify their political party (38% are Democrats and 37% are Republicans). Although the survey does not identify patenters, we know whether respondents have a graduate degree and whether they are professional workers; we focus on these because most patenters are in these groups.

In Figure 4, we plot the difference in the share of Democratic and Republican respondents ("Dem minus Rep") choosing "Getting better" in response to the question "Right now, do you think that economic conditions in this country, as a whole, are getting better or getting worse?" Panel (a) presents the percentage separately for respondents with and without a graduate degree, while panel (b) presents it for professional workers and non-professional workers. Both panels show that the optimism among Democrats who have patenter-like characteristics rises sharply after the 2008 election and falls markedly after the 2016 election, relative to well educated and professional Republicans.

### Figure 4: Optimism about National Economy: the Gallup U.S. Daily Survey by Education and Occupation

- **Panels:** (a) Share saying economy is *getting better*, by education; (b) Share saying economy is *getting better*, by occupation
- **Axes:** y-axis "Econ getting better: Dem - Rep" (-40 to 80); x-axis quarters 2008q1-2018q1; vertical dashed lines mark the 2008 and 2016 elections
- **Legend:** Panel (a): Graduate+ (solid), Others (dashed); panel (b): Professional (solid), Others (dashed); thick horizontal lines mark the within-administration average for the Graduate+/Professional group

**Note (verbatim):** This figure plots the difference in the share of Democratic and Republican respondents ("Dem minus Rep") answering "Getting better" to the question "Right now, do you think that economic conditions in this country, as a whole, are getting better or getting worse?" in the Gallup U.S. Daily Survey. Values are normalized to their 2008 Q3 levels and units are in percentage points. Panel (a) plots the response by education level and panel (b) by occupation. "Graduate+" refers to respondents who self-identify as having a graduate or higher degree. "Professional" refers to respondents who self-identify as professional workers (lawyer, doctor, scientist, teacher, engineer, nurse, accountant, computer programmer, architect, investment banker, stock brokerage, marketing, musician, artist). The thick horizontal line represents the average value among the Graduate+ group in panel (a) and the Professional group in panel (b).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

The patterns from the Gallup survey are consistent with those from other surveys that elicit Democratic and Republican voters' economic views such as those by Bloomberg and the University of Michigan (see Figure A1). While these other surveys do not allow us to separately identify professionals and those with a graduate degree, they demonstrate persistent partisan differences in economic views across multiple party-changing elections. These differences are larger for questions eliciting forward-looking expectations (over the next 1-5 years, panel c), compared to those about current economic conditions (panels a and b).

Overall, the survey evidence points to sharp divergences across party lines in the predicted directions. The forward-looking expectation evidence is consistent with the economic optimism channel and some myopia: partisans not only believe that economic conditions are worse throughout the time their party is out of power, they also believe that economic conditions will remain worse in the future – even immediately before their party returns to power.

**Mood.** A second channel through which political sentiment may affect productivity is general mood. Those aligned with the losing side may become less happy following the election (Di Tella and MacCulloch, 2005), leading them to experience a decline in their productivity (Banerjee and Mullainathan, 2008, Oswald, Proto, and Sgroi, 2015). One question about this channel is whether it is realistic that mood – and thus patenting – could be affected for years after an election loss.[^20] This question echoes the debate in psychology around the "set point model" of happiness. More recent research has shown that durable changes in happiness do occur in response to external events (e.g., Lucas, 2007, Headey, 2010, Diener, Oishi, and Tay, 2018). In our context, political outcomes may lead to especially durable changes in happiness because the media environment increases the salience of political news on an ongoing basis (e.g., Ford et al., 2023). Relevant to our study, Lench et al. (2019) track voters around the 2016 election and find that Clinton supporters remained below baseline levels of general happiness, and substantially below the level of Republicans, six months after the election (the longest horizon that they examined).

[^20]: Even if changes in happiness were only transitory, there could still be long-lasting effects on innovative output due to the path-dependent nature of technological progress. For example, even if Democrats were only unhappy about the election of Trump for the first year of his administration, their diminished productivity in that year could lead to a decline in innovation subsequently, as innovations build upon one another.

We also find evidence of mood shifts along partisan lines from the Gallup Survey. In Figure 5 we plot the average "Dem minus Rep" difference in response to questions about mood. These are "Did you experience the feeling of worry during a lot of the day yesterday" (panels a and c) and "Did you experience the feeling of enjoyment during a lot of the day yesterday?" (panels b and d). Around both the 2008 and 2016 elections, we find that those affiliated with the losing party report increased levels of worry compared to those with the winning party. Moreover, elevated worry persists throughout the time that their party is out of power. We also observe similar, albeit less robust, patterns for levels of enjoyment.[^21]

[^21]: After 2012 the series becomes more volatile because the questions were asked of a lower share of respondents.

### Figure 5: Mood: the Gallup U.S. Daily Survey by Education or Occupation

- **Panels:** (a) Qs: *Worry yesterday*, by education; (b) Qs: *Enjoyment yesterday*, by education; (c) Qs: *Worry yesterday*, by occupation; (d) Qs: *Enjoyment yesterday*, by occupation
- **Axes:** y-axis "Felt worry yesterday: Dem - Rep" (-15 to 5; panels a, c) or "Felt enjoyment yesterday: Dem - Rep" (-2 to 6; panels b, d); x-axis quarters 2008q1-2017q1; vertical dashed lines mark the 2008 and 2016 elections
- **Legend:** Graduate+ or Professional (solid) vs. Others (dashed); thick horizontal lines mark within-administration averages for the Graduate+/Professional group

**Note (verbatim):** This figure plots the difference in the share of Democratic and Republican respondents ("Dem minus Rep") answering "Yes" to the questions "Did you experience the feeling of *worry* during a lot of the day yesterday?" (panels a and c) and "Did you experience the feeling of *enjoyment* during a lot of the day yesterday?" (panels b and d) in the Gallup U.S. Daily Survey. The thick horizontal line represents the average value among the Graduate+ group in panels (a)-(b) and the Professional group in panels (c)-(d). Everything else follows those in Figure 4. The data series for the Professional group stops after 2017q1 because the questions were not asked of them after that.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

Taken together, the survey evidence suggests that partisans change both their economic optimism and general mood following party-switching presidential elections. In addition, the graphs indicate that these changes persist throughout each administration.

**Economic Optimism vs. Mood: Evidence from Citations.** To further explore whether our results are consistent with a political sentiment channel, we examine the effect of party-changing elections on the quality of the patents produced by Democrats and Republicans. If there are political sentiment effects tied to economic optimism, patenters aligned with the losing side may focus their efforts only on the most promising ideas – which would be robust to the poor economic conditions they expect. Thus, while their likelihood of patenting would decline, the average quality of submitted patents should increase. In contrast, if there are political sentiment effects tied to general mood, we would expect to see a decrease in both the likelihood and quality of patenting on the losing side. This is because patenters aligned with the losing party might be less able to execute on ideas and to generate good ideas.

Following the patent literature, we proxy for the quality of patenters' output using the number of citations their patents receive from other patents. For patents submitted surrounding the 2008 and 2016 elections, we examine their forward citations by 2020.[^22] We measure citations using three metrics: the number of forward cites, scaled citations (the number of forward cites divided by the average number of cites within the patent's technology class and grant year), and normalized citations (the number of forward cites subtracting the average and dividing by the standard deviation of the cites within the patent's technology class and grant year). We then average the citations across all patents an inventor submitted in a year and re-estimate equation 2. Note that this regression sample is conditional on patent activity, i.e., only inventors who submitted patents in a year are included.

[^22]: Forward citations are based on cites after a patent is granted. Patent applications that are rejected or have not been granted by 2020 will have zero citations.

Table 8 column 1 indicates that patents submitted by Democrats following the 2008 election accumulate fewer cites (6% of the mean) than patents submitted by Republicans living in the same area and working in the same technology class at the same time. In contrast, patents submitted by Democrats following the 2016 election accumulate more cites (14% of the mean) than those by their Republican counterparts. The same holds true, albeit with substantially more statistical noise, when we examine scaled and normalized citations, which further account for the variation in citations across technologies and grant years.

Overall, this evidence from citations is consistent with political sentiment effects mainly driven by economic optimism (rather than mood). When Democratic patenters become economically optimistic after Obama's election, they become more likely to patent, but these appear to be of lower average quality, reflecting a lower selectivity of which projects to pursue. When Democratic patenters become economically pessimistic after Trump's election, they produce fewer, but better quality patents, reflecting higher project selectivity.

### Table 8: Election DID Analysis: Patent Citations

- **Table type:** Regression
- **Sample:** Patenters who submit at least one patent in a year (only they can receive citations); patenter-year panel
- **Standard errors:** Clustered by zip code, in parentheses
- **Demographics, Zip FE, Technology Class×Post FE:** Included in all columns
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | dependent_variable | State×Post FE |
|---:|---|---|
| 1 | # Citations | No |
| 2 | # Citations | Yes |
| 3 | Scaled # | No |
| 4 | Scaled # | Yes |
| 5 | Normalized # | No |
| 6 | Normalized # | Yes |

#### Estimates — Panel A: 2008 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Dem×Post | coefficient | -0.595** | -0.335 | -0.053* | -0.047 | -0.020** | -0.017* |
| Dem×Post | standard_error | 0.274 | 0.290 | 0.032 | 0.032 | 0.010 | 0.010 |
| Dem | coefficient | 0.126 | 0.010 | 0.056** | 0.053** | 0.021** | 0.020** |
| Dem | standard_error | 0.315 | 0.316 | 0.024 | 0.023 | 0.008 | 0.008 |

#### Model statistics — Panel A: 2008 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Observations | 216,685 | 216,685 | 216,684 | 216,684 | 216,682 | 216,682 |
| R-squared | 0.153 | 0.154 | 0.103 | 0.104 | 0.107 | 0.108 |
| Outcome mean | 10.79 | 10.79 | 1.28 | 1.28 | .11 | .11 |
| N clusters (zip) | 12,834 | 12,834 | 12,834 | 12,834 | 12,834 | 12,834 |

#### Estimates — Panel B: 2016 election

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Dem×Post | coefficient | 0.289** | 0.355*** | 0.088* | 0.085* | 0.009 | 0.015* |
| Dem×Post | standard_error | 0.113 | 0.118 | 0.047 | 0.050 | 0.008 | 0.009 |
| Dem | coefficient | -0.277** | -0.298*** | -0.053 | -0.052 | -0.008 | -0.010 |
| Dem | standard_error | 0.111 | 0.114 | 0.033 | 0.034 | 0.007 | 0.007 |

#### Model statistics — Panel B: 2016 election

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Observations | 235,347 | 235,347 | 235,307 | 235,307 | 235,307 | 235,307 |
| R-squared | 0.137 | 0.141 | 0.083 | 0.084 | 0.094 | 0.094 |
| Outcome mean | 2.09 | 2.09 | 1.1 | 1.1 | .03 | .03 |
| N clusters (zip) | 12,658 | 12,658 | 12,657 | 12,657 | 12,657 | 12,657 |

**Note:** This table reports estimates from DID analyses comparing the number of patent citations to Democratic and Republican inventors' patents around the 2008 and 2016 presidential elections. The sample is composed of patenters who submit at least one patent in a year, as only they can receive citations. The outcomes in columns 1-2, columns 3-4, and columns 5-6 are, respectively, (i) an inventor's average number of citations across the patents they submitted in each year (# Citations), (ii) the average number divided by the technology class and grant year mean (Scaled #), and (iii) the average number after subtracting the mean and dividing by the standard deviation of the technology class and grant year (Normalized #). Variable definitions and specifications mirror those in Table 2 columns 4 and 6. Standard errors in parentheses are clustered by zip code. *** 1%, ** 5%, * 10% significance level.

### 3.4 Political segregation and aggregate effects

Thus far, we have shown that election outcomes affect the productivity of partisan patenters. Here we consider whether these individual-level effects aggregate up to the technology or firm levels. If some inventors become less productive while others become more productive following an election, it is possible that the individual-level effects offset in the aggregate. However, if certain technologies or firms are disproportionately Democrat or Republican, the effects will not cancel out. For this reason, we begin by investigating whether there is political segregation across firms and technologies.

Table 9 documents which technologies and firms disproportionately employ patenters registered as either Republicans or Democrats. Panel A classifies patenters according to the broadest possible technology group (nine "sections"), while panel B deploys a finer classification (123 classes). These panels document substantial political segregation across technologies. For example, in Biochemistry there are 41.6 percentage points more Democratic patenters than Republican ones. Organic Chemistry, Nanotechnology and Combinatorial Technology also heavily favor Democratic patenters. However, in the Weapons technology class, Republican patenters outnumber Democratic ones by 45.3 percentage points. Ammunition, Construction and Hydraulic Engineering also heavily favor Republican patenters. In addition, there are technology classes that show no meaningful partisan differences, such as Dyes, Sports and Apparel.

Panel C presents a similar exercise for the top ten publicly traded firms with over 1,000 party-identified patenters. Google, Yahoo and Microsoft all have at least 65 percentage points more Democratic than Republican patenters, while Halliburton, Kimberly Clark and Caterpillar are Republican-leaning by over 35 percentage points. These rankings are consistent with Silicon Valley firms being Democratic (FiveThirtyEight, 2016) and defense/weapons firms skewing Republican, such as Halliburton where former Republican Vice President Dick Cheney served as Chairman and CEO. In summary, we find substantial political clustering in the cross-section of firms and technologies.

### Table 9: Party Concentration by Technology and by Firm

- **Table type:** Descriptive (party-share differences)
- **Measure:** %Dem-Rep — the difference in the shares of Democrat and Republican inventors among partisans, by technology section, technology class, or firm, using USPTO patent applications submitted between 2001 and 2019. Positive values are Democrat-leaning; negative values are Republican-leaning.

#### Panel A: By technology section

| lean | name | pct_dem_minus_rep |
|---|---|---:|
| Democrat-leaning | Chemistry; Metallurgy | 18.9 |
| Democrat-leaning | Physics | 15.0 |
| Democrat-leaning | Electricity | 11.0 |
| Republican-leaning | Fixed Constructions | -33.9 |
| Republican-leaning | Mech. Eng.; Lighting; Heating; Weapons; Blasting | -23.1 |
| Republican-leaning | Performing Operations; Transporting | -15.9 |
| Republican-leaning | Textiles; Paper | -15.0 |
| No lean | Human Necessities | 1.2 |

#### Panel B: By technology class

| lean | name | pct_dem_minus_rep |
|---|---|---:|
| Democrat-leaning | Combinatorial Technology | 47.5 |
| Democrat-leaning | Biochemistry; Beer; Spirits; Wine; Vinegar and etc | 41.6 |
| Democrat-leaning | Organic Chemistry | 36.6 |
| Democrat-leaning | Nanotechnology | 29.8 |
| Democrat-leaning | Musical Instruments; Acoustics | 27.6 |
| Democrat-leaning | Information And Communication Technology | 21.8 |
| Democrat-leaning | Computing; Calculating; Counting | 21.2 |
| Democrat-leaning | Electric Communication Technique | 19.8 |
| Democrat-leaning | Microstructural Technology | 18.8 |
| Democrat-leaning | Crystal Growth | 18.0 |
| Republican-leaning | Weapons | -45.3 |
| Republican-leaning | Ammunition; Blasting | -42.2 |
| Republican-leaning | Construction of Roads, Railways, or Bridges | -41.5 |
| Republican-leaning | Hydraulic Engineering; Foundations; Soil Shifting | -39.5 |
| Republican-leaning | Saddlery; Upholstery | -37.8 |
| Republican-leaning | Earth Drilling; Mining | -37.3 |
| Republican-leaning | Presses | -36.5 |
| Republican-leaning | Crushing, Pulverising, or Disintegrating; Prep. of Grain | -35.1 |
| Republican-leaning | Butchering; Meat Treatment; Processing Poultry or Fish | -35.0 |
| Republican-leaning | Making Articles of Paper | -34.8 |
| No lean | Dyes; Paints; Polishes; Natural Resins | 0.0 |
| No lean | Hand or Travelling Articles | 0.1 |
| No lean | Signalling | 0.3 |
| No lean | Sports; Games; Amusements | -0.5 |
| No lean | Machines or Engines for Liquids | -0.6 |
| No lean | Sugar Industry | -0.7 |
| No lean | Controlling; Regulating | -0.8 |
| No lean | Wearing Apparel | 0.9 |
| No lean | Organic Macromolecular Compounds | 1.4 |
| No lean | Checking-Devices | -1.4 |

#### Panel C: By firm

| lean | name | pct_dem_minus_rep |
|---|---|---:|
| Democrat-leaning | Google Inc. | 70.4 |
| Democrat-leaning | Yahoo Inc. | 65.6 |
| Democrat-leaning | Microsoft Corp. | 65.2 |
| Democrat-leaning | Genentech Inc. | 63.7 |
| Democrat-leaning | Apple Inc. | 60.0 |
| Democrat-leaning | Oracle Int Corp. | 44.4 |
| Democrat-leaning | Merck & Co Inc. | 39.0 |
| Democrat-leaning | Sun Microsystems Inc. | 35.6 |
| Democrat-leaning | Cisco Tech Inc. | 33.3 |
| Democrat-leaning | Qualcomm Inc. | 32.3 |
| Republican-leaning | Halliburton Energy Services Inc. | -39.3 |
| Republican-leaning | Baker Hughes Inc. | -38.9 |
| Republican-leaning | Kimberly Clark Worldwide Inc. | -36.9 |
| Republican-leaning | Caterpillar Inc. | -34.6 |
| Republican-leaning | Illinois Tool Works Inc. | -33.8 |
| Republican-leaning | 3M Innovative Properties Co | -31.0 |
| Republican-leaning | Delphi Tech Inc. | -29.2 |
| Republican-leaning | Micron Tech Inc. | -28.5 |
| Republican-leaning | Honeywell Int Inc. | -23.7 |
| Republican-leaning | Lockheed Martin Corp. | -21.3 |
| No lean | Dow Global Tech LLC | 0.9 |
| No lean | Chevron USA Inc. | -1.3 |
| No lean | GM Global Tech Operations LLC | 2.0 |
| No lean | United Tech Corp. | -2.8 |
| No lean | The Procter & Gamble Co | -2.9 |
| No lean | Verizon Patent & Licensing Inc | 3.9 |
| No lean | Dell Prod LP | -4.8 |
| No lean | Bank of America Corp. | -4.8 |
| No lean | Motorola Inc. | 5.3 |
| No lean | Boston Sci Scimed Inc. | -7.3 |

**Note:** This table reports the difference in the shares of Democrat and Republican inventors among partisans by technology section, by technology class, or by firm using USPTO patent applications submitted between 2001 and 2019. Panel A reports the difference for each technology section in our sample. Panel B reports the difference for the ten technology classes with the greatest difference (i) between Democrat and Republican shares ("Democrat-leaning"), (ii) between Republican and Democrat shares ("Republican-leaning") and (iii) between the two with the least difference ("No lean"); panel C does the same for the ten publicly traded firms with >1,000 inventors in our sample in each of the three "lean" categories.

Consistent with evidence from U.S. C-suites (Fos, Kempf, and Tsoutsoura, 2023), we find increasing segregation in the time series. For each year we construct two standard measures of segregation: the isolation and dissimilarity indices, at the technology subclass or the firm level.[^23] The isolation index captures the extent to which Republican patenters disproportionately cluster in a technology or firm with other Republican patenters. An isolation index of one represents the maximum level of segregation, meaning that partisan patenters only patent in technology subclasses or work in firms where 100% of patenters match their partisanship. The dissimilarity index instead captures the share of one group of partisans that would have to be moved to produce an unsegregated distribution.

[^23]: We calculate isolation index and dissimilarity index in year $t$ following White (1986) and Cutler, Glaeser, and Vigdor (1999), respectively:
$$
Isolation_t = \frac{\sum_{j\in J}\frac{Rep_{jt}}{Rep_t}\times\frac{Rep_{jt}}{total_{jt}} - \frac{Rep_t}{total_t}}{1 - \frac{Rep_t}{total_t}} \tag{4}
$$
$$
Dissimilarity_t = \frac{1}{2}\sum_{j\in J}\left|\frac{Rep_{jt}}{Rep_t} - \frac{Dem_{jt}}{Dem_j}\right| \tag{5}
$$
where $Rep_{jt}$ ($Dem_{jt}$) is the number of Republican (Democractic) patenters in technology subclass or firm $j$ in year $t$; $total_{jt}$ the total number of patenters in $j$ in year $t$; $Rep_t$ ($Dem_t$) the number of all Republican (Democratic) patenters in year $t$; and $total_t$ the number of all Republican and Democratic patenters in year $t$. [Conversion note: the denominator subscript $Dem_j$ in equation 5 is transcribed as printed in the original.]

Figure 6 panels (a) and (b) plot the isolation and dissimilarity indices. These indices provide similar evidence of increasing political segregation. For example, while relatively flat before 2016, the subclass-level dissimilarity index increased by over 10% by the end of the sample, with a similar pattern for the firm-level index.

Panel (c) examines segregation at the team level, because teamwork plays a central role in the creation of patents (Jaravel, Petkova, and Bell, 2018). Specifically, it plots the probability of mixed-party teams applying for a patent in each year relative to the probability in the base year 2004, controlling for zip code and technology class fixed effects as well as team characteristics.[^24] As an additional control we include the predicted annual likelihood of forming a mixed-party team with N members in each technological subclass ("subclass control") or across the U.S. ("US control)," by calculating the share of mixed party teams that result from randomly picking N patenters within the subclass or across the U.S. The likelihood of a mixed team submitting a patent fell steadily from 36% in 2004 to 31% in 2019. After controls, the decrease becomes 3 percentage points, or 8% of the 2004 level. Panel (d) shows the same pattern as in panel (c) using patent grants. These segregation patterns may be due to sorting of partisans into increasingly segregated firms (as suggested by panels a and b), or by sorting into homogeneous teams within the same firm. Controlling for the predicted probability of a mixed team within a firm (the triangle-dashed line in panel d) indicates that there has only been a moderate increase in sorting within the same firm. Thus, most of the decline in mixed teams is driven by across-firm sorting, consistent with our results in Table 7.[^25]

[^24]: The team characteristics are team size, sex, education, race and age group; all as a share of the team.

[^25]: We are able to control for within-firm probability of mixed teams for patent grants, but not applications, because grants have much better assignee (firm) information.

### Figure 6: Partisan Affiliation and Clustering by Technology, Firm, or Team

- **Panels:** (a) Isolation index; (b) Dissimilarity index; (c) Prob. mixed-party application teams; (d) Prob. mixed-party grant teams
- **Axes:** Panels (a)-(b): left y-axis "Subclass segregation (%)", right y-axis "Firm segregation (%)", x-axis years 2004-2019; panels (c)-(d): y-axis "P(mixed party team) (%)" (-4 to 0), x-axis years 2004-2019
- **Legend:** Panels (a)-(b): Subclass level (solid), Firm level (dotted); panel (c): US control, Subclass control; panel (d): US control, Subclass control, Firm control (triangle-dashed)

**Note (verbatim):** This figure plots inventors' segregation along party lines by technology subclass, firm, or team over time. Panel (a) plots the isolation index (White 1986) and panel (b) the dissimilarity index (Cutler, Glaeser, and Vigdor 1999) for technology subclasses and firms. Only technology subclasses and firms with more than 10 Republican or Democratic inventors in a year are included. Panels (c) and (d) plot the probability of mixed-party teams (and 90 percent confidence intervals) relative to 2004, using USPTO patent application data and grant data, respectively. Both panels control for zip code fixed effects, technology class fixed effects, and team characteristics (i.e., team size, fraction of men, fraction of college educated, fraction of a certain race, fraction in a certain age group). Different lines in each panel result from different controls used in predicting the likelihood of forming a mixed-party team: *US control*, *subclass control*, and *firm control* refer to controlling for the likelihood of forming a mixed-party team by randomly picking N inventors (team size) in the US, in a technological subclass, and in a firm, respectively. Panel (c) does not show results for *firm control* because a large fraction of patent applications lack firm information. Standard errors are clustered by zip code. Units are in percentage points.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

Given political segregation at the team, firm and technology levels, shocks to political sentiment (e.g., from an election outcome) should have effects on the innovative activity of entire sectors. As an example, if Republicans, who are disproportionately clustered in the Weapons subclass, become pessimistic after the 2008 election, this effect should aggregate to less innovative activity in Weapons relative to Biochemistry, where Democrats outnumber Republicans by more than 2:1. While the political segregation we have shown implies post-election effects at the technology level, it is nonetheless of interest to explore them empirically. However, we caution that aggregate analysis does not allow us to address the endogeneity concern that policy may directly affect investment in technologies, which we address in our individual-level analysis (with firm-time and firm-technology-time fixed effects and individual measures of partisan intensity).

Figure 7 examines whether Democratic technologies register more granted patents relative to Republican technologies following the 2008 election. We focus on granted patents as these are the innovations that matter for technological progress, and on the 2008 election because our data ends in 2020, making the data on granted patents following the 2016 election too sparse. Panels (a) and (b) present evidence for technology subclasses, while (c) and (d) focus on classes. Panels (a) and (c) display the annual difference in the number of patent grants between Democratic and Republican technologies, while panels (b) and (d) present the difference in the standardized number (subtracting the mean and dividing by the standard deviation). All four panels tell the same story: innovative activity in Democratic technologies steadily increased relative to Republican ones following the 2008 election, with no discernable pre-trends. Subclasses are more politically segregated, generating larger effect sizes and tighter confidence intervals compared to the class-level evidence, which is not statistically significant. For example, in panel (b) we see Democratic subclasses experience a standard deviation increase in patenting relative to Republican ones by 2010, while it takes until 2015 to reach this point estimate at the class-level in panel (d).

### Figure 7: Political Mismatch and Number of Granted Patents by Technology Class and Subclass

- **Panels:** (a) Subclass-level granted patents; (b) Subclass-level granted patents (std); (c) Class-level granted patents; (d) Class-level granted patents (std)
- **Axes:** y-axis "Dem - Rep, # granted patents" (panels a, c) or "Dem - Rep, # granted patents (std)" (panels b, d); x-axis calendar years 2005-2015; vertical dashed line at 2008

**Note (verbatim):** This figure plots estimates (and 90% confidence intervals) of the effect of political alignment on the number of granted patents at the technology (sub)class-level around the 2008 presidential election. In this figure we assign a granted patent to its application year. Democratic technologies are those with an above-median share of Democrats among all inventors actively patenting in the 10 through 4 years preceding the 2008 election. Republican technologies are similarly defined. Only technologies with at least eight actively patenting inventors before the election are assigned a partisan leaning. The outcome for panel (a) is the number of eventually-granted patents submitted in each subclass each year. The outcome in panel (b) standardizes by the pre-election subclass mean and standard deviation. Panels (c) and (d) repeat the exercise at the class level. Specifications follow Figure 2 panel (a) while controlling for technology subclass (or class) fixed effects and class (or section)-by-year fixed effects. Standard errors are clustered by subclass (or class).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

Appendix Table A9 presents DID estimates corresponding to the subclass-level analysis in panels (a) and (b) using various definitions of Republican and Democratic technologies. Columns 1-2 compare technologies above vs. below median (as in the panels), columns 3-4 compare top vs. bottom tercile, and columns 5-6 compare quartiles. Results are very similar across comparisons. In the three years following the 2008 election, Democratic subclasses on average submitted 42 (or a standard deviation) more patent applications that are eventually granted relative to Republican subclasses in each year. Aggregating across all subclasses in our sample, the effect amounts to a difference of nearly 10,600 (=42×625/2) patent grants per year or 5.6% of annual total patent grants in the U.S. during our sample period.

## 4. Conclusion

Political affiliation has become an increasingly important part of American identity (Dias and Lelkes, 2022) and predictive of a wide range of beliefs and behaviors (Pew, 2017). This paper documents an effect of political identity on worker productivity: when workers' political party wins a party-changing presidential election, they become relatively more productive, whereas those on the losing side become relatively less productive.

While we find this effect among patenters – where we can measure productivity via the number of patents they produce – many unanswered questions remain. For example, if the productivity declines we document after a political loss reflect reduced effort following increased pessimism, we would expect declines in productivity regardless of occupation. Is this the case, or are there some occupations whose productivity is particularly vulnerable to political regime changes?

In addition, as Americans have become increasingly partisan (Pew, 2017), there is growing concern that workplaces may become politically homogeneous. We find a pattern of increasing political homogeneity among patenters and that this aggregates to effects on the rate of progress across technologies. If current polarization trends continue, we should see even larger aggregate productivity effects following election outcomes or other shocks to political sentiment.

## References

Aghion, P., and P. Howitt. 1992. A model of growth through creative destruction. *Econometrica* 323–51.

Allcott, H., L. Braghieri, S. Eichmeyer, and M. Gentzkow. 2020. The welfare effects of social media. *American Economic Review* 110:629–76.

Babina, T., A. Bernstein, and F. Mezzanotti. 2023. Financial disruptions and the organization of innovation: Evidence from the great depression. *Review of Financial Studies* 36:4271–317.

Balsmeier, B., A. Chavosh, G.-C. Li, G. Fierro, K. Johnson, A. Kaulagi, D. O'Reagan, B. Yeh, and L. Fleming. 2015. Automated disambiguation of US patent grants and applications. Working paper.

Banerjee, A. V., and S. Mullainathan. 2008. Limited attention and income distribution. *American Economic Review* 98:489–93.

Bartels, L. M. 2002. Beyond the running tally: Partisan bias in political perceptions. *Political Behavior* 24:117–50.

Bena, J., and E. Simintzi. 2023. Machines could not compete with Chinese labor: Evidence from US firms' innovation. Working Paper.

Bernstein, A., S. B. Billings, M. T. Gustafson, and R. Lewis. 2022a. Partisan residential sorting on climate change risk. *Journal of Financial Economics* 146:989–1015.

Bernstein, S. 2015. Does going public affect innovation? *Journal of Finance* 70:1365–403.

Bernstein, S., R. Diamond, A. Jiranaphawiboon, T. McQuade, and B. Pousada. 2022b. The contribution of high-skilled immigrants to innovation in the United States. NBER Working Paper 30797.

Bernstein, S., T. McQuade, and R. R. Townsend. 2021. Do household wealth shocks affect productivity? Evidence from innovative workers during the Great Recession. *Journal of Finance* 76:57–111.

Billings, S. B., E. Chyn, and K. Haggag. 2021. The long-run effects of school racial diversity on political identity. *American Economic Review: Insights* 3:267–84.

Bloom, N., S. J. Davis, and Y. Zhestkova. 2021. Covid-19 shifted patent applications toward technologies that support working from home. *AEA Papers and Proceedings* 111:263–6.

Bloom, N., C. I. Jones, J. Van Reenen, and M. Webb. 2020. Are ideas getting harder to find? *American Economic Review* 110:1104–44.

Brown, J. R., and R. D. Enos. 2021. The measurement of partisan sorting for 180 million voters. *Nature Human Behaviour* 1–11.

Colonnelli, E., V. P. Neto, and E. Teso. 2022. Politics at work. NBER Working Paper 30182.

Cookson, J. A., J. E. Engelberg, and W. Mullins. 2020. Does partisanship shape investor beliefs? Evidence from the COVID-19 pandemic. *Review of Asset Pricing Studies* 10:863–93.

Cowen, T. 2011. The great stagnation: How america ate all the low-hanging fruit of modern history, got sick, and will (eventually) feel better. Penguin.

Cullen, J. B., N. Turner, and E. Washington. 2021. Political alignment, attitudes toward government, and tax evasion. *American Economic Journal: Economic Policy* 13:135–66.

Cutler, D. M., E. L. Glaeser, and J. L. Vigdor. 1999. The rise and decline of the American ghetto. *Journal of Political Economy* 107:455–506.

Dagostino, R., J. Gao, and P. Ma. 2023. Partisanship in loan pricing. *Journal of Financial Economics* 150:103717–.

Dahl, G. B., R. Lu, and W. Mullins. 2022. Partisan fertility and presidential elections. *American Economic Review: Insights* 4:473–90.

Di Tella, R., and R. MacCulloch. 2005. Partisan social happiness. *Review of Economic Studies* 72:367–93.

Dias, N., and Y. Lelkes. 2022. The nature of affective polarization: Disentangling policy disagreement from partisan identity. *American Journal of Political Science* 66:775–90.

Diener, E., S. Oishi, and L. Tay. 2018. Advances in subjective well-being research. *Nature Human Behaviour* 2:253–60.

Engelberg, J., J. Guzman, R. Lu, and W. Mullins. 2024. Partisan entrepreneurship. *Journal of Finance* (Forthcoming).

Evans, G., and R. Andersen. 2006. The political conditioning of economic perceptions. *The Journal of Politics* 68:194–207.

Farre-Mensa, J., D. Hegde, and A. Ljungqvist. 2020. What is a patent worth? Evidence from the US patent "lottery". *Journal of Finance* 75:639–82.

FiveThirtyEight. 2016. Nearly All Of Silicon Valley's Political Dollars Are Going To Hillary Clinton. https://fivethirtyeight.com/features/nearly-all-of-silicon-valleys-political-dollars-are-going-to-hillary-clinton/ (accessed August 24, 2022).

Ford, B. Q., M. Feinberg, B. Lassetter, S. Thai, and A. Gatchpazian. 2023. The political is personal: The costs of daily politics. *Journal of Personality and Social Psychology* 125:1–.

Fos, V., E. Kempf, and M. Tsoutsoura. 2023. The Political Polarization of Corporate America. NBER Working Paper 30183.

Gabaix, X. 2020. A Behavioral New Keynesian model. *American Economic Review* 110:2271–327.

Ganguli, I., J. Lin, and N. Reynolds. 2020. The paper trail of knowledge spillovers: Evidence from patent interferences. *American Economic Journal: Applied Economics* 12:278–302.

Gordon, R. J. 2016. The rise and fall of american growth. Princeton University Press.

Headey, B. 2010. The set point theory of well-being has serious flaws: on the eve of a scientific revolution? *Social Indicators Research* 97:7–21.

Hombert, J., and A. Matray. 2018. Can innovation help US manufacturing firms escape import competition from China? *Journal of Finance* 73:2003–39.

Jaravel, X., N. Petkova, and A. Bell. 2018. Team-specific capital and innovation. *American Economic Review* 108:1034–73.

Jones, B. F. 2009. The burden of knowledge and the "death of the renaissance man": Is innovation getting harder? *Review of Economic Studies* 76:283–317.

Kempf, E., and M. Tsoutsoura. 2021. Partisan professionals: Evidence from credit rating analysts. *Journal of Finance* 76:2805–56.

Kline, P., N. Petkova, H. Williams, and O. Zidar. 2019. Who profits from patents? Rent-sharing at innovative firms. *Quarterly Journal of Economics* 134:1343–404.

Kogan, L., D. Papanikolaou, A. Seru, and N. Stoffman. 2017. Technological innovation, resource allocation, and growth. *Quarterly Journal of Economics* 132:665–712.

Kortum, S. S. 1997. Research, patenting, and technological change. *Econometrica* 1389–419.

Krieger, J., D. Li, and D. Papanikolaou. 2022. Missing novelty in drug development. *Review of Financial Studies* 35:636–79.

Lench, H. C., L. J. Levine, K. A. Perez, Z. K. Carpenter, S. J. Carlson, and T. Tibbett. 2019. Changes in subjective well-being following the us presidential election of 2016. *Emotion* 19:1–.

Liu, E., and S. Ma. 2021. Innovation networks and R&D allocation. NBER Working Paper 29607.

Lucas, R. E. 2007. Adaptation and the set-point model of subjective well-being: Does happiness change after major life events? *Current Directions in Psychological Science* 16:75–9.

Manso, G. 2011. Motivating innovation. *Journal of Finance* 66:1823–60.

McCartney, W. B., J. Orellana-Li, and C. Zhang. 2024. Political polarization affects households' financial decisions: Evidence from home sales. *Journal of Finance* 79:795–841.

Meeuwis, M., J. A. Parker, A. Schoar, and D. Simester. 2022. Belief disagreement and portfolio choice. *Journal of Finance* 77:3191–247.

Mian, A., A. Sufi, and N. Khoshkhou. 2023. Partisan bias, economic expectations, and household spending. *Review of Economics and Statistics* 105:493–510.

Mokyr, J. 1992. The lever of riches: Technological creativity and economic progress. Oxford University Press.

Nanda, R., and M. Rhodes-Kropf. 2013. Investment cycles and startup innovation. *Journal of Financial Economics* 110:403–18.

Oswald, A. J., E. Proto, and D. Sgroi. 2015. Happiness and productivity. *Journal of Labor Economics* 33:789–822.

Pew. 2017. The partisan divide on political values grows even wider. Working Paper, Pew Research Center.

———. 2018. Commercial voter files and the study of US politics. Working Paper, Pew Research Center.

Rice, A. B. 2023. Executive partisanship and corporate investment. *Journal of Financial and Quantitative Analysis* 1–30.

Romer, P. M. 1990. Endogenous technological change. *Journal of Political Economy* 98:S71–S102.

Spenkuch, J. L., E. Teso, and G. Xu. 2023. Ideology and performance in public organizations. *Econometrica* 91:1171–203.

White, M. J. 1986. Segregation and diversity measures in population distribution. *Population index* 198–221.

## Appendix

### A. USPTO Name Disambiguation

**Assignee Name Disambiguation**

- We collect all patent grants and applications with non-missing assignees corresponding to firms (asgtype=2 or asgtype=3).
- We standardize all assignee names using the name standardization algorithm developed by the NBER patent data project. This replaces different variations of common words with one standardized version and also standardizes capitalization, punctuation, etc. (https://sites.google.com/site/patentdataproject/)
  - The NBER name standardization algorithm creates a standardized name and also a stem name (which excludes words like "Incorporated," "LLC," etc.).
- We also standardize and parse assignee location names (into city, state, country) by running them through the Google geocode API.
- Initial assignee IDs are then generated based on the standardized assignee names (assignee_id). That is, two patents assigned to assignees with the exact same standardized name are given the same value of assignee_id.
- These initial assignee IDs are then "smoothed" (i.e. multiple values of assignee_id are combined into one) several times based on alternative ID variables containing further disambiguating information.
- This smoothing process is recursive, such that if any two values of assignee_id are linked by an alternative ID (either directly or indirectly), they are combined. For example, two patents with assignee_id=104 and assignee_id=2007 may be linked by the same alternative ID (e.g. alt_id=57). And two different patents with assignee_id=2007 and assignee_id=9782 may also be linked by the same alternative ID (e.g., alt_id=3450). In this case, after smoothing based on alt_id, all patents that had assignee_id=104 or assignee_id=2007 or assignee_id=9782 would now have assignee_id=104.
- Note that the alternative IDs do not need to be non-missing for all observations. Nonetheless, an alternative ID may end up changing assignee_id, even for observations for which the alternative ID is missing. o In the example above, there may be an observation with assignee_id==9782 and alt_id missing. Nonetheless, after smoothing, assignee_id would change to 104 for that observation. [Conversion note: the stray "o" before "In the example above" appears in the original, likely a sub-bullet marker from the source document.]
- The alternative IDs used for smoothing are as follows, with all variables required to be non-missing:
  1. The assignee ID developed by the NBER patent project for granted patents from 1976-2006. https://sites.google.com/site/patentdataproject/
  2. Tuples based on assignee stem name and assignee city
  3. Tuples based on assignee short name (first 4 non-white space characters, excluding "THE"), inventor first name, inventor last name, inventor city, and assignee city. The assignee name cannot contain the "UNIV"
  4. Tuples based on assignee acronym (first letters of each word in stem name), inventor first name, inventor last name, inventor city, and assignee city. The assignee acronym must be at least 3 characters long. The assignee name cannot contain the "UNIV"
  5. Tuples based on assignee stem name, patent application number, and patent application date. This links assignees from a patent application to assignees from a subsequent patent grant

**Inventor Name Disambiguation**

- Inventor names are disambiguated using a similar methodology to assignee names.
- We collect all patent grants and applications with non-missing inventors.
- We standardize and parse inventor names
  - We take the first "word" in the name to be their first name and the last "word" in the name to be the last name (where words are separated by white space), except for certain exceptions where the last two words are consider a middle name (e.g., last names beginning with the word "AL," "DA," "DE," "DEL," "DELLA," "DER," "DI," "DU," "EL," etc.). [Conversion note: "are consider" appears in the original.]
  - All other words in between the first and last are considered middle names o In some cases we only observe middle initials or no middle name/initial information. [Conversion note: the stray "o" appears in the original, likely a sub-bullet marker from the source document.]
- We standardize and parse inventor locations using the google geocode API..
- Initial inventor IDs are then generated based on the following tuples, with missing values treated as values.
  - First name, middle names (all), middle initials (all), last name, inventor city, assignee_id
- These initial inventor IDs are then smoothed based on the following tuples. Missing values treated as values for tuple 1, and all variables are required to be non-missing for tuples 2-11.
  1. First name, middle names (all), middle initials (all), last name, inventor city, technology section
  2. First name, middle initial (first), last name, inventor city, assignee_id
  3. First name, middle initial (first), last name, inventor city, technology section
  4. First name, middle name (first), last name, inventor location
  5. First name, middle name (first), last name, technology section, inventor country
  6. First name, middle initials (all), last name, inventor city
  7. First name, middle initials (all), last name, technology section, inventory country [Conversion note: "inventory country" appears in the original; likely "inventor country."]
  8. First name, last name, application number, application date
  9. First name, application number, application date, inventor sequence number
  10. Last name, application number, application date, inventor sequence number
  11. First name, middle names (all), last name

### Figure A1: Optimism about the National Economy: Additional Survey Evidence

- **Panels:** (a) Bloomberg Consumer Comfort Index; (b) University of Michigan Survey of Consumers: Index of Current Economic Conditions; (c) University of Michigan Survey of Consumers: Index of Consumer Expectations
- **Axes:** y-axis "Democrat - Republican (% positive response)" in panel (a) and "Democrat - Republican (positive response)" in panels (b)-(c); x-axis quarters 1990q3-2022q1 in panel (a) and 2006q3-2024q3 in panels (b)-(c)
- **Annotations:** Election markers (1992, 2000, 2008, 2016, 2020 in panel a; 2008, 2016, 2020 in panels b-c) with presidential administration labels (Clinton, G.W. Bush, Obama, Trump, Biden) and dashed horizontal lines for administration averages

**Note (verbatim):** This figure plots the difference in the ratings of Democratic and Republican respondents ("Democrat - Republican") on the national economy from two surveys. For panel (a), respondents for the Bloomberg survey are asked to rate (i) the national economy, (ii) their personal finances, and (iii) the buying climate as "Excellent," "Good," "Not so Good," or "Poor." The index is calculated as the quarterly average fraction of positive responses ("Good" or "Excellent") across the three questions. Panel (b) is a composite index of two questions from the University of Michigan Survey of Consumers: (i) "We are interested in how people are getting along financially these days. Would you say that you (and your family living there) are better off or worse off financially than you were a year ago?" (ii) "About the big things people buy for their homes–such as furniture, a refrigerator, stove, television, and things like that. Generally speaking, do you think now is a good or bad time for people to buy major household items?" Panel (c) is a composite index of three questions from the University of Michigan Survey of Consumers: (i) "Now looking ahead–do you think that a year from now you (and your family living there) will be better off financially, or worse off, or just about the same as now?" (ii) "Now turning to business conditions in the country as a whole–do you think that during the next twelve months we'll have good times financially, or bad times, or what?" (iii) "Looking ahead, which would you say is more likely–that in the country as a whole we'll have continuous good times during the next five years or so, or that we will have periods of widespread unemployment or depression, or what?" Note that the underlining is present in the original document.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Table A1: Summary Statistics by Election – Democrats vs. Republicans

- **Units:** Percentage points (pp); Mean and SD refer to the annual probability of submitting a patent conditional on the row characteristic; %Sample is the fraction of patenters with each characteristic.
- **Column groups:** Full sample (Mean, SD, %Sample); Democrat (Mean, SD, %Sample); Republican (Mean, SD, %Sample)

#### Panel A: 2008 election

| Characteristic | Full Mean | Full SD | Full %Sample | Dem Mean | Dem SD | Dem %Sample | Rep Mean | Rep SD | Rep %Sample |
|---|---|---|---|---|---|---|---|---|---|
| All | 19.60 | 39.70 | 100 | 21.53 | 41.10 | 100 | 17.90 | 38.34 | 100 |
| Male | 20.11 | 40.08 | 90.20 | 22.31 | 41.63 | 87.02 | 18.29 | 38.66 | 93.01 |
| Female | 14.97 | 35.68 | 9.80 | 16.31 | 36.95 | 12.98 | 12.78 | 33.39 | 6.99 |
| College+ | 20.61 | 40.45 | 83.56 | 22.66 | 41.86 | 85.15 | 18.85 | 39.11 | 82.25 |
| High school– | 15.18 | 35.88 | 16.44 | 16.69 | 37.29 | 14.85 | 14.13 | 34.84 | 17.75 |
| White | 19.12 | 39.33 | 84.81 | 21.38 | 41 | 77.10 | 17.50 | 38 | 91.36 |
| Black | 12.55 | 33.13 | 3.03 | 12.30 | 32.84 | 6.03 | 15.25 | 35.95 | 0.48 |
| Hispanic | 17.10 | 37.65 | 3.33 | 18.71 | 39 | 4.50 | 14.49 | 35.20 | 2.34 |
| Asian | 24.59 | 43.06 | 8.83 | 25.39 | 43.52 | 12.37 | 23.13 | 42.17 | 5.82 |
| Age 18-29 | 17.96 | 38.38 | 3.32 | 17.64 | 38.12 | 4.26 | 18.43 | 38.78 | 2.50 |
| Age 30-39 | 22.68 | 41.88 | 14.63 | 24.20 | 42.83 | 15.29 | 21.22 | 40.89 | 14.04 |
| Age 40-49 | 21.14 | 40.83 | 34.17 | 23.37 | 42.32 | 32.92 | 19.32 | 39.48 | 35.27 |
| Age 50-59 | 19.21 | 39.39 | 31.26 | 21.30 | 40.95 | 31.48 | 17.34 | 37.86 | 31.07 |
| Age 60-70 | 14.79 | 35.50 | 16.61 | 16.70 | 37.29 | 16.05 | 13.22 | 33.87 | 17.11 |
| With a firm | 22.06 | 41.46 | 86.72 | 23.80 | 42.59 | 88.71 | 20.45 | 40.34 | 84.96 |
| Without a firm | 3.58 | 18.57 | 13.28 | 3.71 | 18.91 | 11.29 | 3.49 | 18.35 | 15.04 |
| Voting activeness (all elections) | 19.21 | 39.39 | 41.52 | 21.47 | 41.06 | 42.27 | 17.14 | 37.69 | 40.86 |
| Voting activeness (primaries) | 19.04 | 39.26 | 45.32 | 21.49 | 41.07 | 44.01 | 17.01 | 37.57 | 46.47 |
| Donation activeness | 24.80 | 43.18 | 9.34 | 27.17 | 44.48 | 11.97 | 21.23 | 40.90 | 7.02 |

Sample counts (Panel A): N patenters×year: full 1,528,849; Democrat 715,811; Republican 813,038. N patenters: full 223,685; Democrat 104,729; Republican 118,956. N states: 51 in all three groups.

#### Panel B: 2016 election

| Characteristic | Full Mean | Full SD | Full %Sample | Dem Mean | Dem SD | Dem %Sample | Rep Mean | Rep SD | Rep %Sample |
|---|---|---|---|---|---|---|---|---|---|
| All | 22.13 | 41.51 | 100 | 23.73 | 42.54 | 100 | 20.48 | 40.35 | 100 |
| Male | 22.70 | 41.89 | 88.73 | 24.55 | 43.04 | 85.57 | 20.94 | 40.69 | 91.97 |
| Female | 17.58 | 38.06 | 11.27 | 18.87 | 39.13 | 14.43 | 15.19 | 35.89 | 8.03 |
| College+ | 22.82 | 41.96 | 85.82 | 24.50 | 43.01 | 87.14 | 21.18 | 40.86 | 84.58 |
| High school– | 18.35 | 38.71 | 14.18 | 19.72 | 39.79 | 12.86 | 17.28 | 37.81 | 15.42 |
| White | 21.69 | 41.21 | 81.50 | 23.62 | 42.47 | 73.59 | 20.12 | 40.09 | 89.30 |
| Black | 15.21 | 35.92 | 2.60 | 14.88 | 35.59 | 4.82 | 19.03 | 39.26 | 0.41 |
| Hispanic | 19.93 | 39.95 | 3.93 | 21.20 | 40.87 | 5.23 | 17.48 | 37.98 | 2.65 |
| Asian | 25.50 | 43.59 | 11.97 | 25.92 | 43.82 | 16.36 | 24.63 | 43.09 | 7.64 |
| Age 18-29 | 19.78 | 39.84 | 2.76 | 19.84 | 39.88 | 3.67 | 19.67 | 39.75 | 1.82 |
| Age 30-39 | 25.27 | 43.45 | 12.27 | 26.18 | 43.96 | 14.51 | 23.91 | 42.65 | 9.98 |
| Age 40-49 | 24.04 | 42.73 | 26.69 | 25.34 | 43.50 | 27.20 | 22.65 | 41.85 | 26.16 |
| Age 50-59 | 22.32 | 41.64 | 34.62 | 24.33 | 42.91 | 31.72 | 20.57 | 40.42 | 37.60 |
| Age 60-70 | 18.33 | 38.70 | 23.66 | 20.06 | 40.05 | 22.90 | 16.68 | 37.28 | 24.45 |
| With a firm | 23.84 | 42.61 | 90.16 | 25.22 | 43.43 | 91.96 | 22.38 | 41.68 | 88.31 |
| Without a firm | 6.38 | 24.45 | 9.84 | 6.73 | 25.05 | 8.04 | 6.14 | 24.01 | 11.69 |
| Voting activeness (all elections) | 22.16 | 41.53 | 41.36 | 24.18 | 42.82 | 41.61 | 20.07 | 40.05 | 41.11 |
| Voting activeness (primaries) | 22.02 | 41.44 | 44.13 | 24.08 | 42.76 | 44.88 | 19.84 | 39.88 | 43.37 |
| Donation activeness | 26.36 | 44.06 | 8.87 | 27.94 | 44.87 | 11.17 | 23.59 | 42.45 | 6.53 |

Sample counts (Panel B): N patenters×year: full 1,585,778; Democrat 802,319; Republican 783,459. N patenters: full 234,796; Democrat 118,620; Republican 116,176. N states: 51 in all three groups.

**Note (verbatim):** This table reports sample statistics separately for the 2008 and 2016 elections, spanning 2005-2011 and 2013-2019, respectively. See note to Table 1 for variable definitions.

### Table A2: Election Event Study: Democratic vs. Republican Inventors

- **Dependent variable:** 1(Apply for patent)×100 (indicator for submitting a patent application in a year; units in percentage points)
- **Standard errors:** Clustered by zip code, in parentheses
- **All models include:** Demographics; Zip code FE; Technology Class×Event FE
- **Significance legend (verbatim):** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model_N | election |
|---|---|
| model_1 | 2008 election |
| model_2 | 2016 election |

#### Estimates

| variable | statistic | model_1 | model_2 |
|---|---|---|---|
| Dem×-3 | coefficient | 0.0775 | -0.2929 |
| Dem×-3 | std. error | (0.2087) | (0.2027) |
| Dem×-2 | coefficient | -0.0740 | 0.0674 |
| Dem×-2 | std. error | (0.1946) | (0.2042) |
| Dem×0 | coefficient | -0.0406 | -0.0094 |
| Dem×0 | std. error | (0.1947) | (0.1894) |
| Dem×1 | coefficient | -0.0327 | -0.0349 |
| Dem×1 | std. error | (0.1967) | (0.1931) |
| Dem×2 | coefficient | 0.3470* | -0.4917*** |
| Dem×2 | std. error | (0.1978) | (0.1907) |
| Dem×3 | coefficient | 0.4048** | -0.8493*** |
| Dem×3 | std. error | (0.1979) | (0.1961) |
| Dem | coefficient | 1.5700*** | 1.7377*** |
| Dem | std. error | (0.1900) | (0.1939) |

#### Model statistics

| statistic | model_1 | model_2 |
|---|---|---|
| Observations | 1,528,168 | 1,584,826 |
| R2 | 0.077 | 0.075 |
| Outcome mean | 19.602 | 22.126 |
| N clusters (zip) | 18,561 | 17,663 |

**Note (verbatim):** This table reports the coefficients in Figure 2. The table reports estimates from a DID event-study analysis comparing the likelihood that a Democratic inventor submits a patent application relative to a Republican inventor around the 2008 and 2016 presidential elections. The outcome is an indicator for submitting a patent applicationin a year, and units are in percentage points. *Dem* is one for Democrats and zero for Republicans (see section 2.2 for definition of partisanship). Event time 0 refers to the year of a presidential election. Event time -1 is the omitted period. All regressions control for zip code fixed effects, technology class×event fixed effects, and fully interacted inventor characteristics (i.e., gender, education, age groups, race). Standard errors in parentheses are clustered by zip code. *** 1%, ** 5%, * 10% significance level. [Conversion note: "applicationin" appears in the original.]

### Table A3: 2016 Election DID Analysis: Democratic vs. Republican Inventors — Inventor Partisanship from the 2014 Voter Roll

- **Dependent variable:** 1(Apply for patent)×100
- **Standard errors:** Clustered by zip code, in parentheses
- **All models include:** Demographics
- **Significance legend (verbatim):** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model_N | County FE | Zip FE | Person FE | State×Post FE | Technology Class×Post FE |
|---|---|---|---|---|---|
| model_1 | Y | N | N | Y | N |
| model_2 | N | Y | N | Y | N |
| model_3 | Y | N | N | N | Y |
| model_4 | N | Y | N | N | Y |
| model_5 | Y | N | N | Y | Y |
| model_6 | N | Y | N | Y | Y |
| model_7 | N | N | Y | N | Y |
| model_8 | N | N | Y | Y | Y |

#### Panel A: 2016 election pooled — Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---|---|---|---|---|---|---|---|
| Dem×Post | coefficient | -0.554*** | -0.544*** | -0.382*** | -0.376*** | -0.306** | -0.300** | -0.284* | -0.215 |
| Dem×Post | std. error | (0.144) | (0.144) | (0.145) | (0.145) | (0.146) | (0.146) | (0.145) | (0.147) |
| Dem | coefficient | 1.871*** | 1.687*** | 1.285*** | 1.216*** | 1.249*** | 1.180*** | not applicable | not applicable |
| Dem | std. error | (0.170) | (0.179) | (0.167) | (0.177) | (0.167) | (0.177) | not applicable | not applicable |

#### Panel A: Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---|---|---|---|---|---|---|
| Observations | 1,072,720 | 1,072,733 | 1,072,229 | 1,072,242 | 1,072,229 | 1,072,242 | 1,072,242 | 1,072,242 |
| R2 | 0.033 | 0.065 | 0.050 | 0.081 | 0.050 | 0.081 | 0.499 | 0.499 |
| Outcome mean | 21.28 | 21.28 | 21.28 | 21.28 | 21.28 | 21.28 | 21.28 | 21.28 |
| N clusters (zip) | 16,356 | 16,359 | 16,354 | 16,357 | 16,354 | 16,357 | 16,357 | 16,357 |

#### Panel B: 2016 election by donation — Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---|---|---|---|---|---|---|---|
| Active Dem×Post | coefficient | -2.075*** | -2.106*** | -1.585*** | -1.630*** | -1.502*** | -1.545*** | -1.556*** | -1.488*** |
| Active Dem×Post | std. error | (0.570) | (0.568) | (0.571) | (0.570) | (0.571) | (0.570) | (0.570) | (0.571) |
| Inactive Dem×Post | coefficient | -0.485*** | -0.475*** | -0.325** | -0.319** | -0.252* | -0.245* | -0.233 | -0.166 |
| Inactive Dem×Post | std. error | (0.145) | (0.145) | (0.145) | (0.145) | (0.147) | (0.147) | (0.146) | (0.148) |
| Active Dem | coefficient | 6.744*** | 5.813*** | 5.756*** | 5.095*** | 5.716*** | 5.055*** | not applicable | not applicable |
| Active Dem | std. error | (0.637) | (0.649) | (0.638) | (0.649) | (0.639) | (0.650) | not applicable | not applicable |
| Inactive Dem | coefficient | 1.675*** | 1.530*** | 1.108*** | 1.070*** | 1.073*** | 1.035*** | not applicable | not applicable |
| Inactive Dem | std. error | (0.171) | (0.181) | (0.168) | (0.178) | (0.168) | (0.178) | not applicable | not applicable |

#### Panel B: Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---|---|---|---|---|---|---|
| Observations | 1,072,720 | 1,072,733 | 1,072,229 | 1,072,242 | 1,072,229 | 1,072,242 | 1,072,242 | 1,072,242 |
| R2 | 0.033 | 0.065 | 0.050 | 0.081 | 0.050 | 0.081 | 0.499 | 0.499 |
| Outcome mean | 21.28 | 21.28 | 21.28 | 21.28 | 21.28 | 21.28 | 21.28 | 21.28 |
| N clusters (zip) | 16,356 | 16,359 | 16,354 | 16,357 | 16,354 | 16,357 | 16,357 | 16,357 |

[Conversion note: "not applicable" marks cells empty in the original because level terms are absorbed by person fixed effects in columns 7-8.]

**Note (verbatim):** Panels A and B in this table replicate Table 2 panel B and Table A4 panel B, respectively, but using the 2014 voter roll and patenters' party as of 2014. All specifications mirror those in the corresponding tables. We do not have voting history for the 2014 voter roll, and so cannot replicate Tables 3, 4, and 5. *** 1%, ** 5%, * 10% significance level.

### Table A4: Election DID Analysis: Democratic vs. Republican Inventors by Donation Activeness

- **Dependent variable:** 1(Apply for patent)×100
- **Standard errors:** Clustered by zip code, in parentheses
- **All models include:** Demographics
- **Significance legend (verbatim):** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model_N | Zip FE | Person FE | State×Post FE | Technology Class×Post FE |
|---|---|---|---|---|
| model_1 | Y | N | Y | N |
| model_2 | Y | N | N | Y |
| model_3 | Y | N | Y | Y |
| model_4 | N | Y | N | Y |
| model_5 | N | Y | Y | Y |

#### Panel A: 2008 election — Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---|---|---|---|---|
| Active Dem×Post | coefficient | 0.481 | 0.723** | 0.768** | 0.646** | 0.669** |
| Active Dem×Post | std. error | (0.313) | (0.320) | (0.313) | (0.321) | (0.314) |
| Inactive Dem×Post | coefficient | 0.027 | 0.183 | 0.228* | 0.262* | 0.295** |
| Inactive Dem×Post | std. error | (0.133) | (0.136) | (0.134) | (0.137) | (0.135) |
| Active Dem | coefficient | 5.896*** | 4.889*** | 4.866*** | not applicable | not applicable |
| Active Dem | std. error | (0.343) | (0.340) | (0.339) | not applicable | not applicable |
| Inactive Dem | coefficient | 1.881*** | 1.192*** | 1.169*** | not applicable | not applicable |
| Inactive Dem | std. error | (0.158) | (0.155) | (0.156) | not applicable | not applicable |

#### Panel A: Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---|---|---|---|
| Observations | 1,309,566 | 1,309,242 | 1,309,242 | 1,309,242 | 1,309,242 |
| R2 | 0.063 | 0.078 | 0.078 | 0.484 | 0.485 |
| Outcome mean | 19.69 | 19.69 | 19.69 | 19.69 | 19.69 |
| N clusters (zip) | 18,562 | 18,561 | 18,561 | 18,561 | 18,561 |

#### Panel B: 2016 election — Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---|---|---|---|---|
| Active Dem×Post | coefficient | -1.601*** | -1.222*** | -1.108*** | -1.391*** | -1.308*** |
| Active Dem×Post | std. error | (0.295) | (0.295) | (0.296) | (0.294) | (0.296) |
| Inactive Dem×Post | coefficient | -0.390*** | -0.260** | -0.134 | -0.106 | 0.000 |
| Inactive Dem×Post | std. error | (0.132) | (0.129) | (0.133) | (0.130) | (0.134) |
| Active Dem | coefficient | 5.432*** | 4.965*** | 4.910*** | not applicable | not applicable |
| Active Dem | std. error | (0.352) | (0.352) | (0.352) | not applicable | not applicable |
| Inactive Dem | coefficient | 1.764*** | 1.306*** | 1.245*** | not applicable | not applicable |
| Inactive Dem | std. error | (0.163) | (0.160) | (0.161) | not applicable | not applicable |

#### Panel B: Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---|---|---|---|
| Observations | 1,358,125 | 1,357,474 | 1,357,474 | 1,357,474 | 1,357,474 |
| R2 | 0.059 | 0.075 | 0.075 | 0.501 | 0.501 |
| Outcome mean | 22.12 | 22.12 | 22.12 | 22.12 | 22.12 |
| N clusters (zip) | 17,665 | 17,663 | 17,663 | 17,663 | 17,663 |

[Conversion note: "not applicable" marks cells empty in the original because level terms are absorbed by person fixed effects in columns 4-5.]

**Note (verbatim):** This is a variant of Table 3 columns 1-5 where political activeness is measured using FEC donation data. *** 1%, ** 5%, * 10% significance level.

### Table A5: Election DID Analysis within Firm and Technology by Voting Activeness — USPC Technology Classifications

- **Dependent variable:** 1(Apply for patent)×100
- **Standard errors:** In parentheses
- **All models include:** Demographics; Zip FE
- **Column groups:** Columns 1-4 use voting activeness in general & primary elections; columns 5-6 use voting activeness in primary elections
- **Significance legend (verbatim):** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model_N | activeness measure | Technology Class×Post FE | Firm×Post FE | Firm×Technology Class×Post FE | FEs estimated with expanded sample |
|---|---|---|---|---|---|
| model_1 | general & primary | Y | Y | N | N |
| model_2 | general & primary | N | N | Y | N |
| model_3 | general & primary | Y | Y | N | Y |
| model_4 | general & primary | N | N | Y | Y |
| model_5 | primary | Y | Y | N | Y |
| model_6 | primary | N | N | Y | Y |

#### Panel A: 2008 election — Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|---|
| Active Dem×Post | coefficient | 0.556*** | 0.584** | 0.584*** | 0.603*** | 0.531*** | 0.565*** |
| Active Dem×Post | std. error | (0.211) | (0.235) | (0.199) | (0.210) | (0.200) | (0.212) |
| Inactive Dem×Post | coefficient | 0.065 | 0.095 | 0.073 | 0.084 | 0.041 | 0.059 |
| Inactive Dem×Post | std. error | (0.205) | (0.230) | (0.193) | (0.204) | (0.202) | (0.213) |
| Active Dem | coefficient | 1.208*** | 1.360*** | 1.280*** | 1.384*** | 1.313*** | 1.417*** |
| Active Dem | std. error | (0.236) | (0.267) | (0.240) | (0.250) | (0.244) | (0.255) |
| Inactive Dem | coefficient | 1.664*** | 1.519*** | 1.804*** | 1.742*** | 1.830*** | 1.767*** |
| Inactive Dem | std. error | (0.226) | (0.260) | (0.242) | (0.274) | (0.250) | (0.284) |

#### Panel A: Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|
| Observations | 998,394 | 998,394 | 2,322,060 | 2,322,060 | 2,295,872 | 2,295,872 |
| R2 | 0.205 | 0.302 | 0.234 | 0.301 | 0.235 | 0.302 |
| Outcome mean | 21.78 | 21.78 | 21.78 | 21.78 | 21.74 | 21.74 |

#### Panel B: 2016 election — Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|---|
| Active Dem×Post | coefficient | -0.381* | -0.386* | -0.633*** | -0.606** | -0.803*** | -0.730*** |
| Active Dem×Post | std. error | (0.206) | (0.233) | (0.245) | (0.256) | (0.247) | (0.261) |
| Inactive Dem×Post | coefficient | -0.264 | -0.068 | -0.525** | -0.468* | -0.416* | -0.387 |
| Inactive Dem×Post | std. error | (0.188) | (0.209) | (0.224) | (0.248) | (0.225) | (0.247) |
| Active Dem | coefficient | 1.734*** | 1.804*** | 1.899*** | 1.910*** | 1.893*** | 1.863*** |
| Active Dem | std. error | (0.257) | (0.280) | (0.282) | (0.282) | (0.276) | (0.277) |
| Inactive Dem | coefficient | 1.288*** | 1.070*** | 1.580*** | 1.507*** | 1.567*** | 1.503*** |
| Inactive Dem | std. error | (0.235) | (0.260) | (0.276) | (0.287) | (0.280) | (0.289) |

#### Panel B: Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|
| Observations | 1,035,742 | 1,035,742 | 2,669,505 | 2,669,505 | 2,653,413 | 2,653,413 |
| R2 | 0.221 | 0.314 | 0.260 | 0.320 | 0.260 | 0.321 |
| Outcome mean | 24.31 | 24.31 | 24.31 | 24.31 | 24.26 | 24.26 |

**Note (verbatim):** This table replicates Table 4 but uses the USPC instead of the CPC technology classification scheme. There are 420 USPC technology classes and around 138,000 subclasses in our sample, so we only use Firm × USPC Technology Class × Post because its granularity is similar to Firm × CPC subclass (625 subclasses) × Post. We define a patenter's technology class as their modal USPC class among eventually granted patents submitted in the pre pre-period. Some patents applied for in the pre pre-period do not have a USPC classification because they were granted after the change to CPC, leading to smaller sample sizes compared to Table 4. Everything else follows Table 4. *** 1%, ** 5%, * 10% significance level.

### Table A6: Election DID Analysis within Firm and Technology Class — Controlling for Team Characteristics

- **Dependent variable:** 1(Apply for patent)×100
- **Standard errors:** Clustered by zip code, in parentheses
- **All models include:** Demographics; Zip FE; Firm×Technology Class×Post FE; Team size controls; Team size controls×Post
- **Significance legend (verbatim):** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model_N | election | Team partisan controls (and ×Post) | Team demographic controls (and ×Post) |
|---|---|---|---|
| model_1 | 2008 | N | N |
| model_2 | 2008 | Y | N |
| model_3 | 2008 | Y | Y |
| model_4 | 2016 | N | N |
| model_5 | 2016 | Y | N |
| model_6 | 2016 | Y | Y |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|---|
| Active Dem×Post | coefficient | 0.597** | 0.640*** | 0.631** | -0.614*** | -0.695*** | -0.686*** |
| Active Dem×Post | std. error | (0.246) | (0.247) | (0.247) | (0.227) | (0.227) | (0.227) |
| Inactive Dem×Post | coefficient | 0.178 | 0.276 | 0.257 | -0.203 | -0.209 | -0.228 |
| Inactive Dem×Post | std. error | (0.238) | (0.239) | (0.239) | (0.212) | (0.211) | (0.211) |
| Active Rep×Post | coefficient | 0.229 | 0.245 | 0.245 | -0.322 | -0.352 | -0.338 |
| Active Rep×Post | std. error | (0.231) | (0.233) | (0.232) | (0.228) | (0.228) | (0.228) |
| Active Dem | coefficient | 1.232*** | 1.054*** | 1.006*** | 2.213*** | 2.536*** | 2.456*** |
| Active Dem | std. error | (0.284) | (0.282) | (0.281) | (0.282) | (0.286) | (0.281) |
| Inactive Dem | coefficient | 1.695*** | 1.366*** | 1.354*** | 1.415*** | 1.624*** | 1.590*** |
| Inactive Dem | std. error | (0.266) | (0.265) | (0.264) | (0.260) | (0.257) | (0.254) |
| Active Rep | coefficient | -0.065 | -0.247 | -0.263 | 0.921*** | 0.849*** | 0.856*** |
| Active Rep | std. error | (0.264) | (0.263) | (0.261) | (0.273) | (0.270) | (0.267) |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|
| Observations | 1,002,941 | 1,002,941 | 1,002,941 | 1,155,176 | 1,155,176 | 1,155,176 |
| R2 | 0.259 | 0.271 | 0.274 | 0.259 | 0.273 | 0.277 |
| Outcome mean | 21.62 | 21.62 | 21.62 | 23.78 | 23.78 | 23.78 |
| N clusters (zip) | 16,181 | 16,181 | 16,181 | 16,190 | 16,190 | 16,190 |

**Note (verbatim):** This table adds team-level controls to the specification in Table 5 column 2 (which includes Firm×Technology Class×Post fixed effects). Teams are defined by each (eventually granted) patent application submitted in years t-10 through t-4 before an election (i.e., the pre pre-period of each election). Team characteristics (e.g., team size) are calculated for each team the focal patenter participates in during this period (leaving out the focal patenter) and are averaged across their teams. Each team characteristic is also interacted with the *Post* indicator. Columns 1 and 4 add team size controls: the average number of teammates and fraction of teammates matched to the political affiliation data per patent application. Columns 2 and 5 add team partisan controls: the average share of teammates that are independent, the average share that are politically active Democrats or Republicans (based on voting history), and an indicator for ever working on a team with members of the opposite party. Columns 3 and 6 add team demographic controls: the average age of teammates, the share that have a college degree or higher, and the shares of immigrants, men, Asian, African American, or Hispanic patenters. Everything else follows Table 5 column 2. Standard errors are clustered by zip code. *** 1%, ** 5%, * 10% significance level.

### Table A7: Election DID Analysis within Firm and Technology Subclass — Controlling for Team Characteristics

- **Dependent variable:** 1(Apply for patent)×100
- **Standard errors:** Clustered by zip code, in parentheses
- **All models include:** Demographics; Zip FE; Firm×Technology Subclass×Post FE; Team size controls; Team size controls×Post
- **Significance legend (verbatim):** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model_N | election | Team partisan controls (and ×Post) | Team demographic controls (and ×Post) |
|---|---|---|---|
| model_1 | 2008 | N | N |
| model_2 | 2008 | Y | N |
| model_3 | 2008 | Y | Y |
| model_4 | 2016 | N | N |
| model_5 | 2016 | Y | N |
| model_6 | 2016 | Y | Y |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|---|
| Active Dem×Post | coefficient | 0.486* | 0.499* | 0.484* | -0.528** | -0.636*** | -0.633*** |
| Active Dem×Post | std. error | (0.255) | (0.257) | (0.257) | (0.237) | (0.238) | (0.238) |
| Inactive Dem×Post | coefficient | 0.030 | 0.101 | 0.073 | -0.140 | -0.157 | -0.177 |
| Inactive Dem×Post | std. error | (0.247) | (0.247) | (0.248) | (0.221) | (0.220) | (0.219) |
| Active Rep×Post | coefficient | 0.163 | 0.162 | 0.167 | -0.317 | -0.369 | -0.350 |
| Active Rep×Post | std. error | (0.241) | (0.244) | (0.244) | (0.235) | (0.237) | (0.237) |
| Active Dem | coefficient | 1.347*** | 1.220*** | 1.178*** | 2.116*** | 2.514*** | 2.447*** |
| Active Dem | std. error | (0.297) | (0.295) | (0.294) | (0.291) | (0.297) | (0.292) |
| Inactive Dem | coefficient | 1.749*** | 1.488*** | 1.496*** | 1.354*** | 1.595*** | 1.565*** |
| Inactive Dem | std. error | (0.273) | (0.272) | (0.272) | (0.270) | (0.267) | (0.263) |
| Active Rep | coefficient | 0.052 | -0.108 | -0.131 | 0.970*** | 0.946*** | 0.937*** |
| Active Rep | std. error | (0.273) | (0.273) | (0.272) | (0.283) | (0.281) | (0.278) |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|
| Observations | 1,002,953 | 1,002,953 | 1,002,953 | 1,155,076 | 1,155,076 | 1,155,076 |
| R2 | 0.292 | 0.303 | 0.306 | 0.291 | 0.304 | 0.308 |
| Outcome mean | 21.62 | 21.62 | 21.62 | 23.78 | 23.78 | 23.78 |
| N clusters (zip) | 16,182 | 16,182 | 16,182 | 16,189 | 16,189 | 16,189 |

**Note (verbatim):** This table adds team-level controls to the specification in Table 5 column 3 (which includes Firm×Technology Subclass×Post fixed effects). All team controls are defined as in Table A6. Everything else follows Table 5 column 3. Standard errors are clustered by zip code. *** 1%, ** 5%, * 10% significance level.

### Table A8: Election DID Analysis within Firm and Technology — Excluding States with Modeled Party Affiliation

- **Dependent variable:** 1(Apply for patent)×100
- **Standard errors:** Clustered by zip code, in parentheses
- **All models include:** Demographics; Zip FE
- **Column groups:** Columns 1-3 drop pure modeling states; columns 4-6 drop states with any modeling
- **Significance legend (verbatim):** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model_N | sample restriction | Technology Class×Post FE | Firm×Post FE | Firm×Technology Class×Post FE | Firm×Technology Subclass×Post FE |
|---|---|---|---|---|---|
| model_1 | drop pure modeling states | Y | Y | N | N |
| model_2 | drop pure modeling states | N | N | Y | N |
| model_3 | drop pure modeling states | N | N | N | Y |
| model_4 | drop states with any modeling | Y | Y | N | N |
| model_5 | drop states with any modeling | N | N | Y | N |
| model_6 | drop states with any modeling | N | N | N | Y |

#### Panel A: 2008 election — Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|---|
| Active Dem×Post | coefficient | 0.654*** | 0.673*** | 0.582** | 0.714*** | 0.733*** | 0.673** |
| Active Dem×Post | std. error | (0.240) | (0.255) | (0.265) | (0.258) | (0.275) | (0.287) |
| Inactive Dem×Post | coefficient | 0.141 | 0.198 | 0.070 | 0.253 | 0.300 | 0.171 |
| Inactive Dem×Post | std. error | (0.232) | (0.247) | (0.256) | (0.248) | (0.263) | (0.273) |
| Active Rep×Post | coefficient | 0.154 | 0.259 | 0.166 | 0.088 | 0.226 | 0.210 |
| Active Rep×Post | std. error | (0.226) | (0.241) | (0.252) | (0.242) | (0.260) | (0.272) |
| Active Dem | coefficient | 1.184*** | 1.146*** | 1.207*** | 1.452*** | 1.433*** | 1.493*** |
| Active Dem | std. error | (0.274) | (0.293) | (0.305) | (0.294) | (0.317) | (0.334) |
| Inactive Dem | coefficient | 1.707*** | 1.712*** | 1.737*** | 1.643*** | 1.689*** | 1.696*** |
| Inactive Dem | std. error | (0.255) | (0.275) | (0.283) | (0.274) | (0.296) | (0.306) |
| Active Rep | coefficient | -0.144 | -0.185 | -0.011 | 0.005 | -0.054 | 0.112 |
| Active Rep | std. error | (0.257) | (0.279) | (0.290) | (0.274) | (0.299) | (0.312) |

#### Panel A: Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|
| Observations | 935,416 | 935,416 | 935,428 | 824,275 | 824,275 | 824,281 |
| R2 | 0.201 | 0.261 | 0.295 | 0.209 | 0.271 | 0.306 |
| Outcome mean | 21.5 | 21.5 | 21.5 | 21.51 | 21.51 | 21.52 |
| N clusters (zip) | 14,937 | 14,937 | 14,938 | 13,861 | 13,861 | 13,862 |

#### Panel B: 2016 election — Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|---|
| Active Dem×Post | coefficient | -0.464** | -0.553** | -0.503** | -0.446* | -0.508* | -0.449* |
| Active Dem×Post | std. error | (0.223) | (0.237) | (0.247) | (0.242) | (0.261) | (0.271) |
| Inactive Dem×Post | coefficient | -0.302 | -0.196 | -0.162 | -0.336 | -0.215 | -0.186 |
| Inactive Dem×Post | std. error | (0.209) | (0.220) | (0.229) | (0.226) | (0.238) | (0.250) |
| Active Rep×Post | coefficient | -0.307 | -0.336 | -0.313 | -0.371 | -0.404 | -0.335 |
| Active Rep×Post | std. error | (0.224) | (0.237) | (0.245) | (0.237) | (0.253) | (0.262) |
| Active Dem | coefficient | 2.051*** | 2.185*** | 2.123*** | 2.155*** | 2.349*** | 2.295*** |
| Active Dem | std. error | (0.272) | (0.292) | (0.302) | (0.297) | (0.320) | (0.331) |
| Inactive Dem | coefficient | 1.409*** | 1.341*** | 1.299*** | 1.516*** | 1.448*** | 1.386*** |
| Inactive Dem | std. error | (0.253) | (0.270) | (0.281) | (0.271) | (0.288) | (0.301) |
| Active Rep | coefficient | 0.715*** | 0.859*** | 0.933*** | 0.882*** | 1.043*** | 1.103*** |
| Active Rep | std. error | (0.270) | (0.287) | (0.299) | (0.287) | (0.305) | (0.321) |

#### Panel B: Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|
| Observations | 1,079,854 | 1,079,854 | 1,079,766 | 934,245 | 934,245 | 934,141 |
| R2 | 0.206 | 0.261 | 0.294 | 0.218 | 0.275 | 0.308 |
| Outcome mean | 23.74 | 23.74 | 23.74 | 23.85 | 23.85 | 23.84 |
| N clusters (zip) | 14,900 | 14,900 | 14,899 | 13,809 | 13,809 | 13,808 |

**Note (verbatim):** This table reports robustness tests for Table 5 columns 1-3 by excluding states that model voter party affiliation using only demographic and geographic information ("pure modeling") in the first three columns, or states that either use a mix of pure modeling and primary voting behavior ("any modeling") in the next three columns. Thus, columns 4-6 leave in the sample only patenters with self-identified partisanship. Everything else follows Table 5 columns 1-3. Standard errors in parentheses are clustered by zip code. *** 1%, ** 5%, * 10% significance level.

### Table A9: Political Mismatch and the Number of Granted Patents: Democratic versus Republican Technologies

- **Standard errors:** Clustered by subclass, in parentheses
- **All models include:** Subclass FE; Technology Class×Post FE
- **Significance legend (verbatim):** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model_N | technology split | outcome |
|---|---|---|
| model_1 | Median split | Grant |
| model_2 | Median split | Std. grant |
| model_3 | Top vs. bottom tercile | Grant |
| model_4 | Top vs. bottom tercile | Std. grant |
| model_5 | Top vs. bottom quartile | Grant |
| model_6 | Top vs. bottom quartile | Std. grant |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|---|
| Dem×Post | coefficient | 41.891*** | 0.974*** | 42.071*** | 0.926** | 48.084* | 0.796** |
| Dem×Post | std. error | (13.479) | (0.360) | (15.682) | (0.442) | (25.159) | (0.364) |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---|---|---|---|---|
| Observations | 5,040 | 5,040 | 3,950 | 3,950 | 2,900 | 2,900 |
| R2 | 0.959 | 0.556 | 0.958 | 0.553 | 0.956 | 0.575 |
| Outcome mean | 223.76 | .344 | 235.79 | .412 | 247.4 | .38 |
| N clusters (subclass) | 504 | 504 | 395 | 395 | 290 | 290 |

**Note (verbatim):** This table shows the robustness of the main result in Figure 7 panels (a) and (b) using differing definitions of Democratic and Republican technology subclasses. The table compares the number of granted patents in Democratic vs. Republican technology subclasses submitted in the years around the 2008 presidential election. Democratic technology subclasses are those whose share of Democrats among all inventors actively patenting in the pre-pre-period (i.e., years 10 through 4 before the 2008 election) exceeds a certain threshold: columns (1)-(2) use sample median, (3)-(4) the 66th percentile, and (5)-(6) the 75th percentile. Only subclasses with at least eight actively patenting patenters before the election are assigned a partisan leaning. The outcome in columns (1), (3), and (5) is the number of eventually granted patents submitted in each subclass each year; the outcome in columns (2), (4), and (6) is the number subtracting the pre-election subclass mean and then dividing by the standard deviation. All regressions control for subclass fixed effects and Technology Class×Post fixed effects. Standard errors in parentheses are clustered by subclass. *** 1%, ** 5%, * 10% significance level.
