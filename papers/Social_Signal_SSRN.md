---
title: "The Social Signal"
authors: ["J. Anthony Cookson", "Runjing Lu", "William Mullins", "Marina Niessner"]
date: "December 15, 2023"
status: "Published"
journal: "Journal of Financial Economics"
doi: "10.1016/j.jfineco.2024.103870"
url: "https://doi.org/10.1016/j.jfineco.2024.103870"
jel: ["G14", "G41", "G12"]
keywords: ["Social media", "Retail trading", "Social finance"]
conversion: "Text-only Markdown for LLM reading, converted from the SSRN working-paper version (December 15, 2023), which may differ from the published article. Images omitted. Tables converted to semantic Markdown."
mode: "publication"
---

# The Social Signal

## Converter's summary

*This summary was written by the converter, not the authors.* The paper asks whether the market-relevant information in investor social media — decomposed into attention and sentiment — is common across platforms or platform-specific. Using firm-day data from 2012-2021 on StockTwits, Twitter, and Seeking Alpha (roughly 815,000 firm-day observations covering the 1,500 most-discussed firms on StockTwits), the authors run principal component analyses on the six signals. Attention has a strong common component (PC1 explains 67% of variation; Table 2, Panel C) while sentiment's common component is weak (PC1 explains 38.8%, barely above the 33.3% idiosyncratic benchmark), and these patterns survive residualizing on news, firm fixed effects, and lagged returns (Table 3). The two signals also predict returns with opposite signs: a one-standard-deviation increase in the sentiment PC1 predicts a 6.1 bps higher next-day abnormal return, while the attention PC1 predicts -13.1 bps (Table 6, column 1), with attention's negative predictability reflecting partial reversal of same-day overreaction (Table 7, Figure 3). Two events identify mechanisms: after StockTwits raised its character limit from 140 to 1,000 in May 2019, StockTwits sentiment became more informative (+7 bps; Table 8, column 1), driven by professionals writing longer messages; and after the January 2021 GameStop short squeeze, sentiment informativeness deteriorated (-12.5 bps; Table 9, column 1), concentrated among new users. The paper concludes that attention-based results in the social finance literature are more likely to generalize across platforms than sentiment-based results.

## Abstract

We examine social media attention and sentiment from three major platforms: Twitter, StockTwits, and Seeking Alpha. We find that, even after controlling for firm disclosures and news, attention is highly correlated across platforms, but sentiment is not: its first principal component explains little more variation than purely idiosyncratic sentiment. Using market events, we attribute differences across platforms to differences in users (e.g., professionals vs. novices) and differences in platform design (e.g., character limits in posts). We also find that sentiment and attention contain different return-relevant information. Sentiment predicts positive next-day returns, but attention predicts negative next-day returns. These results highlight the importance of distinguishing between social media sentiment and attention across different investor social media platforms. In the burgeoning social finance literature, nearly all papers examine single platforms; our paper cautions that attention-related results from these papers are more likely to generalize than results concerning sentiment.

**Keywords:** Social media, Retail trading, Social finance

**JEL Codes:** G14, G41, G12

**Authors and affiliations:** J. Anthony Cookson: University of Colorado at Boulder (tony.cookson@colorado.edu); Runjing Lu: University of Alberta (runjing1@ualberta.ca); William Mullins: UC San Diego (wmullins@ucsd.edu); Marina Niessner: Indiana University (mniessne@iu.edu).

**Acknowledgments:** This draft has benefited from comments by Zhi Da, Yao Deng, Joey Engelberg, Lukasz Pomorski, Brian Waters, and Isabella Wolfskeil as well as from presentations at University of Colorado at Boulder, University of Texas-El Paso, University of Toronto, Washington University of St. Louis, University of Notre Dame, George Washington University, University of Florida, University of Miami, Arizona State University, University of Washington, Iowa State University, University of Iowa, National University of Singapore, Singapore Management University, Nanyang Technical University, 5th Future of Financial Information Conference, 7th Annual News and Finance Conference at Columbia, 8th Annual Conference on Network Science and Economics, 18th Annual Conference in Financial Economics Research by Eagle Labs, FMA, the Michigan State FCU Conference, the USC Conference on Behavioral and Social Economics, MFA, UChicago Empirical Finance Conference, Future of Financial Information Conference, Kepos Capital, Citigroup Global Insights, and USC Finance.

## 1. Introduction

Social media has grown exponentially over the past two decades. Americans spent 3.6 hours per day on some form of social media in 2020 (Forbes, 2021), and increasingly view social media as a primary source of news (Pew, 2021). Financial markets also reflect this: investors frequently post opinions about securities on social media, and firms use it to disclose information and interact with investors (Blankespoor et al., 2014). Despite these trends, investor social media was largely seen as a sideshow until recent social media-fueled trading frenzies, most prominently the 2021 GameStop phenomenon. These events raise questions about the role social platforms play for trading and information in financial markets (Pedersen, 2022), and an emerging line of research has organized around these important questions.

Prior analyses of investor social media have almost exclusively examined data from a single platform, and related papers often draw upon evidence from different investor social networks, typically StockTwits, Seeking Alpha, and Twitter.[^1] While most of this work considers questions that are not specific to the particular investor social platform studied, these platforms differ in myriad ways.[^2] Communication theory implies that social media platforms may not be interchangeable because the characteristics of a communication medium affect both the content and impact of messages (e.g., McLuhan, 1975). Because communication is a socially emergent phenomenon, differences in user populations, incentives to post, and ability to engage may lead each platform to have unique informational content.

[^1]: For example, for StockTwits see Giannini et al. (2019), Cookson et al. (2022a,b), Irvine et al. (2021); for Twitter, Gu and Kurov (2020), Chen et al. (2019), Cookson et al. (2023), Bianchi et al. (2023, 2024); for Seeking Alpha, Chen et al. (2014), Dim (2020), Chen and Hwang (2022), Farrell et al. (2022), Kogan et al. (2022).

[^2]: For example, Seeking Alpha articles are long-form and lightly moderated; Twitter posts are limited to 280 characters, but multiple posts can be threaded together for longer arguments; while StockTwits posts cannot be threaded, they have had a 1,000 character limit since 2019. These platforms also differ in their user bases, recommendation algorithms, how individuals interact through messages and tagging, and many other characteristics. Figure 1 presents an example post for each platform in our study.

To examine whether and how these platforms generate differing market-relevant information – the social media signal – this paper examines a decade of comprehensive firm-day-level data (2012-2021) from the three most established investor social networks: StockTwits, Twitter, and Seeking Alpha. We first distinguish between two features common to all social networks: attention and sentiment. We find that over two-thirds of the firm-day attention signal is common across the major social platforms: on a given day, people on different platforms tend to talk about the same firms. By contrast, the common component of sentiment is weak, explaining only slightly more than it would if sentiment across the three platforms were idiosyncratic.

In addition, we show that the common components of social sentiment and attention have opposing return predictions: attention generally predicts negative next day returns, while sentiment predicts positive returns. Exploiting two events – a change in the message character limit on StockTwits and the GameStop (GME) short squeeze – we find that differences in platform features (the character-limit event) and differences across user populations (the GME event) each contribute to differences in the market-relevant information generated by investor social media.

We now describe our findings in greater detail. We begin by decomposing the social signal generated by all three platforms using principal component analysis (PCA) separately for attention and sentiment. We find that attention has a powerful common component, with the first principal component (PC1) explaining 67% of the variation. Conversely, the PC1 of sentiment explains 39% of the variation in sentiment, only slightly more than the 33% it would explain if the three signals were idiosyncratic. We show that these findings are not driven by news, firm disclosures, stock returns, or persistent firm components by first regressing attention and sentiment from each platform on these variables and firm fixed effects, and then performing a PCA on the residualized signals. This conditional PCA analysis yields very similar patterns to the unconditional PCA we started with, indicating that the common signal in investor social media is distinct from the information in traditional media.[^3]

[^3]: We will make the PC1s of sentiment and attention available to researchers on our websites upon publication.

An alternative explanation for the weak cross-platform correlation in sentiment is that the signals from each platform are extracted using different natural language processing algorithms (NLPs). We provide evidence that NLPs cannot explain these differences by comparing different user types within StockTwits, thus holding constant both platform features and NLP. Consistent with our cross-platform results, we find that attention is highly correlated across user types such as influencers, professionals, and novices (i.e., the PC1 explains 84% of the variation), whereas sentiment signals have a weak correlation across user types. Thus, differences in NLPs cannot fully drive our results. Moreover, this evidence suggests that, even if NLPs and all platform features were identical, we would see cross-platform differences in the sentiment signal because of differences in user populations.

The most salient difference across social investor platforms is in the size of the firms they cover. StockTwits focuses more on small-cap firms, whereas Twitter and Seeking Alpha pay greater attention to large-cap firms. When we repeat our conditional PCA separately by firm size bins, we find that attention displays more commonality than sentiment irrespective of firm size. However, large-cap firms display stronger commonality in attention and sentiment than small cap firms. This size-based heterogeneity for sentiment suggests that whether a sentiment-related result in the social finance literature generalizes across platforms may depend on how important small firms are in driving that result.

Next, we explore whether the informativeness of sentiment and attention signals differs across platforms. To capture informativeness, we regress next-day abnormal returns on sentiment and attention signals from the three platforms, controlling for news from traditional media, firm announcements, lagged returns and volatility, and Google search volume (Da et al., 2011). The signal from any given platform is a combination of a common component, captured by PC1s of sentiment and attention, and a platform-specific idiosyncratic component. We find that the common component of sentiment predicts positive next day abnormal returns and that the common component of attention predicts negative next day returns. Looking at signals from each platform separately, we find that informativeness of signals varies substantially across platforms.[^4] Overall, StockTwits' signal is better aligned with the common components than Twitter and Seeking Alpha (especially for attention), with respect to next-day returns.[^5]

[^4]: When we examine the signals from Reddit WallStreetBets (WSB) starting in 2018, we find no link between sentiment and next day returns and a positive loading on attention. We also show that the inclusion of WSB signals in the conditional PCA does not change our findings.

[^5]: Because these platforms focus on different-sized firms, we examine heterogeneity in informativeness by firm size. The informativeness of sentiment does not appear to differ by firm size, either across or within platforms. However, StockTwits attention is more informative for small and mid-size firms than it is for large firms.

To shed light on the mechanisms behind the informativeness of the social signal, we explore how it relates to same-day returns and to returns out to 20 days. We find that more positive sentiment is associated with higher same-day and day $t+1$ returns, with no reversal in the subsequent 20 days. By contrast, higher attention is associated with higher same-day returns, followed by a partial reversal over the next 10 to 20 days. Digging deeper, we show that net retail buying is positively related to same-day sentiment and attention, but this positive relation only lasts for one to two days. These results help explain our findings on the informativeness of social signal for next-day returns: the positive predictability of sentiment is likely because it contains return-relevant information, while the negative predictability of attention is most consistent with a partial and gradual reversal of an over-reaction on high-attention days.

We next examine two events which provide insight into whether platform-specific features and user groups contribute to the differences in the informativeness of sentiment and attention. First, we examine changes in the informativeness of the social signal around May 8, 2019, when StockTwits increased its character limit per message from 140 to 1,000 characters. We find that StockTwits sentiment became more predictive of next-day stock returns after this change. Moreover, this effect is driven by sentiment when messages are longer; the informativeness of shorter messages and attention were unchanged. We find that professionals' messages are more informative on average, and that after the character limit increase they write longer messages, suggesting a possible mechanism. Consistent with the fact that Twitter and Seeking Alpha were unaffected by StockTwits' character limit increase, we find no change in the informativeness of signals from these platforms. These results indicate that a within-platform change to users' ability to communicate can affect the market-relevant information encoded in the social media signal, in line with communication theory. These findings also suggest that structural differences across investor social media platforms contribute to the differences we find in the signal they generate.

Second, we examine how the informativeness of sentiment and attention changed around the January 2021 GME phenomenon. In 2020, the number of U.S. retail brokerage accounts increased rapidly and StockTwits saw an influx of new users, both likely a result of COVID stay-at-home orders coupled with the introduction of no-fee trading at many brokerages. Bradley et al. (2021) shows that Reddit retail trading based on WSB "due diligence" reports became less informative in the wake of the GME short squeeze. We show that the informativeness of sentiment across all platforms deteriorated significantly after the GME short squeeze: returns became less sensitive to sentiment. Moreover, the drop in informativeness is concentrated among messages by new users, as the informativeness of the signal extracted from more established users (who joined before 2020) did not change after January 2021. These findings emphasize the importance of changing user populations and new narratives in shaping the information content of the social signal.

**Related literature.** Our paper makes several contributions to the literature on retail investors, sentiment, attention, and the informativeness of novel data sources in financial markets. Our core contribution is to quantify the information content, similarities and differences across the three most-established investor social media platforms over the last decade. With the rising significance of social media platforms as a forum for communicating investor beliefs, a literature has emerged to study their information content. Investors discuss financial ideas on myriad online forums, but analyses typically focus on a single platform and employ different data (e.g., Chen et al., 2014, Cookson and Niessner, 2020, Gu and Kurov, 2020, Irvine et al., 2021).[^6] Divergent findings may stem from examining different parts of the investor social media space. In this paper, we show that this concern is particularly important for sentiment, while cross-platform differences are somewhat less important for attention. More generally, we illustrate how features of different social media platforms (e.g., character limits and different user-bases) matter for the informativeness of the social signal.

[^6]: Recent work on earnings forecasts from Estimize has examined similar questions about information transmission and social influence – e.g., Da and Huang (2020) and Jame et al. (2016) study aspects of the wisdom of crowds, and Da et al. (2021) shows how Estimize analysts extrapolate their beliefs from past experience.

We also contribute to the social economics literature (Akçay and Hirshleifer, 2021, Hirshleifer, 2020, Kuchler and Stroebel, 2021), and especially research on the economics of social media (Pedersen, 2022). Connections on social media have been shown to shape political disagreements, amplify anti-minority sentiment, and even influence house price expectations (Bailey et al., 2018a, Levy, 2021, Lu and Sheng, 2022). In this broader literature, some have used connections on a single social media platform as a proxy for social connections in general (e.g., Bailey et al., 2018b, Hirshleifer et al., 2023), while other research presents evidence that a specific platform has economic impacts (e.g., Müller and Schwarz, 2022). The market events we examine provide some support to both approaches. Our findings around the message limit change to StockTwits support the view that social media is not interchangeable, as platform-specific features significantly impact the information each platform generates. However, the evidence from the GME event also illustrates how events on one platform spill over onto others, showing strong common effects of a sufficiently large change in the social media space.

Our results also contribute to the literature on retail attention and sentiment (e.g., Da et al., 2011, Sicherman et al., 2016, Gargano and Rossi, 2018). Existing work with investor social media either focuses on aspects of investor attention (e.g., Giannini et al., 2018, Cookson et al., 2022a, Irvine et al., 2021) or on sentiment and optimism (e.g., Antweiler and Frank, 2004, Renault, 2017, Cookson et al., 2020). Outside of social media, research on sentiment (e.g., Tetlock, 2007, Garcia, 2013) and attention (e.g., Barber and Odean, 2008, Da et al., 2011) has also typically focused on only one of the two. As a result, a seemingly conflicting body of evidence has emerged in which sentiment is typically informative of future returns, but retail attention appears strongly misinformed. The literature has partly resolved this tension by showing that different kinds of attention have different return implications (Ben-Rephael et al., 2017, Da et al., 2022, Barber et al., 2022). By examining sentiment and attention together across multiple platforms, we show that there is a striking difference in the informativeness of sentiment vs. attention.

We also contribute to the literature on the role of new entrants to financial markets and their implications for markets (e.g., Bradley et al., 2021). In early work, Chen et al. (2014) shows that Seeking Alpha recommendations are informative. With the advent of new firm-day retail trading measures (Boehmer et al., 2021), the literature has examined how retail trading relates to social media activity, with a primary focus on Seeking Alpha (e.g., Farrell et al., 2022). This research has also shown that retail investor activity has important implications for market quality, particularly driven by new retail traders on Robinhood (e.g., Eaton et al., 2022). Relative to this literature, our results connect social media, retail traders, and market outcomes, and we show that new entrants lead to much of the decline in informativeness of social media signal following the GME phenomenon.[^7] This finding highlights how the content of previously informative signals can change upon the arrival of new participants, and that this is a general phenomenon that is not confined to one social network.

[^7]: In connecting social media and retail trading, we also relate to the literature that studies motivations for retail trade (Liu et al., 2020). Prior work shows how peer interactions lead to excessive trading and exacerbate behavioral biases (Heimer, 2016), and emphasizes the role of overconfidence (Barber and Odean, 2001, Daniel and Hirshleifer, 2015), particularly about the precision of one's information (e.g., Daniel et al., 1998).

## 2. Data and summary statistics

### 2.1 Social media sentiment and attention data

Our data come from three investor social media platforms: Twitter, Seeking Alpha, and StockTwits. We obtain firm-day data on financially-oriented Twitter posts (tweets) from Social Market Analytics (SMA), a firm that provides sentiment information to professional investors. Specifically, we use daily 4pm snapshots of the number of tweets and average sentiment over the prior 24-hour period for each firm.

For Seeking Alpha, we obtain article-level sentiment from Ravenpack 1.0, keeping all articles with a relevance score above 75, which Ravenpack considers to be "significantly relevant." To measure sentiment, we use the Event Sentiment Score (ESS) calculated by Ravenpack, which ranges between -1 and 1, with 0 indicating neutral sentiment and positive (negative) values indicating positive (negative) sentiment.

For the investor social platform StockTwits, we obtain comprehensive message-level data. Like Twitter, StockTwits allows users to publicly post short messages (henceforth "tweets") with a limited number of characters – 140 before May 8, 2019, and 1,000 thereafter. Unlike Twitter, StockTwits is primarily focused on financial markets. By including a "cashtag," a dollar sign (\$) followed by a ticker symbol, StockTwits users can specify that their post refers to a specific firm or security. We limit our analysis to messages that mention exactly one company, so we can accurately assign sentiment to the company. We have data on all single-firm tweets from 2010 through 2021: 150 million tweets from over 800,000 users. Similar to Cookson et al. (2022a), we drop users posting over 1,000 tweets in a day, and we restrict our sample to the top 1,500 firms by the number of tweets posted between 2010 and 2021.

StockTwits allows users to attach a sentiment tag to their tweet indicating if their tweet reflects "bullish" or "bearish" sentiment. We assign +1 to self-labeled "bullish" tweets and -1 to self-labeled "bearish" tweets. We also obtain a sentiment score for each tweet ranging from -1 (extremely bearish) to +1 (extremely bullish) which is calculated by StockTwits using a proprietary text classification algorithm called MarketLex.[^8]

[^8]: According to StockTwits, this methodology uses lexical and semantic rules based on a custom-built lexicon for social finance, constructed from a combination of words and phrases from 4 million messages with user-provided bullish or bearish tags and manual human supervision.

To aggregate sentiment at the firm-day level ($Sentiment_{i,t}$) for StockTwits and Seeking Alpha, we compute average sentiment across all tweets (or articles) about a firm $i$ from 4:00 pm (close) on date $t-1$ to 4:00 pm on date $t$. These firm-day sentiment measures are thus comparable to the Twitter firm-day sentiment measure provided by SMA. Similarly, we compute firm-day message volume ($Messages_{i,t}$) for StockTwits and Seeking Alpha by counting the number of messages (tweets or articles) about each firm over the same period. We then define a firm-day measure of attention, $Attention_{i,t}$, for each platform by dividing the firm-day number of messages by the total number of messages on that platform in a day:[^9]

$$Attention_{i,t} = \frac{Messages_{i,t}}{\sum_i Messages_{i,t}} \tag{1}$$

[^9]: Our results are robust to using an alternate firm-day measure of attention: the deviation from its median number of messages over the preceding 10 days. See Appendix Tables A2 and A7.

StockTwits users can voluntarily declare their level of experience using the options provided when filling out their user profile. StockTwits also provides information on how many followers each user has. Thus, for StockTwits, we can separate sentiment and attention into distinct series by user profile or follower base: Professionals, Intermediates, Novices, No experience label, and Influencers (> 99th percentile by number of followers). We also produce a separate series for self-classified sentiment (explicit bullish/bearish declarations), as opposed to StockTwits' sentiment measure based on MarketLex.

### 2.2 Firm news data

In addition to social media sentiment and attention, we also control for firm news events. Specifically, we collect information on coverage and sentiment of traditional news media from the Wall Street Journal and the Dow Jones Newswire. These measures come from Ravenpack 1.0, which provides information on the number of articles by firm-day as well as article-level sentiment. We keep all articles with a relevance score above 75 and use the Ravenpack Event Sentiment Score, aggregating the article-level sentiment to the firm-day level by averaging firm-specific sentiment across articles within a day.

To capture other sources of news, we collect information on 8-K filing dates (unscheduled firm-specific news) and earnings announcement dates. The 8-K filing dates are collected from the SEC Analytics Suite by WRDS, and the earnings announcement dates are from I/B/E/S.

### 2.3 Returns data

We compute daily abnormal returns by subtracting the value-weighted market return from the firm's daily return using CRSP data.

### 2.4 Sample Characteristics

To allow accurate measurement of the social signal, our sample focuses on the 1,500 firms with the most single-firm tweets about them on StockTwits between 2010 and 2021. Although this reduces the number of firms in our sample from more than 9,000 to 1,500, it only reduces the number of StockTwits messages by about 20% (from 150 million to 120 million). We also restrict attention to firm-days for which there are at least 10 single-firm tweets on StockTwits. Because Twitter and Seeking Alpha data are sparsely populated before 2012, we begin our analysis sample in 2012. After merging the social media data with Ravenpack for traditional news media information and market data for return reactions, we obtain a final sample of roughly 815,000 firm-day observations.

Sample summary statistics are reported in Table 1. Panel A presents statistics on activity across the three platforms. For the average firm-day, the number of messages on StockTwits is a multiple of the number on Twitter or Seeking Alpha. Despite this substantial difference in message volume, the three platforms cover a similar number of firms (i.e., StockTwits mentions cover 1,497 firms in our final sample compared with just under 1,300 for Twitter, and Seeking Alpha). Thus, even if individual messages on StockTwits were to contain less information than a Seeking Alpha post, the greater volume of messages on StockTwits could aggregate into an informative firm-day signal. In Panel B, we present the same statistics for subgroups of StockTwits investors. This decomposition highlights that there is significant activity within each subgroup (the average number of posts ranges from 5.87 to 13.37).

Panel C illustrates how platforms differ in terms of the size of firms they pay attention to. The first three columns show the size distribution of the top 1,500 most talked-about firms on each platform, split into small-cap, mid-cap and large-cap bins. The three firm size bins each capture about a third of the most popular firms on Twitter and Seeking Alpha, while two-thirds of firms most discussed on StockTwits are small-cap. The second three columns present the share of messages discussing firms in each size bin. Large firms typically attract the most messages: around 60% of messages on Twitter and Seeking Alpha, despite accounting for a much smaller share of the firm-level coverage. By contrast, StockTwits still shows a small-cap focus at the message-level, with comparatively little difference between the shares of messages and of firms in each bin.

Panel D shows how restricting our sample to firm-days with at least 10 StockTwits messages affects the observation count in the sample. The firm-day sample size falls from nearly 2.8 million to roughly 821,000 observations. Additional sample filters (e.g., requiring data on controls or returns) have a negligible impact on our observation count.

### Table 1: Summary Statistics

- **Table type:** Summary statistics
- **Unit of observation:** Firm-day (Panels A, B, D); firm and message shares (Panel C)
- **Sample:** Firm-day observations with at least 10 StockTwits messages; Jan. 1, 2012 to Dec. 31, 2021

#### Panel A: Statistics by social media platform

| platform | sentiment_mean | sentiment_sd | sentiment_min | sentiment_max | messages_mean | messages_sd | messages_min | messages_max | firms_ever_mentioned | firms_all | firm_days_mentioned | firm_days_all |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| StockTwits | 0.10 | 0.14 | -0.97 | 0.97 | 132.40 | 734.97 | 10 | 138,280 | 1,497 | 1,500 | 815,980 | 815,980 |
| Twitter | 0.02 | 0.06 | -0.80 | 0.94 | 18.84 | 62.69 | 0 | 7,160 | 1,271 | 1,500 | 522,284 | 815,980 |
| Seeking Alpha | 0.02 | 0.12 | -1 | 1 | 0.46 | 1.75 | 0 | 150 | 1,283 | 1,500 | 137,018 | 815,980 |

#### Panel B: Statistics by user type on StockTwits

| user_type | sentiment_mean | sentiment_sd | sentiment_min | sentiment_max | messages_mean | messages_sd | messages_min | messages_max | users_n | users_share | firm_days_nonzero | firm_days_all |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Top 1% | 0.07 | 0.29 | -1 | 1 | 5.97 | 34.04 | 0 | 4,212 | 7,173 | 0.01 | 512,549 | 815,980 |
| Professional | 0.09 | 0.30 | -1 | 1 | 7.89 | 28.92 | 0 | 2,405 | 20,073 | 0.02 | 591,383 | 815,980 |
| Intermediate | 0.09 | 0.29 | -1 | 1 | 13.37 | 50.88 | 0 | 5,439 | 45,156 | 0.05 | 687,993 | 815,980 |
| Novice | 0.07 | 0.29 | -1 | 1 | 5.87 | 26.18 | 0 | 3,645 | 34,118 | 0.04 | 514,773 | 815,980 |
| No label | 0.10 | 0.18 | -0.99 | 0.99 | 105.27 | 658.60 | 0 | 127,243 | 730,164 | 0.88 | 810,614 | 815,980 |

*Conversion note: the dispersion column header is printed as "S.D." in Panel A and "DS." in Panel B of the original; both are rendered here as `sentiment_sd` / `messages_sd`.*

#### Panel C: Stock characteristics by social media platform

| size_bin | share_of_firms_StockTwits_pct | share_of_firms_Twitter_pct | share_of_firms_SeekingAlpha_pct | share_of_messages_StockTwits_pct | share_of_messages_Twitter_pct | share_of_messages_SeekingAlpha_pct |
|---|---:|---:|---:|---:|---:|---:|
| Small-cap | 68.60 | 30.07 | 30.67 | 54.27 | 16.13 | 18.27 |
| Mid-cap | 15.13 | 36.20 | 37.27 | 15.41 | 22.21 | 24.65 |
| Large-cap | 16.27 | 33.73 | 32.07 | 30.32 | 61.66 | 57.09 |

#### Panel D: Firm-day observations satisfying sample restriction

| sample_restriction | n_obs | n_dropped_obs |
|---|---:|---:|
| Full sample | 2,795,852 | - |
| At least 10 StockTwits messages | 821,534 | 1,974,318 |
| Non-missing controls data | 815,980 | 5,554 |
| Non-missing controls + returns | 814,646 | 1,334 |

**Note:** Panel A reports statistics on the firm-day level sentiment and attention by social media platform for all observations with at least 10 StockTwits messages. The sample time frame is Jan. 1, 2012 to Dec. 31, 2021 for StockTwits, Twitter, and Seeking Alpha. "# of firms - Ever mentioned" refers to the # of firms ever mentioned on a platform during our sample period; "# of firms - All" refers to the # firms included in our analysis sample (with the sentiment of firms not mentioned replaced by zeros). "Firm-day observations - Mentioned" refers to the # of firm-day observations with non-zero attention; "firm-day observations - All" refers to the # of firm-day observations in our analysis sample. Panel B provides similar statistics by user type on StockTwits. "Users - # (or Share)" refers to the # (or share) of StockTwits users of a certain type; Panel C reports the share of the 1,500 most talked-about firms on each platform that are in each of three market capitalization bins (first three columns), and the share of messages about firms in each bin (columns 4-6). "Small-cap," "mid-cap," and "large-cap" refer to stocks with market capitalizations below 2 bn., between 2 and 10 bn., and above 10 bn. Panel D shows how sample restrictions reduce the # of firm-day observations to arrive at our analysis sample.

### 2.5 Platform features and users

Communication theory (e.g., McLuhan, 1975) holds that the characteristics of a communication medium affect both the content and impact of its message. Thus, differences between platforms – in user populations, incentives to post, and ability to engage – may lead to important differences in the information each platform attracts and aggregates. Figure 1 presents three messages about Apple Stock (\$AAPL), one from each investor social media platform, in order to illustrate cross-platform differences.

### Figure 1: Examples of Posts Across Three Social Media Platforms

- **Panels:** (a) StockTwits; (b) Twitter; (c) Seeking Alpha
- **Content:** Screenshots of one example post per platform, all about Apple stock (AAPL) on the same day. The StockTwits post is a short message tagged "Bullish" with the \$AAPL cashtag; the Twitter post is a tweet with the \$AAPL cashtag; the Seeking Alpha post shows a long-form article title and bullet-point summary (article dated Sep. 26, 2022, with comment and like counts displayed).

**Note:** This figure presents example posts for StockTwits, Twitter, and Seeking Alpha. For ease of direct comparison, all three examples are about Apple stock (AAPL) on the same day (September 28, 2022). Only the summary is presented for the Seeking Alpha post; the full post is much longer.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

The most immediate difference in Figure 1 is that Seeking Alpha content consists of long-form articles (the screenshot displays only the title and summary), in contrast to the short posts on StockTwits and Twitter. There are many other platform feature differences. For example, although StockTwits and Twitter both allow "cashtags," only on StockTwits can posts be flagged as bullish or bearish by the poster. Moreover, StockTwits is an investment-specific platform, while Twitter covers an unrestricted variety of topics. Other differences include the recommendation algorithms and the ability to thread tweets. Each of these can contribute to important discrepancies across platforms in both the social signal (sentiment and attention measures) as well as how the social signal relates to market outcomes. We exploit a change in one of these dimensions – when StockTwits increased their message character limit from 140 to 1,000 characters – to examine how platform features impact the information content on the platform.

Another major difference across social media platforms is that they attract different users. Seeking Alpha posters are much more selected than Twitter or StockTwits users, which are open to anyone who signs up for an account. StockTwits has historically attracted users aiming to build reputation via their posts: deletion of past posts is not possible. Moreover, interest in these platforms has shifted and grown markedly over time, as is clear from Appendix Figure A1. To explore the importance of user composition, we test whether newer StockTwits users provide a less informative signal around a notable market event: the GME short squeeze of early 2021. We also use our within-StockTwits decomposition of different user types to examine how each type contributes to the social signal.

## 3. Decomposing the social signal

This section describes the commonalities and differences in the signals drawn from different social media investing platforms and across StockTwits investor types. Here, we distinguish between two key dimensions of the social signal: sentiment and attention.

### 3.1 Are social signals common across platforms?

We begin by examining how much commonality there is in the social signal across StockTwits, Twitter, and Seeking Alpha. Figure 2 and Panel A of Table 2 present the correlations of attention and sentiment between StockTwits and corresponding measures on Twitter and Seeking Alpha at the firm-day level. As a benchmark, we also present the correlations of StockTwits with traditional news coverage and sentiment from the Dow Jones Newswire (DJNW) and the Wall Street Journal (WSJ). The correlation between attention series on social platforms is relatively high at 0.595 between StockTwits and Twitter attention, and 0.398 between StockTwits and Seeking Alpha. By comparison, the correlations with coverage by traditional news media are much weaker: 0.163 for the WSJ and 0.144 for the DJNW. These correlations suggest that attention across social investing platforms contains a strong common component that is not well explained by news media coverage.

In contrast to the attention correlations, we observe much weaker correlations in sentiment series across different platforms. The correlation of StockTwits with Twitter sentiment is only 0.125, whereas the correlation with Seeking Alpha sentiment is 0.038. The correlation with news sentiment is also low, at 0.010 for the WSJ and 0.069 for the DJNW. This suggests that sentiment is more idiosyncratic across social investing platforms, and as Figure 2 highlights, the difference in the magnitudes of the correlations for attention and sentiment is striking.

*[Conversion note: the prose on this point in the original gives DJNW correlations of 0.144 (attention) and 0.069 (sentiment), while Table 2 Panel A prints 0.220 and 0.032 respectively. Both are transcribed exactly as printed in their respective locations; the discrepancy is in the source document.]*

### Figure 2: Cross-platform Correlation of Social Signals

- **Panels:** (a) Attention signal; (b) Sentiment signal
- **Chart type:** Bar charts of bivariate correlations between StockTwits and each of: Twitter, Seeking Alpha, DJNW, WSJ
- **Axes:** y-axis "Correlation" from 0 to 1; bars grouped by comparison series (legend: Twitter, Seeking Alpha, DJNW, WSJ)

**Note:** This figure reports the bivariate correlations of attention and sentiment signals between StockTwits and other platforms or news sources at the firm-day level. Attention is measured as the fraction of messages, reports, or articles about a firm across all firms on a platform in a day. Sentiment is measured as the average sentiment of all messages about a firm on a platform in a day.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred. (The underlying correlations appear in Table 2, Panel A.)

A priori, there are various plausible hypotheses about how the six signals we analyze could be cross-correlated. For example, sentiment and attention signals could have a strong correlation with one another under the theory that people pay attention to what they feel strongly about. Alternatively, people with similar outlooks could cluster within platforms, leading to correlation within platform between attention and sentiment. It is also not clear that the strongest cross-correlations are positive. If disagreement across platforms in sentiment or attention were the norm, we would expect to see negative cross-platform correlations. In the following analysis, our main finding is that the strongest cross-correlations are attention across platforms and sentiment across platforms, with little within-platform clustering or correlation between attention and sentiment signals.

To systematically describe the cross-correlation of the six signals (attention and sentiment for each of the three platforms), we employ principal components analysis (PCA). PCA provides a convenient way to describe the multivariate correlations across attention and sentiment signals on the social platforms. The first principal component (PC1) from a PCA yields the linear combination of the signals that explain the most variation across the six signals. The second principal component (PC2) is the linear combination that explains the most of the remaining variation, and so on. Thus, if the loadings on the underlying signals are large within a principal component, these signals are mutually correlated. In other words, the loadings identify the clustering of signals within the data. Further, a standard output from PCA is the fraction of variation explained by each principal component. This is a useful summary statistic of how much cross-correlation there is in each principal component for the signals that matter most to it.

To gauge the extent to which sampling variability determines our ability to draw conclusions about PC loadings and explained variation, we compute standard errors for the loadings and the fraction of variation explained by each PC by conducting a block bootstrap procedure that clusters standard errors by firm and by date. To do this, we separately conduct a block bootstrap by firm and by date, drawing 1,000 replications from each. Then, we follow the formula in Thompson (2011) to compute the double clustered variance-covariance matrix from each single clustered variance-covariance matrix. Throughout our analysis, we obtain relatively small standard errors, indicating that the statistics we focus on from the PCA are sufficiently precise. For table legibility, we suppress the reporting of standard errors on the PC loadings in later tables.

Panel B of Table 2 presents the PCA across the six signals we consider in this paper (i.e., sentiment and attention across the three platforms at the firm-day level). PC1 explains 35.6% of the variation across the six signals, which is nearly twice the variation explained in PC2. Moreover, PC1 is roughly an equal-weighted average of attention signals, with low loadings on sentiment signals. Almost a mirror of PC1, PC2 is roughly an equal weighted average of sentiment signals, with low loadings on attention signals. This structure implies that sentiment and attention have a low correlation, and motivates our subsequent approach of using separate PCAs for attention signals and for sentiment signals.

### Table 2: How Common is Sentiment and Attention across Platforms?

- **Table type:** Correlation (Panel A) and PCA loadings (Panels B, C)
- **Unit of observation:** Firm-day
- **Standard errors:** In parentheses; double clustered by firm and by date via a block bootstrap procedure following Thompson (2011)
- **Significance:** not reported in table note

#### Panel A: Correlations with the StockTwits Signal

| variable | Twitter | Seeking Alpha | DJNW | WSJ |
|---|---:|---:|---:|---:|
| StockTwits attention | 0.595 | 0.398 | 0.220 | 0.163 |
| StockTwits sentiment | 0.125 | 0.038 | 0.032 | 0.010 |

#### Panel B: PCA of All Platform-Level Signals

| signal | statistic | PC1 | PC2 | PC3 | PC4 | PC5 | PC6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Attention: StockTwits | loading | 0.548 | -0.130 | -0.188 | 0.047 | 0.638 | 0.488 |
| Attention: StockTwits | standard_error | 0.052 | 0.107 | 0.292 | 0.069 | 0.155 | 0.076 |
| Attention: Twitter | loading | 0.605 | -0.033 | -0.098 | -0.009 | 0.048 | -0.788 |
| Attention: Twitter | standard_error | 0.013 | 0.050 | 0.126 | 0.016 | 0.142 | 0.025 |
| Attention: Seeking Alpha | loading | 0.548 | -0.007 | 0.052 | 0.084 | -0.745 | 0.368 |
| Attention: Seeking Alpha | standard_error | 0.017 | 0.047 | 0.180 | 0.021 | 0.212 | 0.117 |
| Sentiment: StockTwits | loading | -0.031 | 0.644 | -0.345 | 0.682 | 0.017 | -0.014 |
| Sentiment: StockTwits | standard_error | 0.014 | 0.011 | 0.337 | 0.010 | 0.056 | 0.006 |
| Sentiment: Twitter | loading | 0.082 | 0.647 | -0.225 | -0.720 | -0.008 | 0.071 |
| Sentiment: Twitter | standard_error | 0.046 | 0.041 | 0.282 | 0.013 | 0.035 | 0.024 |
| Sentiment: Seeking Alpha | loading | 0.160 | 0.384 | 0.885 | 0.087 | 0.190 | 0.008 |
| Sentiment: Seeking Alpha | standard_error | 0.070 | 0.021 | 0.737 | 0.040 | 0.221 | 0.051 |
| Fraction of variation | estimate | 35.6% | 19.3% | 15.9% | 14.5% | 9.2% | 5.5% |
| Fraction of variation | standard_error | 4.284 | 0.124 | 0.482 | 0.085 | 2.240 | 1.638 |

#### Panel C: PCA of Platform-Level Attention or Sentiment Signals

| signal_set | platform | statistic | PC1 | PC2 | PC3 |
|---|---|---|---:|---:|---:|
| Attention | StockTwits | loading | 0.565 | -0.665 | 0.489 |
| Attention | StockTwits | standard_error | 0.027 | 0.592 | 0.073 |
| Attention | Twitter | loading | 0.614 | -0.057 | -0.787 |
| Attention | Twitter | standard_error | 0.029 | 0.075 | 0.020 |
| Attention | Seeking Alpha | loading | 0.551 | 0.745 | 0.376 |
| Attention | Seeking Alpha | standard_error | 0.022 | 0.620 | 0.109 |
| Attention | Fraction of variation | estimate | 67% | 18.9% | 11.1% |
| Attention | Fraction of variation | standard_error | 9.336 | 6.033 | 3.360 |
| Sentiment | StockTwits | loading | 0.611 | -0.464 | 0.642 |
| Sentiment | StockTwits | standard_error | 0.006 | 0.021 | 0.010 |
| Sentiment | Twitter | loading | 0.662 | -0.147 | -0.735 |
| Sentiment | Twitter | standard_error | 0.003 | 0.015 | 0.002 |
| Sentiment | Seeking Alpha | loading | 0.435 | 0.874 | 0.217 |
| Sentiment | Seeking Alpha | standard_error | 0.009 | 0.009 | 0.024 |
| Sentiment | Fraction of variation | estimate | 38.8% | 32.3% | 29% |
| Sentiment | Fraction of variation | standard_error | 0.170 | 0.069 | 0.144 |

**Note:** This table reports the correlations and principal component analyses of social signals across platforms. Panel A reports the bivariate correlations of attention and sentiment between StockTwits and another platform. Panel B reports the principal components of attention and sentiment signals in one analysis, while panel C reports the principal components separately for attention (columns 1-3) and for sentiment (columns 4-6). Standard errors in parentheses are double clustered by firm and by date via a block bootstrap procedure following Thompson (2011).

Next, we describe the common variation between social media signals in PCAs for attention, and separately for sentiment. These PCAs are summarized in Panel C of Table 2. Consistent with the view that attention is common across investors on various social media platforms, PC1 of attention explains 67.0% of the variation across platforms. Further, all three attention signals are given similar positive weights in this first PC, suggesting a natural interpretation that the common component of attention is manifested in all three social media platforms. PC2 captures differences in attention across Seeking Alpha and StockTwits since it places positive weight on Seeking Alpha and negative weight on StockTwits (with roughly zero weight on Twitter). However, these differences in attention across platforms captured by the second PC only explain 18.9% of the variation in attention.

Turning to the sentiment PCA, the first PC only explains 38.8% of sentiment variation across platforms. This is a weak common component, because purely idiosyncratic variation in the three series would result in a first PC explaining 33.3%. Like the attention PCA, the second PC of sentiment mostly captures the difference between Seeking Alpha (positive weight, $w = 0.874$) and StockTwits (negative weight, $w = -0.464$) since the Twitter sentiment series has a much smaller weight ($w = -0.147$). The fact that the second PC explains 32.3% of the variation implies that differences across platforms in sentiment capture approximately as much variation across platforms as similarities. These results suggest that, for any given firm or day, attention-related results from the social finance literature are more likely to generalize than results concerning sentiment.

### 3.2 Conditional PCAs to account for confounding effects of news and firm characteristics

The results in the prior PCA are unconditional, and therefore could be driven by many omitted variables. For example, news coverage or firm announcements could drive attention and sentiment to co-vary across platforms. Naturally, we want to control for this. One approach would be to regress a signal on the other signals, while controlling for news controls and firm fixed effects. However, this does not isolate the correlations across platforms that are of interest to us: for example, in a regression of Stocktwits sentiment on Twitter and Seeking Alpha sentiment, the coefficient on Twitter sentiment holds constant Seeking Alpha sentiment, which is not the variation we are interested in. Thus, we adopt a conditional PCA approach. In a conditional PCA, the input signals are first regressed on controls and fixed effects to orthogonalize the signal with respect to confounding variation. We run regressions of the following form for each of the six signals:

$$Signal^P_{i,t} = \Gamma^P X_{i,t} + \gamma^P_i + \epsilon_{it}, \tag{2}$$

where $Signal^P_{i,t}$ is either attention or sentiment on a platform $P$ for firm $i$ on day $t$; $X_{i,t}$ are controls for traditional news for firm $i$ on day $t$; $\gamma^P_i$ are firm fixed effects. Then, we extract the residual from each signal series and perform the PCA on the 6 residualized signals.

Table 3 Panels A and B first residualize by news only, that is, traditional media coverage of firm $i$ on date $t$ drawn from RavenPack. RavenPack provides both the number of articles about firm $i$ on date $t$, as well as the sentiment of those articles. We control for both sentiment and number of articles. We also include an indicator variable for whether there is an earnings announcement on date $t$ for firm $i$, as well as lags of up to 7 days; we do the same for 8-K disclosures. The aim is to flexibly control for news in the residualization step. In the next three columns of both panels, we residualize by news and also add firm fixed effects to control for any unobserved and time-invariant firm characteristics. Finally, in the last three columns of both panels, we further residualize by lagged return volatility and cumulative abnormal returns.

As Table 3 shows, our controls for news, time-invariant firm characteristics, and lagged returns do not change the qualitative conclusion that attention is highly correlated across social media platforms, while sentiment has a more modest correlation. Instead of the first PC of attention explaining 67% of the variation across platforms, residualized attention explains 64 to 66% of the variation. Sentiment is even more insensitive to controlling for news and firm fixed effects. Relative to the 38.8% in the unconditional PCA of sentiment, the conditional PCA results in a first PC that explains 38 to 38.2% of the variation across platforms. More than showing robustness to controlling for news and other confounding factors, these findings indicate that there is a strong cross-correlation in the information shared on social media platforms that is largely independent of news.[^10] That is, the information on social media is not simply a reflection of traditional news, firm disclosures, and recent market conditions.

[^10]: When social media posts are not talking about firm news, what do they talk about? There are many potential non-news topics. Typical examples include how national or international events affect the focal firm, or how news about competitors does.

### Table 3: How Common is the Social Signal across Platforms? Conditional on News and Firm Fixed Effects

- **Table type:** PCA loadings (residualized signals)
- **Unit of observation:** Firm-day
- **Residualization sets:** (i) news only; (ii) news & firm fixed effects; (iii) news, firm fixed effects, & lagged returns/volatility
- **Standard errors:** In parentheses (reported for fraction of variation only); double clustered by firm and by date via a block bootstrap procedure following Thompson (2011)
- **Significance:** not reported in table note

#### Panel A: PCA of Residualized Attention Signals

| residualization | platform | statistic | PC1 | PC2 | PC3 |
|---|---|---|---:|---:|---:|
| News | StockTwits | loading | 0.582 | -0.548 | 0.601 |
| News | Twitter | loading | 0.616 | -0.185 | -0.766 |
| News | Seeking Alpha | loading | 0.531 | 0.815 | 0.230 |
| News | Fraction of variation | estimate | 66.4% | 21% | 12.7% |
| News | Fraction of variation | standard_error | 8.768 | 5.200 | 3.666 |
| News & firm | StockTwits | loading | 0.608 | -0.421 | 0.674 |
| News & firm | Twitter | loading | 0.627 | -0.266 | -0.732 |
| News & firm | Seeking Alpha | loading | 0.487 | 0.867 | 0.103 |
| News & firm | Fraction of variation | estimate | 63.4% | 24.1% | 12.5% |
| News & firm | Fraction of variation | standard_error | 7.898 | 4.449 | 3.536 |
| News, firm, & returns | StockTwits | loading | 0.606 | -0.427 | 0.671 |
| News, firm, & returns | Twitter | loading | 0.626 | -0.266 | -0.733 |
| News, firm, & returns | Seeking Alpha | loading | 0.492 | 0.864 | 0.106 |
| News, firm, & returns | Fraction of variation | estimate | 63.5% | 23.9% | 12.6% |
| News, firm, & returns | Fraction of variation | standard_error | 8.151 | 4.513 | 3.716 |

#### Panel B: PCA of Residualized Sentiment Signals

| residualization | platform | statistic | PC1 | PC2 | PC3 |
|---|---|---|---:|---:|---:|
| News | StockTwits | loading | 0.639 | -0.376 | 0.671 |
| News | Twitter | loading | 0.675 | -0.144 | -0.724 |
| News | Seeking Alpha | loading | 0.369 | 0.915 | 0.162 |
| News | Fraction of variation | estimate | 38.2% | 32.8% | 29.1% |
| News | Fraction of variation | standard_error | 0.159 | 0.054 | 0.142 |
| News & firm | StockTwits | loading | 0.660 | -0.288 | 0.694 |
| News & firm | Twitter | loading | 0.676 | -0.174 | -0.716 |
| News & firm | Seeking Alpha | loading | 0.327 | 0.942 | 0.080 |
| News & firm | Fraction of variation | estimate | 38.2% | 32.8% | 29% |
| News & firm | Fraction of variation | standard_error | 0.134 | 0.038 | 0.125 |
| News, firm, & returns | StockTwits | loading | 0.660 | -0.289 | 0.694 |
| News, firm, & returns | Twitter | loading | 0.676 | -0.173 | -0.716 |
| News, firm, & returns | Seeking Alpha | loading | 0.327 | 0.942 | 0.081 |
| News, firm, & returns | Fraction of variation | estimate | 38% | 32.8% | 29.2% |
| News, firm, & returns | Fraction of variation | standard_error | 0.134 | 0.038 | 0.125 |

**Note:** This table repeats the principal component analysis in Table 2 using the residualized social signal. The residualized signal in columns 1-3 refers to the residual from regressing a signal on DJNW sentiment (lagged 0 through 7 days), DJNW attention (lagged 0 through 7 days), dummies for earnings announcements (lagged 0 through 7 days), dummies for 8-k filings (lagged 0 through 7 days); in columns 4-6, we also residualize out firm fixed effects; in columns 4-6, we further residualize out lagged return volatility (previous five trading days) and lagged cumulative abnormal returns (previous five trading days and the 25 days before that). Standard errors in parentheses are double clustered by firm and by date via a block bootstrap procedure following Thompson (2011). *[Conversion note: the original note attributes both the firm-FE and lagged-returns residualizations to "columns 4-6"; the second instance presumably refers to columns 7-9. Transcribed as printed.]*

To ensure that these results are not driven by the way we define social media attention in Equation 1, Appendix Table A2 reproduces the analyses in Tables 2 and 3 using an alternate firm-day attention measure: the deviation from the median number of messages over the preceding 10 days ("abnormal attention"). The PCA loadings are very similar, and fraction of variation explained by each PC shows the same pattern, albeit with PC1's share falling to around 50%. To further alleviate this concern, we construct an extensive margin measure of attention: whether a stock is mentioned on a platform ("coverage"). Appendix Table A3 shows that the cross-platform correlations for coverage are lower, at around half the level shown for our main attention measure. However, despite this being an extensive margin measure, the PCA shows similar results to those for abnormal attention.[^11]

[^11]: In Appendix Table A4 we include Reddit's WallStreetBets (WSB) sentiment and attention as additional signals in the conditional PCA. Our findings are unchanged: PC1 of attention explains approximately double the baseline variation (51.1% vs. 25%), while PC1 of sentiment remains barely above the baseline.

### 3.3 Heterogeneity by Firm Size

There are clear differences in coverage across platforms by firm size: StockTwits over-represents small stocks relative to Twitter and Seeking Alpha. Thus, we explore heterogeneity by firm size by performing a separate PCA for firms within different size bins: small (below \$2 billion in market cap), medium (between \$2 billion and \$10 billion), and large (above \$10 billion). For clarity, the heterogeneity analysis reports only the first PC; our main interest is in evaluating this component's strength, loadings, and how it varies by firm size.

Table 4 reports the results. We find that large firms have more commonality in both attention and sentiment signals than do medium and small firms. Moreover, within each size bucket, the main conclusion of the PCA holds: attention is more correlated than is sentiment. However, there is meaningful heterogeneity across the size distribution in the strength of the first PC. Panels A and B present the unconditional PCA results. For attention, the first PC explains 49.5% of variation for small firms, but this increases to 72.5% for large firms. Sentiment's first PC is stronger for large firms (42.4%) than for small firms (36.3%). Panels C and D present the results of the conditional PCA. Similar to our main findings, residualizing attenuates the strength of the first PC slightly, but it does not change the qualitative conclusion. Notably, differences in news and time-invariant firm characteristics do not explain the heterogeneity across the size distribution, which remains pronounced in the conditional PCA.

### Table 4: How Common is the Social Signal across Platforms? Heterogeneity in First Principal Component (PC1) by Firm Size

- **Table type:** PCA loadings (PC1 only), by firm size bin
- **Unit of observation:** Firm-day
- **Size bins:** "small" = market capitalization below \$2 billion; "medium" = between \$2 and \$10 billion; "large" = above \$10 billion
- **Standard errors:** In parentheses (fraction of variation only); double clustered by firm and by date via a block bootstrap procedure following Thompson (2011)
- **Significance:** not reported in table note

#### Panel A: PC1 of Attention Signals by Firm Size

| variable | statistic | Small | Medium | Large |
|---|---|---:|---:|---:|
| StockTwits | loading | 0.577 | 0.620 | 0.566 |
| Twitter | loading | 0.653 | 0.652 | 0.615 |
| Seeking Alpha | loading | 0.490 | 0.436 | 0.549 |
| Fraction of variation | estimate | 49.5% | 58.9% | 72.5% |
| Fraction of variation | standard_error | 1.225 | 1.009 | 10.168 |

#### Panel B: PC1 of Sentiment Signals by Firm Size

| variable | statistic | Small | Medium | Large |
|---|---|---:|---:|---:|
| StockTwits | loading | 0.637 | 0.659 | 0.643 |
| Twitter | loading | 0.661 | 0.665 | 0.670 |
| Seeking Alpha | loading | 0.397 | 0.352 | 0.372 |
| Fraction of variation | estimate | 36.3% | 40.1% | 42.4% |
| Fraction of variation | standard_error | 0.129 | 0.258 | 0.288 |

#### Panel C: PC1 of Residualized Attention Signals by Firm Size

| residualization | variable | statistic | Small | Medium | Large |
|---|---|---|---:|---:|---:|
| News | StockTwits | loading | 0.634 | 0.664 | 0.577 |
| News | Twitter | loading | 0.668 | 0.675 | 0.618 |
| News | Seeking Alpha | loading | 0.390 | 0.321 | 0.534 |
| News | Fraction of variation | estimate | 46% | 54.4% | 69.4% |
| News | Fraction of variation | standard_error | 1.167 | 1.047 | 9.060 |
| News & firm FEs | StockTwits | loading | 0.647 | 0.671 | 0.609 |
| News & firm FEs | Twitter | loading | 0.672 | 0.681 | 0.627 |
| News & firm FEs | Seeking Alpha | loading | 0.360 | 0.293 | 0.485 |
| News & firm FEs | Fraction of variation | estimate | 45.7% | 54.4% | 68.1% |
| News & firm FEs | Fraction of variation | standard_error | 1.139 | 0.798 | 7.651 |

#### Panel D: PC1 of Residualized Sentiment Signals by Firm Size

| residualization | variable | statistic | Small | Medium | Large |
|---|---|---|---:|---:|---:|
| News | StockTwits | loading | 0.656 | 0.671 | 0.656 |
| News | Twitter | loading | 0.674 | 0.678 | 0.682 |
| News | Seeking Alpha | loading | 0.338 | 0.299 | 0.323 |
| News | Fraction of variation | estimate | 36% | 39.6% | 41.7% |
| News | Fraction of variation | standard_error | 0.122 | 0.274 | 0.274 |
| News & firm FE | StockTwits | loading | 0.669 | 0.673 | 0.659 |
| News & firm FE | Twitter | loading | 0.679 | 0.680 | 0.680 |
| News & firm FE | Seeking Alpha | loading | 0.300 | 0.291 | 0.320 |
| News & firm FE | Fraction of variation | estimate | 36.2% | 39.4% | 41.2% |
| News & firm FE | Fraction of variation | standard_error | 0.110 | 0.248 | 0.210 |

**Note:** This table reports heterogeneity in the first principal components from Table 2 panel C and Table 3 columns 1-6. The sample is split into three groups by firm size: "small" refers to stocks whose market capitalization is below 2 billion; "medium" those between 2 and 10 billion; "large" those above 10 billion. Standard errors in parentheses are double clustered by firm and by date via a block bootstrap procedure following Thompson (2011).

### 3.4 Similarities and differences in the social signal across user types

A potential explanation for the weak correlation of sentiment across platforms is that the different natural language processing (NLP) algorithms used for each platform may produce different measures from the same underlying text. We test whether NLPs are a major driver of the low correlation in sentiment signals by focusing on messages within StockTwits across types of users. The StockTwits data allow us to construct attention and sentiment signals separately for different investor subgroups. In this section, we disaggregate the StockTwits signal to separately consider the sentiment and attention of influencers (those in the top 1% by number of followers), professional users, intermediate users, novice users, and users who do not indicate an experience category ("no label").

Panel A of Table 5 presents the correlation of attention for each user subset on StockTwits with its complement at the firm-day level; for example, we compare the attention of the top 1% of users by followers with the remaining 99% in the first column. The correlations of attention across user groups on StockTwits range from 0.819 (top 1%) to 0.987 ("no label" users). In contrast to the high correlations for attention, those for sentiment are weak: correlations range from 0.166 (no label) to 0.088 (novices). These weak correlations in sentiment across user subgroups suggest that differences across user types are an important driver of differences in social media sentiment, because this analysis holds constant the NLP and platform features.

In Panels B and C, we repeat the conditional PCA using the signals from StockTwits subgroups. For brevity, these panels only report the first five PCs.[^12] Consistent with our cross-platform PCA, we see that attention contains a strong common component (84.3% of the variation captured by PC1) while sentiment's common component is weaker, capturing only 27.6%. The second PCs capture differences in attention or sentiment between the more sophisticated investors (top 1% and professionals) and the rest. In the attention PCA, PC3 and higher explain very little variation. In contrast, these components explain a non-trivial share of variation for sentiment. Thus, differences in NLPs across platforms cannot fully drive our results. Moreover, this within-StockTwits evidence suggests that, even if NLPs and all platform features were identical, we would see cross-platform differences in the sentiment signal due to differences in user populations.

[^12]: Appendix Table A1 presents results from the unconditional PCA analysis.

### Table 5: How Common is the Social Signal across User Types? Evidence from Users Groups on StockTwits

- **Table type:** Correlation (Panel A) and PCA loadings (Panels B, C)
- **Unit of observation:** Firm-day
- **Residualization (Panels B, C):** Residuals from regressing each signal on DJNW sentiment (lagged 0 through 7 days), DJNW attention (lagged 0 through 7 days), dummies for earnings announcements (lagged 0 through 7 days), dummies for 8-k filings (lagged 0 through 7 days), and firm fixed effects
- **Standard errors:** In parentheses (fraction of variation only); double clustered by firm and by date via a block bootstrap procedure following Thompson (2011)
- **Significance:** not reported in table note

#### Panel A: Correlations within StockTwits

| variable | Top 1% | Professional | Intermediate | Novice | No label |
|---|---:|---:|---:|---:|---:|
| StockTwits attention | 0.819 | 0.884 | 0.966 | 0.929 | 0.987 |
| StockTwits sentiment | 0.095 | 0.108 | 0.118 | 0.088 | 0.166 |

#### Panel B: PC1 of Residualized Attention Signals

| user_group | statistic | PC1 | PC2 | PC3 | PC4 | PC5 |
|---|---|---:|---:|---:|---:|---:|
| Top 1% | loading | 0.415 | 0.800 | 0.432 | 0.003 | -0.023 |
| Professional | loading | 0.443 | 0.195 | -0.783 | 0.372 | 0.121 |
| Intermediate | loading | 0.466 | -0.193 | -0.124 | -0.490 | -0.700 |
| Novice | loading | 0.445 | -0.464 | 0.423 | 0.632 | -0.094 |
| No label | loading | 0.465 | -0.263 | 0.081 | -0.471 | 0.698 |
| Fraction of variation | estimate | 84.3% | 7.2% | 4.6% | 2.3% | 1.5% |
| Fraction of variation | standard_error | 2.607 | 1.131 | 0.883 | 0.405 | 0.278 |

#### Panel C: PC1 of Residualized Sentiment Signals

| user_group | statistic | PC1 | PC2 | PC3 | PC4 | PC5 |
|---|---|---:|---:|---:|---:|---:|
| Top 1% | loading | 0.572 | -0.182 | -0.128 | 0.084 | -0.785 |
| Professional | loading | 0.472 | -0.398 | -0.473 | 0.311 | 0.547 |
| Intermediate | loading | 0.381 | 0.028 | 0.819 | 0.389 | 0.179 |
| Novice | loading | 0.281 | 0.896 | -0.271 | 0.201 | 0.062 |
| No label | loading | 0.476 | 0.062 | 0.126 | -0.839 | 0.222 |
| Fraction of variation | estimate | 27.6% | 19.5% | 19% | 17.9% | 16% |
| Fraction of variation | standard_error | 0.079 | 0.027 | 0.031 | 0.043 | 0.060 |

**Note:** This table reports the correlations and principal component analyses of social signals across different user types on StockTwits. Panel A reports the bivariate correlations of attention and sentiment between StockTwits signals from each user group and their complements. Panels B and C use residualized attention and sentiment signals, respectively, i.e., residuals from regressing each signal on DJNW sentiment (lagged 0 through 7 days), DJNW attention (lagged 0 through 7 days), dummies for earnings announcements (lagged 0 through 7 days), dummies for 8-k filings (lagged 0 through 7 days), and firm fixed effects. PCA of non-residualized social signals from StockTwits user subgroups are reported in Table A1. Standard errors in parentheses are double clustered by firm and by date via a block bootstrap procedure following Thompson (2011).

### 3.5 Are social signals persistent?

We now examine the persistence of attention and sentiment over time by computing the partial autocorrelation function (PACF) for each platform's attention and sentiment signal. In Appendix Figure A2, we compute the PACF for each series out to 20 lags (days). Attention (dashed lines) tends to have high autocorrelations at lag 1 (around 0.8) that decay to near zero after lag 5. By contrast, sentiment has low autocorrelations at lag 1 (between 0.1 and 0.25) and decays more rapidly to zero.

This constitutes another difference between attention and sentiment signals: attention exhibits a much greater and more persistent autocorrelation than does sentiment. We account for these underlying differences when we relate attention and sentiment to returns by controlling for 10 lags of each.

## 4. Informativeness of Social Media Signals

In the second part of our paper, we examine how the social signal relates to two outcomes typically studied by the literature: returns and retail order imbalance.

First, we explore the informativeness for future returns of the attention and sentiment signals from each social media platform. Note that the signals from each platform are a combination of a platform-specific or idiosyncratic component, and a common social signal component. For example, a coefficient in a regression between an outcome and only the Twitter signal captures the relation between the outcome and a combination of (i) a common social media component and (ii) a Twitter-specific component. In contrast, in a regression with signals from all three platforms, coefficients on signals from each platform reflect only how each platform-specific component relates to the outcome. The contrast between the coefficients from these two regressions captures how the common component of a particular platform's signal relates to returns. Moreover, the informativeness of the common and idiosyncratic components of each platform's signal may be aligned (i.e., they have the same sign and approximate magnitude) or misaligned. Importantly, cases of misalignment can generate differences in informativeness between the platform-specific signal and the common social signal.

### 4.1 Does the social signal predict future returns?

To examine whether the social signal predicts returns, we estimate the following specification:

$$
\begin{aligned}
Abnormal\ Returns_{i,t+\tau} = \ & \beta_1 Attention_{i,t} + \beta_2 Sentiment_{i,t} \\
& + \beta_3 Sentiment_{i,t} \times Attention_{i,t} + X_{i,t} \times \Gamma + \alpha_i + \alpha_t + \epsilon_{i,t}
\end{aligned} \tag{3}
$$

where the dependent variable $Abnormal\ Returns_{i,t+\tau}$ is in percentage points, and $\tau = 0, ..., 20$. $Attention_{i,t}$ and $Sentiment_{i,t}$ are firm-day measures from a particular platform or the principal components constructed in the previous section. In addition, the controls ($X_{i,t}$) include DJNW sentiment and attention, indicators for 8-K filing or earnings announcement days, lagged volatility ($t-1$ to $t-5$), lagged market returns (CAR $t-1$ to $t-5$ and $t-6$ to $t-30$), and firm and date fixed effects. We also control for log Google ASVI as an alternative measure of retail investor attention.[^13] We further control for lagged $Attention_{i,\eta}$ and $Sentiment_{i,\eta}$ (where $\eta = t-1, t-2, ..., t-10$) to account for the autocorrelation documented in the preceding section. Table 6 presents the results from estimating Equation (3) for next day ($t+1$) returns, with each column employing a different source of social signal.

[^13]: Abnormal Google search volume, is calculated following Niessner (2015): we take the daily Google SVI data for each ticker and divide by its median SVI between days t-56 and t-35. We then take the natural logarithm and replace missing values (caused by a missing median) with zero. The SVI data come from 200-day downloads with a day of overlap that we concatenate to ensure consistency across time.

The first column of Table 6 examines the informativeness for next-day returns of the common component in the social media signal captured by the first principal components (PC1s). We find that common social media sentiment is positively related to next day returns (a standard deviation increase predicts a 6.1 bps higher return), while attention is negatively related (-13 bps); note that these estimates of attention's relation to return are conditional on sentiment (and vice versa).[^14] Column 2 includes all six signals, so estimates reflect the platform-specific contributions of each platform's sentiment and attention to informativeness. We see that the informativeness of StockTwits' idiosyncratic component largely aligns with the common component, while those of the other two platforms do not. In particular, Twitter's idiosyncratic sentiment coefficient is near zero, while the attention coefficient is positive and large (+11 bps), making it substantially different from the negative common attention coefficient. Seeking Alpha's idiosyncratic sentiment is aligned with the common component, but it has a near-zero attention coefficient.

[^14]: In Appendix Table A5, we include PC2 and PC3 of sentiment, and we find informativeness of PC1 sentiment is unchanged.

Columns 3-5 reproduce this analysis using the signals from one platform at a time; these single-platform regressions make use of a mix of idiosyncratic and common information. We see that coefficient estimates on StockTwits attention and sentiment in column 3 are well-aligned with the common component coefficients in column 1, making them a good reflection of the overall social signal for next-day returns. By contrast, while Twitter and Seeking Alpha's sentiment coefficients are directionally aligned with the common component, their attention coefficients are not. Comparing columns 1 and 2, we see Twitter's idiosyncratic and common attention components offset each other, leading to a near-zero combined attention effect in column 4. For Seeking Alpha attention, we see that the platform-specific coefficient in column 5 matches the idiosyncratic one from column 2, which suggests that the platform's attention does not load on the common component.

Examining the control variables in the table is also informative. These specifications hold constant the attention and sentiment of traditional media via the DJNW attention and sentiment controls. The coefficient estimates on these controls provide an alternative benchmark: a one standard deviation increase in DJNW sentiment predicts 8 bps higher next-day returns, while there is not a significant relationship between DJNW attention and returns. Log Google ASVI negatively predicts next-day returns and is largely uncorrelated with the social signal measures: coefficients are essentially unchanged when log ASVI is omitted in untabulated results.

### Table 6: How Do Next-Day Returns Relate to Social Signals?

- **Table type:** Regression
- **Unit of observation:** Firm-day
- **Dependent variable:** $AR_{i,t+1}$ (%) — each security's abnormal return on day t+1 in percentage points
- **Estimator:** OLS with firm and date fixed effects
- **Standard errors:** In parentheses; double clustered by firm and by date
- **All columns include:** ten lags (t-1 to t-10) of sentiment and ten lags of attention
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | signal_source |
|---:|---|
| 1 | PC1s of sentiment and attention across the three platforms |
| 2 | All six platform signals jointly |
| 3 | StockTwits signals only |
| 4 | Twitter signals only |
| 5 | Seeking Alpha signals only |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| Sentiment PC1_{i,t}(z) | coefficient | 0.061*** | | | | |
| Sentiment PC1_{i,t}(z) | standard_error | 0.009 | | | | |
| Attention PC1_{i,t}(z) | coefficient | -0.131*** | | | | |
| Attention PC1_{i,t}(z) | standard_error | 0.050 | | | | |
| StockTwits sentiment_{i,t}(z) | coefficient | | 0.049*** | 0.053*** | | |
| StockTwits sentiment_{i,t}(z) | standard_error | | 0.008 | 0.008 | | |
| StockTwits attention_{i,t}(z) | coefficient | | -0.206*** | -0.151*** | | |
| StockTwits attention_{i,t}(z) | standard_error | | 0.056 | 0.051 | | |
| Twitter sentiment_{i,t}(z) | coefficient | | 0.011 | | 0.022*** | |
| Twitter sentiment_{i,t}(z) | standard_error | | 0.007 | | 0.007 | |
| Twitter attention_{i,t}(z) | coefficient | | 0.112*** | | -0.010 | |
| Twitter attention_{i,t}(z) | standard_error | | 0.031 | | 0.020 | |
| Seeking Alpha sentiment_{i,t}(z) | coefficient | | 0.079*** | | | 0.081*** |
| Seeking Alpha sentiment_{i,t}(z) | standard_error | | 0.010 | | | 0.010 |
| Seeking Alpha attention_{i,t}(z) | coefficient | | -0.010 | | | -0.015 |
| Seeking Alpha attention_{i,t}(z) | standard_error | | 0.010 | | | 0.010 |
| DJNW sentiment_{i,t}(z) | coefficient | 0.078*** | 0.067*** | 0.079*** | 0.082*** | 0.071*** |
| DJNW sentiment_{i,t}(z) | standard_error | 0.008 | 0.008 | 0.008 | 0.008 | 0.008 |
| DJNW attention_{i,t}(z) | coefficient | 0.012 | -0.019* | 0.008 | -0.008 | -0.012 |
| DJNW attention_{i,t}(z) | standard_error | 0.011 | 0.010 | 0.010 | 0.010 | 0.009 |
| 8-K report day_{i,t} | coefficient | 0.070 | 0.014 | 0.061 | 0.044 | 0.037 |
| 8-K report day_{i,t} | standard_error | 0.044 | 0.044 | 0.043 | 0.044 | 0.042 |
| EA day_{i,t} | coefficient | -0.547*** | -0.539*** | -0.547*** | -0.538*** | -0.566*** |
| EA day_{i,t} | standard_error | 0.091 | 0.091 | 0.091 | 0.091 | 0.091 |
| Volatility_{i,(t-5)→(t-1)} | coefficient | -0.045 | 0.022 | -0.009 | -0.099 | -0.114 |
| Volatility_{i,(t-5)→(t-1)} | standard_error | 0.375 | 0.378 | 0.377 | 0.375 | 0.373 |
| CAR_{i,(t-5)→(t-1)} | coefficient | -0.007*** | -0.007*** | -0.007*** | -0.008*** | -0.008*** |
| CAR_{i,(t-5)→(t-1)} | standard_error | 0.002 | 0.002 | 0.002 | 0.002 | 0.002 |
| CAR_{i,(t-30)→(t-6)} | coefficient | -0.001* | -0.001* | -0.001* | -0.001* | -0.001* |
| CAR_{i,(t-30)→(t-6)} | standard_error | 0.001 | 0.001 | 0.001 | 0.001 | 0.001 |
| Log Google ASVI_{i,t}(z) | coefficient | -0.053*** | -0.054*** | -0.050*** | -0.064*** | -0.065*** |
| Log Google ASVI_{i,t}(z) | standard_error | 0.017 | 0.017 | 0.017 | 0.017 | 0.017 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| Sentiment & Attention_{i,(t-1),...,(t-10)} | Y | Y | Y | Y | Y |
| Firm (i) FE | Y | Y | Y | Y | Y |
| Date (t) FE | Y | Y | Y | Y | Y |
| Outcome Mean | -0.048 | -0.048 | -0.048 | -0.048 | -0.048 |
| Outcome SD | 7.124 | 7.124 | 7.124 | 7.124 | 7.124 |
| Observations | 819,210 | 819,210 | 819,210 | 819,210 | 819,210 |
| R2 | 0.0320 | 0.0323 | 0.0321 | 0.0318 | 0.0319 |

**Note:** This table reports how next-day abnormal returns relate to social signals. The outcome is each security's abnormal return (AR) on day t+1 in percentage points. We control for DJNW standardized sentiment and attention, 8-K report date indicators, earnings announcement indicators, lagged return volatility (previous five trading days), lagged cumulative abnormal returns (previous five trading days and the 25 days before that), and Log Google ASVI. All regressions include ten lags (t-1 to t-10) of sentiment, and ten lags of attention. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors in parentheses are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level

#### 4.1.1 Mechanisms for return predictability

To better understand the mechanisms behind the informativeness of attention and sentiment for next-day returns, we estimate a specification using the PC1 of attention and sentiment as of day $t$ to predict cumulative abnormal returns for days $t+1$, $t+2$, ..., $t+20$. Figure 3 Panel (a) presents the estimated cumulative return coefficient on the sentiment PC1 (z); the coefficients for the middle and top terciles of attention are in Panel (b). These figures show that the positive cumulative return coefficients on sentiment are stable out to day $t+20$ and do not decline. Similarly, the coefficients on middle and high attention increase in magnitude for several days before flattening out by around day $t+15$. To provide context for these estimates, we run the same specification for day $t$ returns, and find a clear positive relation between both sentiment and attention and day $t$ returns (see columns 1-2 of Table 7).[^15] Putting these findings together, the negative attention estimates out to day $t+20$ reflect a gradual reversal of the positive return that occurs on day $t$ that is especially pronounced for high-attention days. Moreover, this reversal is only partial, adding up to about 1.5 percentage points relative to the day $t$ estimate of around 4 percentage points on high-attention days.

[^15]: Appendix Figure A3 presents the estimates for sentiment and attention by platform for same day return and retail trading imbalance.

### Figure 3: Informativeness of Social Signals for Cumulative Abnormal Returns

- **Panels:** (a) Sentiment signal; (b) Attention signal
- **Chart type:** Coefficient plots with 90% confidence intervals over horizons day 1 to day 20
- **Axes:** x-axis "Day" (1 to 20); y-axis "Coefficients (90% CI)". Panel (b) legend: Mid attention; High attention

**Note:** This figure plots the estimated coefficients (and 90% confidence intervals) on the first principal components (PC1s) of sentiment signal (z) in Panel (a) and on high-level and mid-level attention in Panel (b). High-level (or mid-level) attention equals 1 if the firm-day attention PC1 is above the 67th percentile (or between percentiles 33 and 67) within a year, and zero otherwise. The outcome is the cumulative abnormal return as of day t+1, t+2, ..., t+20, starting on day t+1. We estimate separate regressions for each horizon, and sentiment and attention coefficients are estimated in the same regression. (z) denotes a standardized variable (mean 0, standard deviation 1 using estimation sample statistics). Everything else follows Table 6 column 1.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

The above evidence also rules out some alternative interpretations. For example, the sentiment estimates exhibit no reversal, which is inconsistent with uninformed short-term buying pressure driving the positive day $t$ and $t+1$ returns. Instead, this is consistent with the interpretation that social media sentiment contains market-relevant information. Turning to attention, one hypothesis about the negative day $t+1$ coefficient is that attention on day $t$ reflects negative information that is not fully captured by sentiment. However, that is inconsistent with the positive relation between high attention and day $t$ returns. A natural way to interpret these dynamic results is that high attention days correspond to an over-reaction.[^16]

[^16]: We further examine the role of news as a mediator for our social media sentiment and attention estimates in Appendix Figure A4. To do this, we split days into "news days" (days the firm is covered by Dow Jones Newswire, days with an Earnings Announcement, or days with an 8K filing) and "no-news" days (days outside a +/-7 day window of any news day). We find that sentiment is informative in the presence of news, but not in its absence. By contrast, attention's over-reaction is greatest on no-news days, suggesting that the presence of news disciplines return overshooting.

In Table 7 columns 3-6, we present results on how day $t$ retail trading relates to the PC1s of sentiment and attention. We consider two measures of net retail buying: retail trade imbalance as in Boehmer et al. (2021) and the Robinhood user ratio as in Barber et al. (2022). For both we find that net buying on day $t$ is positively related to sentiment and attention. Coefficient estimates are especially large and statistically significant for attention, consistent with the interpretation that returns overshoot on high-attention days due to net buying by retail investors, and then gradually reverse. Further, in Appendix Figure A5, we present how day $t$ sentiment and attention relate to retail trading imbalance on days $t$, $t+1$, ..., $t+20$. Retail trading is only significantly related to day $t$ sentiment contemporaneously and for one or two days afterwards; the coefficient estimates on attention fall rapidly after day $t$.[^17] Thus, the dynamic relation between returns and the social signal is unlikely to be driven by persistent retail buying or selling pressure.

[^17]: In addition, the attention estimates are the wrong sign to explain the negative returns from day t+1 through t+20 via a buying pressure channel.

### Table 7: How Do Same-Day Returns and Retail Trading Relate to Social Signals?

- **Table type:** Regression
- **Unit of observation:** Firm-day
- **Estimator:** OLS with firm and date fixed effects
- **Standard errors:** In parentheses; double clustered by firm and by date
- **All columns include:** Controls (DJNW standardized sentiment and attention, 8-K report date indicators, earnings announcement indicators, lagged return volatility (previous five trading days), lagged cumulative abnormal returns (previous five trading days and the 25 days before that), and Log Google ASVI); ten lags (t-1 to t-10) of sentiment and ten lags of high and mid attention indicators. Columns 3-4 additionally control for lagged RT imbalance (previous five trading days and the 25 days before that); columns 5-6 for lagged RH user ratio (same lags)
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | dependent_variable |
|---:|---|
| 1 | $AR_{i,t}$ (%) |
| 2 | $AR_{i,t}$ (%) |
| 3 | RT imbalance_{i,t} (%) |
| 4 | RT imbalance_{i,t} (%) |
| 5 | RH user ratio_{i,t} (%) |
| 6 | RH user ratio_{i,t} (%) |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Sentiment PC1_{i,t}(z) | coefficient | 1.591*** | 1.498*** | 0.781*** | 0.655*** | 1.373 | 1.182 |
| Sentiment PC1_{i,t}(z) | standard_error | 0.036 | 0.033 | 0.046 | 0.043 | 1.025 | 1.055 |
| Attention PC1_{i,t}(z) | coefficient | 3.630*** | | 1.084*** | | 7.033*** | |
| Attention PC1_{i,t}(z) | standard_error | 0.734 | | 0.214 | | 1.701 | |
| Mid attention_{i,t} | coefficient | | 1.496*** | | 2.000*** | | 1.897*** |
| Mid attention_{i,t} | standard_error | | 0.058 | | 0.089 | | 0.531 |
| High attention_{i,t} | coefficient | | 4.049*** | | 3.969*** | | 5.976*** |
| High attention_{i,t} | standard_error | | 0.155 | | 0.143 | | 1.337 |
| DJNW sentiment_{i,t}(z) | coefficient | 0.425*** | 0.380*** | 0.135*** | 0.073*** | 0.031 | -0.029 |
| DJNW sentiment_{i,t}(z) | standard_error | 0.023 | 0.021 | 0.025 | 0.024 | 0.073 | 0.074 |
| DJNW attention_{i,t}(z) | coefficient | -0.272*** | 0.019 | -0.134*** | -0.107** | -0.303 | 0.303 |
| DJNW attention_{i,t}(z) | standard_error | 0.046 | 0.036 | 0.044 | 0.042 | 0.358 | 0.260 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Sentiment & Attention_{i,(t-1),...,(t-10)} | Y | Y | Y | Y | Y | Y |
| Controls | Y | Y | Y | Y | Y | Y |
| Firm (i) FE | Y | Y | Y | Y | Y | Y |
| Date (t) FE | Y | Y | Y | Y | Y | Y |
| Outcome Mean | 0.358 | 0.358 | -0.327 | -0.327 | 3.705 | 3.705 |
| Outcome SD | 9.190 | 9.190 | 23.173 | 23.173 | 178.715 | 178.715 |
| Observations | 819,706 | 819,706 | 810,652 | 810,652 | 171,479 | 171,479 |
| R2 | 0.0917 | 0.0779 | 0.0279 | 0.0300 | 0.1988 | 0.1989 |

**Note:** This table reports how same-day abnormal returns and retail trading relate to social signals. The outcome in columns 1-2, 3-4, and 5-6 is abnormal returns (AR) on day t in percentage points, retail trading (RT) imbalance on day t in percentage points, and Robinhood (RH) user ratio on day t in percentage points, respectively. RH user ratio on day t is calculated as (user number around 4pm on t / number around 4pm on t-1) - 1 following (Barber et al., 2022). High (or mid) attention equals 1 if the firm-day attention PC1 is above 67 percentile (or between 33 and 67 percentile) within a year, and zero otherwise. We control for DJNW standardized sentiment and attention, 8-K report date indicators, earnings announcement indicators, lagged return volatility (previous five trading days), lagged cumulative abnormal returns (previous five trading days and the 25 days before that), and Log Google ASVI. We additionally control for lagged RT imbalance (previous five trading days and the 25 days before that) in columns 3-4 and lagged RH user ratio (previous five trading days and the 25 days before that) in columns 5-6. All regressions include ten lags (t-1 to t-10) of sentiment, and ten lags of high and mid attention indicators. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors in parentheses are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level

#### 4.1.2 Heterogeneity by Size

In Table 1 Panel C, we show that the platforms focus on different parts of the firm size distribution, with StockTwits weighted towards small-cap firms, and Seeking Alpha and Twitter focusing on large-cap firms. Therefore, we examine whether the informativeness of the signal in columns 1-3 of Table 6 varies by firm size. Figure 4 plots the coefficients of sentiment and attention from regressions similar to the ones in Table 6, except run separately for small, mid-, and large-cap firms. In Panel (a) we find that sentiment for all three platforms positively predicts next-day abnormal returns, with sentiment on Twitter having the least predictive power across all firm size bins. The informativeness and the differences between platforms are larger for small-cap firms than for large-caps. In Panel (b) we show that, consistent with the results in Table 6, attention predicts lower next day returns, most evident for StockTwits for small- and mid-cap firms. To sum up, the informativeness of sentiment is higher for small-cap and mid-cap firms, whereas that of attention is concentrated mostly in small-cap and somewhat in mid-cap firms.[^18]

[^18]: Given that the distribution of returns is different for the three size subgroups, we normalize next-day returns within each size bin before estimation in Appendix Figure A6. Our conclusions are similar to the analysis in the main text. In addition, Appendix Figure A7 repeats the dynamic plot in Figure 3 in small-, mid-, and large-cap firm subsamples. These dynamics are similar to the overall results, with larger coefficient estimates for small-cap firms than for larger firms.

### Figure 4: How Do Next-Day Returns Relate to Platform-Specific Social Signals by Firm Size?

- **Panels:** (a) Informativeness of sentiment signal; (b) Informativeness of attention signal
- **Chart type:** Grouped bar charts of coefficient estimates with 90% confidence intervals
- **Axes:** x-axis groups: Small-cap, Mid-cap, Large-cap; bars per group (legend): StockTwits, Twitter, Seeking Alpha; y-axis "Coefficients (90% CI)"

**Note:** This figure plots the estimated coefficients (and 90% confidence intervals) on sentiment and attention signals (z) for StockTwits, Twitter, and Seeking Alpha for small-cap, mid-cap, and large-cap firms, separately. Firm size categories follow those in Table 1. The outcome is the abnormal return on day t+1. (z) denotes a standardized variable (mean 0, standard deviation 1 using estimation sample statistics by firm size). Everything else follows Table 6 columns 3-5.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

#### 4.1.3 Robustness

One downside to using the PC1 in column 4 of Table 6 is that the PCA is conducted over the entire sample period. This means that it would be impossible to take advantage of this information on date $t$, since it uses future data to create the signal. Therefore, in Table A6 we use a 1-year rolling PCA: for each year, we use the PCs constructed using the data from the previous calendar year. In column 1 we examine the PC1s of sentiment and attention, and the results are strikingly similar in magnitude and statistical significance to the corresponding coefficients in column 4 of Table 6. This implies that using data from the future to calculate PCs does not predict next-day returns any better than using data from the prior calendar year. In column 2, we add the second and the third sentiment PCs. Both positively predict next day returns with a smaller coefficient than PC1. Overall, the results in Table A6 suggest that our results in the main tables are not driven by a look-ahead bias.

*[Conversion note: this subsection twice refers to "column 4 of Table 6" when describing the PC1 specification; in the printed Table 6 the PC1 specification is column 1. Transcribed as printed.]*

The attention results in Table 6 may be influenced by our definition of social media attention in Equation 1. Therefore, in Table A7 we replicate the analysis using an alternate firm-day attention measure: the deviation from its median number of messages over the preceding 10 days. The loading on attention for StockTwits stays negative, albeit with slightly lower magnitude and statistical significance. Further, the table shows that attention from Seeking Alpha has a negative relation to next day's returns, especially when sentiment is negative. Overall, this table further supports the finding that attention is negatively related to next day returns.

A natural question in light of the GameStop short squeeze of January 2021 is how social media attention and sentiment from Reddit's WallStreetBets (WSB) relate to the signals we have examined so far. Our focus has been on the three platforms that have the longest time series of data, going back to 2012 (StockTwits, Twitter and Seeking Alpha). However, to understand the contribution of a new social platform, we collected all messages from Reddit WSB from Pushshift.io starting in 2018, when there is enough data to make this analysis meaningful, and using VADER (Hutto and Gilbert, 2014) to classify sentiment. We find that Reddit appears to be different from the major platforms in its relation to next day returns (see Appendix Table A8). WSB attention is positively related to next-day returns, while WSB sentiment is unrelated. Although the sample time window is more limited (2018-2021), the signals for the other three platforms reflect the same pattern we have seen throughout the paper: sentiment is positively related to next-day returns, but attention is negatively related. These contrasting results between WSB and other platforms may reflect differences in platform features or in user populations. We examine these mechanisms in the next section focusing on the three main platforms.

### 4.2 Information from market events

To understand what could be driving the cross-platform differences in the informativeness of sentiment and attention, we study two market events that affected platform-specific features or user populations, thereby potentially changing the information impounded in the social signal. First, we study changes in the informativeness of the social signal when StockTwits substantially increased its character limit per message. Second, we examine how the informativeness of sentiment and attention changed around the January 2021 GME phenomenon.

#### 4.2.1 StockTwits character limit change

On May 8, 2019, StockTwits changed the character limit on its posts from 140 characters to 1,000. We explore whether this change affected the informativeness of the signal from StockTwits, in comparison to the plausibly unaffected signals from Twitter and Seeking Alpha. Communication theory suggests that changes to a medium's features may have large effects on the information it communicates (McLuhan, 1975). To focus on the StockTwits format change, we analyze the period from one year before to one year after May 8, 2019.

Figure 5 Panel (a) plots the distribution of the number of characters per message across this event window, and Panel (b) firm-day averages of the number of characters per message, which ensures the figure is not dominated by messages about the most popular firms. Consistent with the character limit increase only affecting the content of longer messages, whose authors most likely were writing at the character limit, we see that only messages in the top quartile of characters per message become longer after the change. Similarly, the impact of the character limit expansion is also larger at the top of the distribution for the firm-day averages (Panel b).

### Figure 5: Monthly Quartiles of Number of Message Length

- **Panels:** (a) Number of characters per message; (b) Firm-day level average number of characters per message
- **Chart type:** Monthly time-series lines of distribution quantiles, 2017m1 to late 2021
- **Axes:** x-axis: months (2017m1-2021m+); y-axis "Characters per message". Legend: P25, P50, P75, P90. A vertical line marks May 8, 2019

**Note:** This figure plots monthly quartiles of number of characters per message (panel a) and monthly quartiles of the firm-day level average number of characters per message (panel b). The vertical line denotes May 8, 2019, the date when StockTwits increased its character limit from 140 characters to 1,000.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

To focus more cleanly on the impact of the StockTwits character limit increase, we present a set of platform-specific regressions of the form:

$$
\begin{aligned}
Abnormal\ Returns_{i,t+1} = \ & \beta_1 Attention_{i,t} + \beta_2 Sentiment_{i,t} + \beta_3 Sentiment_{i,t} \times Post_t \\
& + \beta_4 Attention_{i,t} \times Post_t + X_{i,t} \times \Gamma + \alpha_t + \alpha_i + \epsilon_{i,t}
\end{aligned} \tag{4}
$$

This specification includes controls and fixed effects as in Equation 3 for next-day returns. Relative to Equation 3, the novel terms are sentiment and attention interacted with a $Post_t$ indicator for the date being after May 8, 2019. The coefficients of interest are these interactions with $Post_t$, which capture changes in the informativeness of the social signal around the character limit increase.

Table 8 reports the results from estimating this specification separately for StockTwits, Twitter, and Seeking Alpha. Consistent with StockTwits sentiment becoming more informative after the character limit increase, we find that the coefficient on sentiment for next-day returns increases by 7 bps (column 1). This estimate is nearly twice the size of the main effect of sentiment (3 bps, row 3 of the table). In column 2 we focus on StockTwits signals for stocks with an average character length in the top quartile on a day, and find an even stronger increase in informativeness of nearly 14 bps. By contrast, we see no change for Twitter or Seeking Alpha in columns 3 and 4, indicating that the change in informativeness is specific to StockTwits.

### Table 8: How Did the Informativeness of Social Signals Change around the StockTwits Character Limit Increase?

- **Table type:** Regression
- **Unit of observation:** Firm-day
- **Dependent variable:** $AR_{i,t+1}$ (%) — abnormal returns on day t+1 in percentage points
- **Sample:** Firm-day observations with at least 10 messages on StockTwits between May 8, 2018 and May 7, 2020
- **$Post_t$:** one if a day is on or after May 8, 2019
- **Estimator:** OLS with firm and date fixed effects
- **Controls (all columns):** 8-K report date indicators, earnings announcement indicators, lagged return volatility (previous five trading days), lagged cumulative abnormal returns (previous five trading days and the 25 days before that), and Log Google ASVI
- **Standard errors:** In parentheses; double clustered by firm and by date
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | signal_source |
|---:|---|
| 1 | StockTwits |
| 2 | StockTwits, stocks with top quartile daily average character length per message |
| 3 | Twitter |
| 4 | Seeking Alpha |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 |
|---|---|---:|---:|---:|---:|
| Post_t × Sentiment_{i,t}(z) | coefficient | 0.070** | 0.138** | -0.010 | -0.007 |
| Post_t × Sentiment_{i,t}(z) | standard_error | 0.034 | 0.055 | 0.043 | 0.034 |
| Post_t × Attention_{i,t}(z) | coefficient | 0.165* | -0.269 | -0.005 | -0.016 |
| Post_t × Attention_{i,t}(z) | standard_error | 0.088 | 0.226 | 0.026 | 0.031 |
| Sentiment_{i,t}(z) | coefficient | 0.031 | 0.004 | 0.000 | 0.078*** |
| Sentiment_{i,t}(z) | standard_error | 0.024 | 0.037 | 0.019 | 0.024 |
| Attention_{i,t}(z) | coefficient | -0.382*** | -0.290 | -0.032 | -0.016 |
| Attention_{i,t}(z) | standard_error | 0.117 | 0.200 | 0.025 | 0.022 |
| DJNW sentiment_{i,t}(z) | coefficient | 0.098*** | 0.091*** | 0.101*** | 0.087*** |
| DJNW sentiment_{i,t}(z) | standard_error | 0.016 | 0.026 | 0.016 | 0.016 |
| DJNW attention_{i,t}(z) | coefficient | 0.019 | -0.008 | -0.005 | -0.011 |
| DJNW attention_{i,t}(z) | standard_error | 0.025 | 0.053 | 0.025 | 0.022 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 |
|---|---:|---:|---:|---:|
| Controls | Y | Y | Y | Y |
| Firm (i) FE | Y | Y | Y | Y |
| Date (t) FE | Y | Y | Y | Y |
| Outcome Mean | -0.093 | 0.004 | -0.093 | -0.093 |
| Outcome SD | 7.819 | 6.455 | 7.819 | 7.819 |
| Observations | 215,319 | 53,659 | 215,319 | 215,319 |
| R2 | 0.027 | 0.065 | 0.026 | 0.026 |

**Note:** This table compares how social signals from different platforms changed their predictive power for next-day returns around the character limit increase on StockTwits. The outcome is abnormal returns (AR) on day t+1 in percentage points. Post_t is one if a day is on or after May 8, 2019. Social signals in columns 1-4 are StockTwits signals, StockTwits signals for stocks with top quartile daily average character length per message, Twitter signals, and Seeking Alpha signals, respectively. Controls are 8-K report date indicators, earnings announcement indicators, lagged return volatility (previous five trading days), lagged cumulative abnormal returns (previous five trading days and the 25 days before that), and Log Google ASVI. The sample consists of firm-day observations with at least 10 messages on StockTwits between May 8,2018 and May 7, 2020. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors in parentheses are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level

A potential mechanism through which posts become more informative after the character limit increase is a change in the composition of the messages. Specifically, it could be the case that more sophisticated investors take advantage of the change to write longer messages, either because the salience of the feature change induces some of them to modify their influence strategy, or because longer posts are more persuasive than shorter ones. This is indeed what we find in Table A9: Professional investors write longer messages before the change, and increase their message length by more after it. In Table A10 we find that Professional investors' sentiment has a stronger predictive power for next day's returns than Novices and Influencers, while the attention of each user type predicts next day returns with a negative sign. Taken together, the increased informativeness of sentiment from longer messages after the character-limit change seems to be driven by Professional investors taking disproportionate advantage of the new feature.

To more formally estimate the impact of the character limit increase, we perform analysis akin to a difference-in-differences design in which we define "treated" observations as firms with an average character length in the top quartile on any given day, and "control" as those in the bottom quartile. Using this definition, we extend the specification in Equation 4 to one that also contains interactions with the $Treated_i$ indicator and report estimates in Appendix Table A11. The estimate on the triple interaction term $Post_t \times Treated_i \times Sentiment_{it}(z)$ shows that, after the character limit increase, sentiment becomes more informative for next-day returns, especially for stocks most affected by the increase. Specifically, a standard deviation increase in sentiment predicts an 17.8 bps greater return for stocks most discussed by long vs. short messages on StockTwits. By contrast, attention's informativeness falls after the character limit change, although the coefficient on the triple interaction is only weakly statistically significant.

Figure 6 presents quarterly estimates of the triple interaction around the character limit increase. This plot indicates that the effect is not driven by any obvious trends in informativeness of sentiment over time.[^19]

[^19]: Appendix Figure A8 extends the sample window relative to Figure 6 and plots coefficient estimates on sentiment for stocks most discussed by long messages on StockTwits at the semester level. We see no pre-trend in the informativeness over this extended period, and the heightened informativeness persists until the beginning of the pandemic (first semester of 2020).

### Figure 6: How Did the Informativeness of the Sentiment Signal for Next-day Returns Change Around the StockTwits Character Limit Increase?

- **Chart type:** Event-study coefficient plot with 90% confidence intervals at quarterly event time
- **Axes:** x-axis "Quarter from May 8, 2019" (-4 to 3); y-axis "Difference (90% CI)". A vertical dashed line separates pre and post periods

**Note:** This figure provides event study estimates (and 90% confidence intervals) of how the StockTwits sentiment signal relates to next day abnormal returns around the StockTwits character limit increase. The treated group is stocks whose daily average number of characters per message is in the top quartile; the comparison group is stocks in the bottom quartile. Event time 0 represents the three months following May 8, 2019 – the date of the character limit change. The omitted period is quarter -1. The sample consists of firm-day observations with at least 10 messages on StockTwits between May 8, 2018 and May 8, 2020. Everything else follows Table A11.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

An alternative explanation for the increased informativeness of the sentiment signal is that once messages become longer, natural language processing (NLP) algorithms are better able to classify sentiment. In Table A12 columns 1 and 2 we focus only on the subset of StockTwits messages that have user-labeled sentiment (as described in Section 2), and reproduce the analysis in Table 8. Reassuringly, the coefficients are similar in sign and magnitude, supporting the view that the increased informativeness after the character limit change is not driven solely by a better NLP classification of longer messages. However, because the standard errors increase due to the reduced sample size, the coefficients are not statistically significant.

#### 4.2.2 Changes around the GameStop short squeeze

In this section, we analyze a second market event that likely influenced the informativeness of social media signals: the GameStop Short Squeeze event (GME event) in late January 2021, interacted with the large influx of new retail investors in US equity markets that occurred in 2020. Bradley et al. (2021) studies a class of posts on Reddit's WallStreetBets (WSB) called "due diligence reports" around this event, finding that these reports were informative for future returns before the event but were much less informative afterwards. We perform a similar analysis for signals from StockTwits, Twitter, and Seeking Alpha around the GME event using the first PCs of attention and sentiment constructed from the three platforms in Section 3.1.

We look at 11 months before and after the GME event since we have data until the end of 2021 (only 11 months after January 2021). We exclude January 2021 to have a cleaner pre/post comparison. The specification follows Equation (4). Table 9 presents the findings on the informativeness of the social signal for next-day returns. We find that next-day returns' sensitivity to sentiment drops substantially following the GME event. Specifically, a standard deviation increase in sentiment (the first PC) is associated with a 12.5 bps lower return after the GME event (column 1), completely offsetting the pre-GME informativeness of social media sentiment (11.1 bps). In column 2, we additionally include the second and third PCs of sentiment (capturing cross-platform differences in sentiment), but the coefficients related to sentiment's first PC are virtually identical.

To better understand the mechanism behind this decline in informativeness, we use tweet-level data from StockTwits. Most social media platforms, including StockTwits, saw an influx of new users and increase in posts starting in 2020, likely the result of stay-at-home orders together with the introduction of no-fee trading at many brokerages in late 2019. We split the sample into tweets by those who joined StockTwits prior to January 1, 2020 (established or old users) and tweets by users who joined more recently (new users). From each subsample of tweets, we construct separate measures of attention and sentiment.

New users display a stronger interest in "short squeeze" strategies after the GME event. Figure 7 documents a persistent uptick in mentions of short squeezes on StockTwits from an average of roughly 6,200 mentions per month in the year before the GME event to an average of nearly 13,000 afterwards. This spike in posts mentioning "short squeeze" is primarily driven by new users with an increase from around 4,300 to over 17,000 posts per month; in contrast, short squeeze posts from established users only see a moderate uptick (from 8,040 to 8,180 per month).

*[Conversion note: the per-group figures in this paragraph (new users from ~4,300 to over 17,000; established users from 8,040 to 8,180) are transcribed exactly as printed; readers may notice they do not aggregate neatly to the overall averages quoted in the same paragraph.]*

### Figure 7: Mentions of "Short Squeeze" on StockTwits around the GameStop Event, Old vs. New Users

- **Chart type:** Monthly time-series of mentions, January 2020 to November 2021, two series
- **Series (legend):** New users (blue diamonds); old users (black triangles). Dashed horizontal lines denote sub-period averages for each user group. A vertical dotted line marks January 2021
- **Axes:** x-axis: months (2020m1-2021m11); y-axis: mentions (axis scale 0 to 30)

**Note:** This figure presents evidence on the changing narratives of StockTwits users in the months around the GME short squeeze event. Specifically, the figure plots monthly mentions of "short squeeze" from new users (blue diamonds) and old users (black triangles) around the event. Old users are those who joined StockTwits before January 2020 and new users are those joined in or after January 2020. Dashed horizontal lines denote sub-period averages for each user group.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

In Table 9 column 3, consistent with new users' stronger interest in "short squeeze," we find that the informativeness of the new users' signal for next-day returns declines by 10.3 bps for a standard deviation increase in sentiment after the GME event, again fully offsetting the pre-GME effect of sentiment. Importantly however, the informativeness of the established users' signal does not change (column 4).[^20]

[^20]: While the coefficient on sentiment in column 4 is not statistically significant, we show in Appendix Figure A9 that it does not represent a meaningful departure from prior years' coefficient estimates, which are positive and statistically significant.

An alternative explanation for the deceased informativeness is that new users might be using non-word tokens, like emojis, in a way that could reduce the effectiveness of NLP sentiment classification. In Table A12 columns 3 and 4, we repeat the analysis using only self-labeled sentiment. Reassuringly, the coefficients are similar in magnitude and statistical significance.

*[Conversion note: "deceased informativeness" is transcribed as printed; presumably "decreased informativeness".]*

Finally, as a complement to the sample split-based evidence, we perform analysis akin to a difference-in-differences design in which we define "treated" observations as posts by new users, and "control" as those made by existing (old) users. This analysis contrasts the informativeness of the social signal for new users vs. established users, before vs. after the event. We report the results in Appendix Table A13. The estimate on the sentiment triple interaction implies that, after the GME event, sentiment becomes less informative for next-day returns for new users – relative to old users – although the coefficient is only significant at the 10% level.

Overall, these findings from the GME event highlight how the arrival of new users can influence the informativeness of the social media signal.

### Table 9: How Did the Informativeness of Social Signals Change around the GameStop Event?

- **Table type:** Regression
- **Unit of observation:** Firm-day
- **Dependent variable:** $AR_{i,t+1}$ (%) — abnormal returns on day t+1 in percentage points
- **Sample:** Firm-day observations with at least 10 messages on StockTwits between February 1, 2020 and December 31, 2021, excluding January 2021
- **$Post_t$:** one for days on or after February 1, 2021
- **Estimator:** OLS with firm and date fixed effects
- **Controls (all columns):** 8-K report day indicators, earnings announcement day indicators, lagged return volatility (previous five trading days), lagged cumulative abnormal returns (previous five trading days and the 25 days before that), and Log Google ASVI
- **Standard errors:** Double clustered by firm and by date
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | signal_source |
|---:|---|
| 1 | PC signal: principal components (z) of attention or sentiment signals from all StockTwits subgroups, StockTwits self-labelled messages, Twitter, and Seeking Alpha |
| 2 | PC signal (as model 1, adding sentiment PC2 and PC3) |
| 3 | StockTwits new: messages from users who joined StockTwits in or after 2020 |
| 4 | StockTwits old: messages from users who joined StockTwits before 2020 |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 |
|---|---|---:|---:|---:|---:|
| Post_t × Sentiment_{i,t}(z) | coefficient | -0.125*** | -0.124*** | -0.103** | 0.002 |
| Post_t × Sentiment_{i,t}(z) | standard_error | 0.048 | 0.048 | 0.043 | 0.034 |
| Post_t × Attention_{i,t}(z) | coefficient | 0.001 | -0.001 | 0.015 | -0.019 |
| Post_t × Attention_{i,t}(z) | standard_error | 0.093 | 0.094 | 0.107 | 0.090 |
| Sentiment_{i,t}(z) | coefficient | 0.111*** | 0.111*** | 0.101** | 0.038 |
| Sentiment_{i,t}(z) | standard_error | 0.042 | 0.042 | 0.039 | 0.028 |
| Attention_{i,t}(z) | coefficient | -0.071 | -0.070 | -0.065 | -0.065 |
| Attention_{i,t}(z) | standard_error | 0.056 | 0.057 | 0.065 | 0.054 |
| Post_t × Sentiment PC2_{i,t}(z) | coefficient | | 0.028 | | |
| Post_t × Sentiment PC2_{i,t}(z) | standard_error | | 0.033 | | |
| Post_t × Sentiment PC3_{i,t}(z) | coefficient | | 0.014 | | |
| Post_t × Sentiment PC3_{i,t}(z) | standard_error | | 0.030 | | |
| Sentiment PC2_{i,t}(z) | coefficient | | -0.004 | | |
| Sentiment PC2_{i,t}(z) | standard_error | | 0.026 | | |
| Sentiment PC3_{i,t}(z) | coefficient | | 0.022 | | |
| Sentiment PC3_{i,t}(z) | standard_error | | 0.026 | | |
| DJNW sentiment_{i,t}(z) | coefficient | 0.086*** | 0.081*** | 0.088*** | 0.087*** |
| DJNW sentiment_{i,t}(z) | standard_error | 0.016 | 0.016 | 0.017 | 0.016 |
| DJNW attention_{i,t}(z) | coefficient | -0.058** | -0.060** | -0.064** | -0.060** |
| DJNW attention_{i,t}(z) | standard_error | 0.029 | 0.029 | 0.029 | 0.029 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 |
|---|---:|---:|---:|---:|
| Controls | Y | Y | Y | Y |
| Firm (i) FE | Y | Y | Y | Y |
| Date (t) FE | Y | Y | Y | Y |
| Outcome Mean | -0.005 | -0.005 | -0.005 | -0.005 |
| Outcome SD | 7.864 | 7.864 | 7.864 | 7.864 |
| Observations | 289,092 | 289,092 | 289,092 | 289,092 |
| R2 | 0.049 | 0.049 | 0.049 | 0.049 |

**Note:** This table compares how social signals from different platforms and/or user types changed their predictive power for next-day abnormal returns (AR) around the GameStop event on January 28, 2021. The outcome is abnormal returns (AR) on day t+1 in percentage points. Post_t is one for days on or after February 1, 2021. Social signals in columns 1-2 are based on principal components (z) of attention or sentiment signals from all StockTwits subgroups, StockTwits self-labelled messages, Twitter, and Seeking Alpha (PC signal); column 3 messages from users who joined StockTwits in or after 2020 (StockTwits new); and column 4 messages from users who joined StockTwits before 2020 (StockTwits old), respectively. Controls are 8-K report day indicators, earnings announcement day indicators, lagged return volatility (previous five trading days), lagged return volatility (previous five trading days), lagged cumulative abnormal returns (previous five trading days and the 25 days before that), and Log Google ASVI. The sample consists of firm-day observations with at least 10 messages on StockTwits between February 1, 2020 and December 31, 2021, excluding January 2021. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level *[Conversion note: "lagged return volatility (previous five trading days)" appears twice in the original note; transcribed as printed.]*

## 5. Conclusion

In this paper, we explore the similarities and differences in the social signals generated from StockTwits, Twitter, and Seeking Alpha. Our analysis reveals differences across social investing platforms that are much more pronounced for sentiment than for attention. We attribute these differences to differences in types of investors (e.g., influencers, professionals, and novices) and differences across platform features (e.g., character limits on posts).

Investor social media has increased steadily in popularity over the past two decades, and has grown rapidly in recent years. Online investment forums attract hundreds of thousands of daily users who intensively discuss individual securities in real time. Given the differences across platforms, particularly new entrants that rely on other kinds of media (e.g., Discord and TikTok), it is natural to expect the informativeness of future social signals and retail trading to evolve as well (Chang and Peng, 2021, Pyun, 2021). Will these new technologies enhance or weaken the information environment? We expect ample opportunities for future work to examine the consequences of these emerging technologies.

## References

Akçay, E. and Hirshleifer, D. (2021). Social finance as cultural evolution, transmission bias, and market dynamics. *Proceedings of the National Academy of Sciences*, 118(26):e2015568118.

Antweiler, W. and Frank, M. Z. (2004). Is all that talk just noise? the information content of internet stock message boards. *Journal of Finance*, 59(3):1259–1294.

Bailey, M., Cao, R., Kuchler, T., and Stroebel, J. (2018a). The economic effects of social networks: Evidence from the housing market. *Journal of Political Economy*, 126(6):2224–2276.

Bailey, M., Cao, R., Kuchler, T., Stroebel, J., and Wong, A. (2018b). Social connectedness: Measurement, determinants, and effects. *Journal of Economic Perspectives*, 32(3):259–80.

Barber, B. M., Huang, X., Odean, T., and Schwarz, C. (2022). Attention induced trading and returns: Evidence from robinhood users. *Journal of Finance*, forthcoming.

Barber, B. M. and Odean, T. (2001). Boys will be boys: Gender, overconfidence, and common stock investment. *Quarterly Journal of Economics*, 116(1):261–292.

Barber, B. M. and Odean, T. (2008). All that glitters: The effect of attention and news on the buying behavior of individual and institutional investors. *Review of Financial Studies*, 21(2):785–818.

Ben-Rephael, A., Da, Z., and Israelsen, R. D. (2017). It depends on where you search: A comparison of institutional and retail attention. *Review of Financial Studies*, 30(9):3009–3047.

Bianchi, F., Gómez-Cram, R., Kind, T., and Kung, H. (2023). Threats to central bank independence: High-frequency identification with twitter. *Journal of Monetary Economics*, 135:37–54.

Bianchi, F., Gómez-Cram, R., and Kung, H. (2024). Using social media to identify the effects of congressional viewpoints on asset prices. *Review of Financial Studies*.

Blankespoor, E., Miller, G. S., and White, H. D. (2014). The role of dissemination in market liquidity: Evidence from firms' use of Twitter. *The Accounting Review*, 89(1):79–112.

Boehmer, E., Jones, C. M., Zhang, X., and Zhang, X. (2021). Tracking retail investor activity. *Journal of Finance*, 76(5):2249–2305.

Bradley, D., Hanousek Jr, J., Jame, R., and Xiao, Z. (2021). Place your bets? the market consequences of investment research on reddit's wallstreetbets. Working paper.

Chang, R. and Peng, L. (2021). Tiktok sentiment, emotional contagion, and global stock returns. Working paper.

Chen, H., De, P., Hu, Y. J., and Hwang, B.-H. (2014). Wisdom of crowds: The value of stock opinions transmitted through social media. *Review of Financial Studies*, 27(5):1367–1403.

Chen, H. and Hwang, B.-H. (2022). Listening in on investors' thoughts and conversations. *Journal of Financial Economics*, 145(2):426–444.

Chen, H., Hwang, B.-H., and Liu, B. (2019). The emergence of 'social executives' and its consequences for financial markets. Working paper.

Cookson, J. A., Engelberg, J., and Mullins, W. (2022a). Echo Chambers. *Review of Financial Studies*.

Cookson, J. A., Engelberg, J. E., and Mullins, W. (2020). Does partisanship shape investor beliefs? Evidence from the COVID-19 pandemic. *Review of Asset Pricing Studies*, 10(4):863–893.

Cookson, J. A., Fox, C., Gil-Bazo, J., Imbet, J. F., and Schiller, C. (2023). Social media as a bank run catalyst. Working paper.

Cookson, J. A. and Niessner, M. (2020). Why don't we agree? Evidence from a social network of investors. *Journal of Finance*, 75(1):173–228.

Cookson, J. A., Niessner, M., and Schiller, C. (2022b). Can social media inform corporate decisions? Evidence from merger withdrawals. Working paper.

Da, Z., Engelberg, J., and Gao, P. (2011). In search of attention. *Journal of Finance*, 66(5):1461–1499.

Da, Z., Hua, J., Hung, C.-C., and Peng, L. (2022). Market returns and a tale of two types of attention. Working paper.

Da, Z. and Huang, X. (2020). Harnessing the wisdom of crowds. *Management Science*, 66(5):1847–1867.

Da, Z., Huang, X., and Jin, L. J. (2021). Extrapolative beliefs in the cross-section: What can we learn from the crowds? *Journal of Financial Economics*, 140(1):175–196.

Daniel, K. and Hirshleifer, D. (2015). Overconfident investors, predictable returns, and excessive trading. *Journal of Economic Perspectives*, 29(4):61–88.

Daniel, K., Hirshleifer, D., and Subrahmanyam, A. (1998). Investor psychology and security market under-and overreactions. *Journal of Finance*, 53(6):1839–1885.

Dim, C. (2020). Should retail investors listen to social media analysts? Evidence from text-implied beliefs. Working paper.

Eaton, G. W., Green, T. C., Roseman, B. S., and Wu, Y. (2022). Retail trader sophistication and stock market quality: Evidence from brokerage outages. *Journal of Financial Economics*, 146(2):502–528.

Farrell, M., Green, T. C., Jame, R., and Markov, S. (2022). The democratization of investment research and the informativeness of retail investor trading. *Journal of Financial Economics*, 145(2):616–641.

Forbes (2021). Americans spent on average more than 1,300 hours on social media last year. *Forbes*. https://www.forbes.com/sites/petersuciu/2021/06/24/americans-spent-more-than-1300-hours-on-social-media/?sh=352920522547 (accessed August 29, 2022).

Garcia, D. (2013). Sentiment during recessions. *Journal of Finance*, 68(3):1267–1300.

Gargano, A. and Rossi, A. G. (2018). Does it pay to pay attention? *Review of Financial Studies*, 31(12):4595–4649.

Giannini, R., Irvine, P., and Shu, T. (2018). Nonlocal disadvantage: An examination of social media sentiment. *Review of Asset Pricing Studies*, 8(2):293–336.

Giannini, R., Irvine, P., and Shu, T. (2019). The convergence and divergence of investors' opinions around earnings news: Evidence from a social network. *Journal of Financial Markets*, 42:94–120.

Gu, C. and Kurov, A. (2020). Informational role of social media: Evidence from twitter sentiment. *Journal of Banking & Finance*, 121:105969.

Heimer, R. Z. (2016). Peer pressure: Social interaction and the disposition effect. *Review of Financial Studies*, 29(11):3177–3209.

Hirshleifer, D. (2020). Presidential address: Social transmission bias in economics and finance. *Journal of Finance*, 75(4):1779–1831.

Hirshleifer, D., Peng, L., and Wang, Q. (2023). News diffusion in social networks and stock market reactions. Technical report.

Hutto, C. and Gilbert, E. (2014). Vader: A parsimonious rule-based model for sentiment analysis of social media text. In *Proceedings of the international AAAI conference on web and social media*, volume 8, pages 216–225.

Irvine, P. J., Shen, S., and Shu, T. (2021). Aggregate attention. Working paper.

Jame, R., Johnston, R., Markov, S., and Wolfe, M. C. (2016). The value of crowdsourced earnings forecasts. *Journal of Accounting Research*, 54(4):1077–1110.

Kogan, S., Moskowitz, T. J., and Niessner, M. (2022). Social Media and Financial News Manipulation. *Review of Finance*, 27(4):1229–1268.

Kuchler, T. and Stroebel, J. (2021). Social finance. *Annual Review of Financial Economics*, 13:37–55.

Levy, R. (2021). Social media, news consumption, and polarization: Evidence from a field experiment. *American Economic Review*, 111(3):831–870.

Liu, H., Peng, C., Xiong, W. A., and Xiong, W. (2020). Resolving the excessive trading puzzle: An integrated approach based on surveys and transactions. NBER working paper.

Lu, R. and Sheng, S. Y. (2022). How racial animus forms and spreads: Evidence from the Coronavirus pandemic. *Journal of Economic Behavior & Organization*, 200:82–98.

McLuhan, M. (1975). *Understanding media: The extensions of man*. Routledge & Kegan Paul.

Müller, K. and Schwarz, C. (2022). From hashtag to hate crime: Twitter and anti-minority sentiment. *American Economic Journal: Applied Economics*.

Niessner, M. (2015). Strategic disclosure timing and insider trading. Working paper.

Pedersen, L. H. (2022). Game on: Social networks and markets. *Journal of Financial Economics*.

Pew (2021). News use across social media platforms in 2020. Pew Research Center.

Pyun, C. (2021). Social media group investing. Working paper.

Renault, T. (2017). Intraday online investor sentiment and return patterns in the us stock market. *Journal of Banking & Finance*, 84:25–40.

Sicherman, N., Loewenstein, G., Seppi, D. J., and Utkus, S. P. (2016). Financial attention. *Review of Financial Studies*, 29(4):863–897.

Tetlock, P. C. (2007). Giving content to investor sentiment: The role of media in the stock market. *Journal of Finance*, 62(3):1139–1168.

Thompson, S. B. (2011). Simple formulas for standard errors that cluster by both firm and time. *Journal of Financial Economics*, 99(1):1–10.

## Online Appendix

*The Social Signal* — J. Anthony Cookson, Runjing Lu, William Mullins, and Marina Niessner

### Figure A1: Monthly Number of Messages and Sentiment Signal Across Platforms

- **Panels:** (a) StockTwits number of messages; (b) Twitter number of messages; (c) Seeking Alpha number of messages; (d) Sentiment signal by platform
- **Chart type:** Monthly time series, 2012m1 to 2022m1
- **Axes:** Panels (a)-(c): y-axis "Number of messages (k)"; Panel (d): y-axis "Average sentiment", legend: StockTwits (z), Twitter (z), Seeking Alpha (z)

**Note:** This figure plots the monthly number of messages on StockTwits in Panel (a), Twitter in Panel (b), and Seeking Alpha in Panel (c), as well as monthly average standardized platform-specific sentiment signal in Panel (d). Values are in thousands of messages in Panels (a)-(c) and range between -1 and +1 in Panel (d).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A2: Partial Auto-correlation Function for Social Signals

- **Chart type:** Partial autocorrelation function plot, lags 0 to 20, with 90% confidence intervals
- **Series (legend):** ST sentiment, TW sentiment, SA sentiment (solid lines); ST attention, TW attention, SA attention (dashed lines)
- **Axes:** x-axis "Lag" (0 to 20); y-axis "Partial autocorrelation (90% CI)"

**Note:** This figure reports the partial auto-correlation for attention and sentiment signals on StockTwits (ST), Twitter (TW), and Seeking Alpha (SA).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A3: How Do Same-Day Returns and Retail Trading Imbalance Relate to Social Signals?

- **Panels:** (a) Informativeness of social signals for $AR_{i,t}$; (b) Informativeness of social signals for RT imbalance_{i,t}
- **Chart type:** Grouped bar charts of coefficient estimates with 90% confidence intervals
- **Axes:** x-axis groups: Sentiment, Attention; bars per group (legend): StockTwits, Twitter, Seeking Alpha, PC1; y-axis "Coefficients (90% CI)"

**Note:** This figure plots the estimated coefficients (and 90% confidence intervals) on sentiment and attention signals (z) for StockTwits, Twitter, Seeking Alpha, and PC1 across the three platforms, separately. The outcome is the abnormal return on day t (panel a) and retail trading imbalance on day t (panel b). (z) denotes a standardized variable (mean 0, standard deviation 1 using estimation sample statistics by firm size). Everything else follows Table 7 columns 3-5.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A4: Informativeness of Social Signals for Cumulative Abnormal Returns, News vs. No News

- **Panels:** (a) Sentiment signal, no-news days; (b) Sentiment signal, news days; (c) Attention signal, no-news days; (d) Attention signal, news days
- **Chart type:** Coefficient plots with 90% confidence intervals over horizons day 1 to day 20. Panels (c)-(d) legend: Mid attention; High attention
- **Axes:** x-axis "Day" (1 to 20); y-axis "Coefficients (90% CI)"

**Note:** This figure repeats Figure 3 by presence of firm news. "News days" refers to firm-day observations that are covered by Dow Jones News wire, with an Earnings Announcement, or with an 8K filing; "no-news days" refers to firm-day observations not within a +/-7 day window of any news days. We estimate separate regressions for each horizon, and sentiment and attention coefficients are estimated in the same regression. Everything else follows Figure 3.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A5: Informativeness of Social Signals for Retail Trading

- **Panels:** (a) RT imbalance, sentiment signal; (b) Robinhood user ratio, sentiment signal; (c) RT imbalance, attention signal; (d) Robinhood user ratio, attention signal
- **Chart type:** Coefficient plots with 90% confidence intervals over horizons day 0 to day 20. Panels (c)-(d) legend: Mid attention; High attention
- **Axes:** x-axis "Day" (0, 1, 5, 10, 15, 20); y-axis "Coefficients (90% CI)"

**Note:** This figure plots the estimated coefficients (and 90% confidence intervals) on sentiment PC1, high-level attention, and mid-level attention. High-level (or mid-level) attention equals 1 if the firm-day attention PC1 is above the 67th percentile (or between 33rd and 67th percentiles) within a year, and zero otherwise. The outcomes are retail trading (RT) imbalance and the Robinhood user ratio as of day t+1, day t+2, ..., day t+20. We estimate separate regressions for each horizon, and sentiment and attention coefficients are estimated in the same regression. Everything else follows Table 7 columns 4 and 6.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A6: How Do Next-Day Returns Relate to Platform-Specific Social Signals by Firm Size? Returns Standardized within Firm Size Group

- **Panels:** (a) Informativeness of the sentiment signal; (b) Informativeness of the attention signal
- **Chart type:** Grouped bar charts of coefficient estimates with 90% confidence intervals
- **Axes:** x-axis groups: Small-cap, Mid-cap, Large-cap; bars per group (legend): StockTwits, Twitter, Seeking Alpha; y-axis "Coefficients (90% CI)"

**Note:** This figure repeats Figure 4 while changing the outcome to the abnormal return on day t+1, standardized within each firm size sub-sample to have mean zero and variance of 1. Everything else follows Figure 4.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A7: Informativeness of Social Signals for Cumulative Abnormal Returns by Firm Size

- **Panels:** (a) Sentiment signal, small-cap; (b) Sentiment signal, mid-cap; (c) Sentiment signal, large-cap; (d) Attention signal, small-cap; (e) Attention signal, mid-cap; (f) Attention signal, large-cap
- **Chart type:** Coefficient plots with 90% confidence intervals over horizons day 1 to day 20. Panels (d)-(f) legend: Mid attention; High attention
- **Axes:** x-axis "Day" (1 to 20); y-axis "Coefficients (90% CI)"

**Note:** This figure plots the estimated coefficients (and 90% confidence intervals) on sentiment PC1, high-level attention, and mid-level attention for small-cap, mid-cap, and large-cap firms, separately. Firm size categories follow those in Table 1. High-level (or mid-level) attention equals 1 if the firm-day attention PC1 is above the 67th percentile (or between percentiles 33 and 67) within a year, and zero otherwise. The outcome is the cumulative abnormal return as of day t+1, t+2, ..., t+20, starting on day t+1. We estimate separate regressions for each horizon, and sentiment and attention coefficients are estimated in the same regression. Sentiment are standardized (z) within firm size category and attention within firm size category and year. Everything else follows Table 6 column 1.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A8: Informativeness of StockTwits Sentiment on Next-Day Returns Over Time, Stocks Most Discussed in Long Messages

- **Chart type:** Coefficient plot at semester frequency with 90% confidence intervals, 2018h1 through 2021h2 plotted; a vertical dashed line marks the semester of the character limit increase
- **Axes:** x-axis: semesters (2018h1, 2019h1, 2020h1, 2021h1); y-axis "Coefficients (90% CI)"

**Note:** This figure plots the estimated coefficients (and 90% confidence intervals) on StockTwits sentiment for stocks with top quartile daily average character length per message by semester. The vertical dashed line denotes the semester when StockTwits increased its character limit. The sample and specification follow Table 6 columns 3 except that sentiment and attention are replaced with the interactions between the social signals and semester indicators for 2012h1 through 2021h2. For readability, only coefficients starting in 2018 are plotted.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A9: Informativeness of StockTwits Sentiment on Next-Day Returns Over Time, StockTwits Old Users

- **Chart type:** Coefficient plot at annual frequency with 90% confidence intervals, 2012 through 2021
- **Axes:** x-axis: years (2012-2021); y-axis "Coefficients (90% CI)"

**Note:** This figure plots the estimated coefficients (and 90% confidence intervals) on sentiment from StockTwits old (or established) users by year. Old users are those who joined StockTwits before 2020. Everything else follows Table 9 column 4 except that (i) sample spans 2012 through 2021, and (ii) sentiment PC1, attention PC1, and their interactions with post dummy are replaced with the interactions between the social signals and annual indicators for 2012 through 2021.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Table A1: How Common is the Social Signal across User Types on StockTwits?

- **Table type:** PCA loadings (non-residualized signals)
- **Unit of observation:** Firm-day
- **Sample and variable definitions:** Follow Table 5
- **Standard errors:** In parentheses (fraction of variation only); double clustered by firm and by date via a block bootstrap procedure following Thompson (2011)
- **Significance:** not reported in table note

#### Panel A: PCA of Attention Signals

| user_group | statistic | PC1 | PC2 | PC3 | PC4 | PC5 |
|---|---|---:|---:|---:|---:|---:|
| Top 1% | loading | 0.426 | 0.694 | 0.570 | -0.105 | -0.034 |
| Professional | loading | 0.446 | 0.359 | -0.684 | 0.413 | 0.186 |
| Intermediate | loading | 0.462 | -0.187 | -0.234 | -0.393 | -0.736 |
| Novice | loading | 0.443 | -0.501 | 0.391 | 0.630 | -0.055 |
| No label | loading | 0.458 | -0.322 | -0.007 | -0.518 | 0.647 |
| Fraction of variation | estimate | 87.7% | 6.4% | 3% | 1.8% | 1.1% |
| Fraction of variation | standard_error | 2.757 | 1.368 | 0.882 | 0.386 | 0.276 |

#### Panel B: PCA of Sentiment Signals

| user_group | statistic | PC1 | PC2 | PC3 | PC4 | PC5 |
|---|---|---:|---:|---:|---:|---:|
| Top 1% | loading | 0.561 | -0.215 | -0.129 | 0.078 | -0.785 |
| Professional | loading | 0.468 | -0.446 | -0.432 | 0.294 | 0.556 |
| Intermediate | loading | 0.387 | 0.104 | 0.799 | 0.419 | 0.159 |
| Novice | loading | 0.287 | 0.858 | -0.369 | 0.205 | 0.052 |
| No label | loading | 0.484 | 0.087 | 0.147 | -0.831 | 0.215 |
| Fraction of variation | estimate | 28.2% | 19.4% | 18.9% | 17.5% | 15.9% |
| Fraction of variation | standard_error | 0.090 | 0.033 | 0.032 | 0.047 | 0.067 |

**Note:** This table repeats the principal component analyses in Table 5 Panels B and C using non-residualized social signals. Sample and variable definitions follow those in Table 5. Standard errors in parentheses are double clustered by firm and by date via a block bootstrap procedure following Thompson (2011).

### Table A2: How Common is the Social Signal across Platforms? Abnormal Attention

- **Table type:** PCA loadings
- **Unit of observation:** Firm-day
- **Attention measure:** Abnormal attention — the deviation in number of messages for a firm-day observation from its median in the preceding 10 days
- **Standard errors:** In parentheses (fraction of variation only); double clustered by firm and by date via a block bootstrap procedure following Thompson (2011)
- **Significance:** not reported in table note

#### Panel A: PCA of Abnormal Attention Signals

| platform | statistic | PC1 | PC2 | PC3 |
|---|---|---:|---:|---:|
| StockTwits | loading | 0.525 | -0.695 | 0.491 |
| Twitter | loading | 0.679 | -0.005 | -0.734 |
| Seeking Alpha | loading | 0.513 | 0.719 | 0.469 |
| Fraction of variation | estimate | 51.7% | 30.7% | 17.6% |
| Fraction of variation | standard_error | 1.068 | 0.631 | 0.766 |

#### Panel B: PCA of Residualized Abnormal Attention Signals

| residualization | platform | statistic | PC1 | PC2 | PC3 |
|---|---|---|---:|---:|---:|
| News | StockTwits | loading | 0.595 | -0.531 | 0.603 |
| News | Twitter | loading | 0.685 | -0.056 | -0.726 |
| News | Seeking Alpha | loading | 0.419 | 0.846 | 0.330 |
| News | Fraction of variation | estimate | 49% | 31.6% | 19.5% |
| News | Fraction of variation | standard_error | 1.073 | 0.483 | 1.034 |
| News & firm FEs | StockTwits | loading | 0.610 | -0.489 | 0.623 |
| News & firm FEs | Twitter | loading | 0.686 | -0.068 | -0.725 |
| News & firm FEs | Seeking Alpha | loading | 0.397 | 0.870 | 0.294 |
| News & firm FEs | Fraction of variation | estimate | 48.6% | 31.7% | 19.7% |
| News & firm FEs | Fraction of variation | standard_error | 1.004 | 0.428 | 1.073 |

**Note:** This table repeats the principal component analyses in Tables 2 and 3 using abnormal attention signal, i.e., the deviation in number of messages for a firm-day observation from its median in the preceding 10 days. Standard errors in parentheses are double clustered by firm and by date via a block bootstrap procedure following Thompson (2011).

### Table A3: How Common is Stock Coverage across Platforms?

- **Table type:** Correlation (Panel A) and PCA loadings (Panels B and C)
- **Unit of observation:** Firm-day; sample consists of firm-day observations on all trading days
- **Coverage:** An indicator for when a firm is mentioned on a platform in a day
- **Standard errors:** In parentheses (fraction of variation only); double clustered by firm and by date via a block bootstrap procedure following Thompson (2011)
- **Significance:** not reported in table note

#### Panel A: Correlations with Coverage on StockTwits

| variable | Twitter | Seeking Alpha |
|---|---:|---:|
| StockTwits | 0.341 | 0.152 |

#### Panel B: PCA of Coverage

| platform | statistic | PC1 | PC2 | PC3 |
|---|---|---:|---:|---:|
| StockTwits | loading | 0.598 | -0.490 | 0.635 |
| Twitter | loading | 0.640 | -0.185 | -0.746 |
| Seeking Alpha | loading | 0.482 | 0.852 | 0.203 |
| Fraction of variation | estimate | 49.6% | 28.8% | 21.6% |
| Fraction of variation | standard_error | 0.354 | 0.178 | 0.260 |

#### Panel C: PCA of Residualized Coverage

*[Conversion note: this panel is labeled "Panel B" in the original PDF — a duplicate of the previous panel header. The table note refers to it as Panel C; relabeled accordingly here and flagged.]*

| residualization | platform | statistic | PC1 | PC2 | PC3 |
|---|---|---|---:|---:|---:|
| News | StockTwits | loading | 0.614 | -0.434 | 0.659 |
| News | Twitter | loading | 0.651 | -0.194 | -0.734 |
| News | Seeking Alpha | loading | 0.447 | 0.880 | 0.164 |
| News | Fraction of variation | estimate | 47.9% | 30% | 22.1% |
| News | Fraction of variation | standard_error | 0.354 | 0.188 | 0.264 |
| News & firm FEs | StockTwits | loading | 0.685 | -0.177 | 0.707 |
| News & firm FEs | Twitter | loading | 0.685 | -0.177 | -0.707 |
| News & firm FEs | Seeking Alpha | loading | 0.250 | 0.968 | 0.000 |
| News & firm FEs | Fraction of variation | estimate | 43.4% | 32.7% | 23.9% |
| News & firm FEs | Fraction of variation | standard_error | 0.198 | 0.044 | 0.197 |

**Note:** This table reports the correlations and principal component analyses of social media coverage across platforms. Coverage is an indicator for when a firm is mentioned on a platform in a day. Panel A reports the bivariate correlations of coverage between StockTwits and Twitter (or Seeking Alpha). Panels B and C report the principal components for stock coverage across all three platforms. Panels B uses non-residualized coverage while panel C uses residualized coverage. The residualization method follows that in Table 3 columns 1-6. The sample consists of firm-day observations on all trading days. Standard errors in parentheses are double clustered by firm and by date via a block bootstrap procedure following Thompson (2011).

### Table A4: How Common is the Social Signal across Platforms? Including the Reddit Wall St. Bets Signal

- **Table type:** PCA loadings (residualized signals)
- **Unit of observation:** Firm-day
- **Sample:** Firm-day observations with at least 10 messages on StockTwits from January 2018 through December 2021, excluding January and February of 2021 (the months surrounding the GME event)
- **Standard errors:** In parentheses (fraction of variation only); double clustered by firm and by date via a block bootstrap procedure following Thompson (2011)
- **Significance:** not reported in table note

#### Panel A: PCA of Residualized Attention Signals

| platform | statistic | PC1 | PC2 | PC3 | PC4 |
|---|---|---:|---:|---:|---:|
| StockTwits | loading | 0.564 | 0.153 | -0.567 | 0.580 |
| Twitter | loading | 0.575 | -0.150 | -0.249 | -0.764 |
| Seeking Alpha | loading | 0.428 | -0.674 | 0.532 | 0.281 |
| Reddit WSB | loading | 0.409 | 0.707 | 0.577 | -0.020 |
| Fraction of variation | estimate | 51.1% | 24.1% | 13.3% | 11.5% |
| Fraction of variation | standard_error | 3.794 | 0.512 | 2.041 | 1.716 |

#### Panel B: PCA of Residualized Sentiment Signals

| platform | statistic | PC1 | PC2 | PC3 | PC4 |
|---|---|---:|---:|---:|---:|
| StockTwits | loading | 0.640 | -0.082 | -0.338 | 0.686 |
| Twitter | loading | 0.660 | -0.127 | -0.178 | -0.719 |
| Seeking Alpha | loading | 0.369 | 0.001 | 0.923 | 0.110 |
| Reddit WSB | loading | 0.138 | 0.988 | -0.052 | -0.036 |
| Fraction of variation | estimate | 27.5% | 25% | 24.6% | 22.9% |
| Fraction of variation | standard_error | 0.090 | 0.014 | 0.035 | 0.085 |

**Note:** This table repeats the principal component analyses in columns 7-9 of Table 3 while adding the Reddit Wall Street Bets social signal. The sample consists of firm-day observations with at least 10 messages on StockTwits from January 2018 through December 2021, excluding January and February of 2021 (the months surrounding the GME event). Standard errors in parentheses are double clustered by firm and by date via a block bootstrap procedure following Thompson (2011).

### Table A5: How Do Next-Day Returns Relate to Social Signals? Additional Sentiment PC's

- **Table type:** Regression
- **Unit of observation:** Firm-day
- **Dependent variable:** $AR_{i,t+1}$ (%) — abnormal returns on day t+1 in percentage points
- **Estimator:** OLS with firm and date fixed effects
- **Standard errors:** In parentheses; double clustered by firm and by date
- **All columns include:** ten lags (t-1 to t-10) of sentiment and attention; controls
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | specification |
|---:|---|
| 1 | Reproduces Table 6 column 1 (PC1s only) |
| 2 | Adds sentiment PC2 and PC3 |

#### Estimates

| variable | statistic | model_1 | model_2 |
|---|---|---:|---:|
| Sentiment PC1_{i,t}(z) | coefficient | 0.061*** | 0.061*** |
| Sentiment PC1_{i,t}(z) | standard_error | 0.009 | 0.009 |
| Sentiment PC2_{i,t}(z) | coefficient | | 0.052*** |
| Sentiment PC2_{i,t}(z) | standard_error | | 0.009 |
| Sentiment PC3_{i,t}(z) | coefficient | | 0.034*** |
| Sentiment PC3_{i,t}(z) | standard_error | | 0.007 |
| Attention PC1_{i,t}(z) | coefficient | -0.131*** | -0.132*** |
| Attention PC1_{i,t}(z) | standard_error | 0.050 | 0.050 |
| DJNW sentiment_{i,t}(z) | coefficient | 0.078*** | 0.071*** |
| DJNW sentiment_{i,t}(z) | standard_error | 0.008 | 0.008 |
| DJNW attention_{i,t}(z) | coefficient | 0.012 | 0.009 |
| DJNW attention_{i,t}(z) | standard_error | 0.011 | 0.010 |

#### Model statistics

| statistic | model_1 | model_2 |
|---|---:|---:|
| Sentiment & Attention_{i,(t-1),...,(t-10)} | Y | Y |
| Controls | Y | Y |
| Firm (i) FE | Y | Y |
| Date (t) FE | Y | Y |
| Outcome Mean | -0.048 | -0.048 |
| Outcome SD | 7.124 | 7.124 |
| Observations | 819,210 | 819,210 |
| R-squared | 0.0320 | 0.0321 |

**Note:** This table provides a robustness test for Table 6 by including additional sentiment PCs. The outcome is abnormal returns (AR) on day t+1 in percentage points. Column 1 reproduces Table 6 column 1; everything in column 2 follows column 1 except for the additional sentiment PCs. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors in parentheses are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level

### Table A6: How Do Next-Day Returns Relate to Social Signals? Annual Rolling Principal Components

- **Table type:** Regression
- **Unit of observation:** Firm-day
- **Dependent variable:** $AR_{i,t+1}$ (%) — abnormal returns on day t+1 in percentage points
- **Estimator:** OLS with firm and date fixed effects
- **Standard errors:** In parentheses; double clustered by firm and by date
- **All columns include:** ten lags (t-1 to t-10) of sentiment and attention; controls
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | specification |
|---:|---|
| 1 | Annual-rolling PC1s, follows Table 6 column 1 |
| 2 | Adds annual-rolling sentiment PC2 and PC3 |

#### Estimates

| variable | statistic | model_1 | model_2 |
|---|---|---:|---:|
| Sentiment PC1_{i,t}(z) | coefficient | 0.061*** | 0.062*** |
| Sentiment PC1_{i,t}(z) | standard_error | 0.010 | 0.010 |
| Sentiment PC2_{i,t}(z) | coefficient | | 0.040*** |
| Sentiment PC2_{i,t}(z) | standard_error | | 0.009 |
| Sentiment PC3_{i,t}(z) | coefficient | | 0.035*** |
| Sentiment PC3_{i,t}(z) | standard_error | | 0.008 |
| Attention PC1_{i,t}(z) | coefficient | -0.158*** | -0.159*** |
| Attention PC1_{i,t}(z) | standard_error | 0.053 | 0.053 |
| DJNW sentiment_{i,t}(z) | coefficient | 0.081*** | 0.074*** |
| DJNW sentiment_{i,t}(z) | standard_error | 0.008 | 0.008 |
| DJNW attention_{i,t}(z) | coefficient | 0.011 | 0.009 |
| DJNW attention_{i,t}(z) | standard_error | 0.012 | 0.012 |

#### Model statistics

| statistic | model_1 | model_2 |
|---|---:|---:|
| Sentiment & Attention_{i,(t-1),...,(t-10)} | Y | Y |
| Controls | Y | Y |
| Firm (i) FE | Y | Y |
| Date (t) FE | Y | Y |
| Outcome Mean | -0.047 | -0.047 |
| Outcome SD | 7.180 | 7.180 |
| Observations | 799,169 | 799,169 |
| R-squared | 0.0322 | 0.0322 |

**Note:** This table provides a robustness test for Table 6 by using annual-rolling principal components (PCs) of the social signals. PCs in a given year are estimated using data from the prior year, so annual-rolling PCs are only available for 2013 through 2021. Column 1 follows Table 6 column 1; everything in column 2 follows column 1 except for the additional sentiment PCs. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors in parentheses are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level

### Table A7: How Do Next-Day Returns Relate to Social Signals? Abnormal Attention

- **Table type:** Regression
- **Unit of observation:** Firm-day
- **Dependent variable:** $AR_{i,t+1}$ (%) — abnormal returns on day t+1 in percentage points
- **Attention measure:** Abnormal attention — the deviation in number of messages for a firm-day observation from its median in the prior 10 days
- **Estimator:** OLS with firm and date fixed effects
- **Standard errors:** In parentheses; double clustered by firm and by date
- **All columns include:** ten lags (t-1 to t-10) of sentiment and attention
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | signal_source |
|---:|---|
| 1 | StockTwits |
| 2 | Twitter |
| 3 | Seeking Alpha |
| 4 | PC1 signal |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 |
|---|---|---:|---:|---:|---:|
| Sentiment_{i,t}(z) | coefficient | 0.054*** | 0.022*** | 0.080*** | 0.061*** |
| Sentiment_{i,t}(z) | standard_error | 0.008 | 0.007 | 0.010 | 0.009 |
| Attention_{i,t}(z) | coefficient | -0.085* | -0.013 | -0.013 | -0.083* |
| Attention_{i,t}(z) | standard_error | 0.047 | 0.027 | 0.008 | 0.042 |
| DJNW sentiment_{i,t}(z) | coefficient | 0.078*** | 0.079*** | 0.069*** | 0.076*** |
| DJNW sentiment_{i,t}(z) | standard_error | 0.008 | 0.008 | 0.008 | 0.008 |
| DJNW attention_{i,t}(z) | coefficient | 0.025** | 0.020 | 0.017 | 0.033** |
| DJNW attention_{i,t}(z) | standard_error | 0.012 | 0.014 | 0.014 | 0.013 |
| 8-K report date_{i,t} | coefficient | 0.020 | 0.022 | 0.022 | 0.034 |
| 8-K report date_{i,t} | standard_error | 0.044 | 0.051 | 0.043 | 0.047 |
| EA date_{i,t} | coefficient | -0.622*** | -0.619*** | -0.632*** | -0.633*** |
| EA date_{i,t} | standard_error | 0.104 | 0.104 | 0.106 | 0.104 |
| Volatility_{i,(t-5)→(t-1)} | coefficient | -0.046 | -0.077 | -0.113 | -0.045 |
| Volatility_{i,(t-5)→(t-1)} | standard_error | 0.368 | 0.369 | 0.375 | 0.371 |
| CAR_{i,(t-5)→(t-1)} | coefficient | -0.008*** | -0.008*** | -0.008*** | -0.008*** |
| CAR_{i,(t-5)→(t-1)} | standard_error | 0.002 | 0.002 | 0.002 | 0.002 |
| CAR_{i,(t-30)→(t-6)} | coefficient | -0.001 | -0.001* | -0.001* | -0.001* |
| CAR_{i,(t-30)→(t-6)} | standard_error | 0.001 | 0.001 | 0.001 | 0.001 |
| Log Google ASVI_{i,t}(z) | coefficient | -0.059*** | -0.065*** | -0.066*** | -0.057*** |
| Log Google ASVI_{i,t}(z) | standard_error | 0.017 | 0.017 | 0.017 | 0.017 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 |
|---|---:|---:|---:|---:|
| Sentiment & Attention_{i,(t-1),...,(t-10)} | Y | Y | Y | Y |
| Firm (i) FE | Y | Y | Y | Y |
| Date (t) FE | Y | Y | Y | Y |
| Outcome Mean | -0.049 | -0.049 | -0.049 | -0.049 |
| Outcome SD | 7.127 | 7.127 | 7.127 | 7.127 |
| Observations | 818,516 | 818,516 | 818,516 | 818,516 |
| R-squared | 0.0320 | 0.0319 | 0.0319 | 0.0320 |

**Note:** This table provides a robustness test for Table 6 by using abnormal attention, i.e., the deviation in number of messages for a firm-day observation from its median in the prior 10 days. Everything else follows Table 6. The outcome is abnormal returns (AR) on day t+1 in percentage points. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level.

### Table A8: How Do Next-Day Returns Relate to Social Signals? Including the Reddit WallStBets Signal

- **Table type:** Regression
- **Unit of observation:** Firm-day
- **Dependent variable:** $AR_{i,t+1}$ (%) — abnormal returns on day t+1 in percentage points
- **Sample:** Firm-day observations with at least 10 messages on StockTwits from January 2018 through December 2021, excluding January and February of 2021 (the months surrounding the GME event)
- **Estimator:** OLS with firm and date fixed effects
- **Standard errors:** In parentheses; double clustered by firm and by date
- **All columns include:** ten lags (t-1 to t-10) of sentiment and attention
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | signal_source |
|---:|---|
| 1 | All four platform signals jointly (WSB, StockTwits, Twitter, Seeking Alpha) |
| 2 | Reddit WSB only |
| 3 | StockTwits only |
| 4 | Twitter only |
| 5 | Seeking Alpha only |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| WSB sentiment_{i,t}(z) | coefficient | 0.001 | 0.002 | | | |
| WSB sentiment_{i,t}(z) | standard_error | 0.011 | 0.011 | | | |
| WSB attention_{i,t}(z) | coefficient | 0.136*** | 0.065** | | | |
| WSB attention_{i,t}(z) | standard_error | 0.033 | 0.030 | | | |
| StockTwits sentiment_{i,t}(z) | coefficient | 0.034*** | | 0.035*** | | |
| StockTwits sentiment_{i,t}(z) | standard_error | 0.012 | | 0.012 | | |
| StockTwits attention_{i,t}(z) | coefficient | -0.470*** | | -0.352*** | | |
| StockTwits attention_{i,t}(z) | standard_error | 0.117 | | 0.104 | | |
| Twitter sentiment_{i,t}(z) | coefficient | -0.010 | | | 0.002 | |
| Twitter sentiment_{i,t}(z) | standard_error | 0.025 | | | 0.025 | |
| Twitter attention_{i,t}(z) | coefficient | 0.037 | | | -0.092* | |
| Twitter attention_{i,t}(z) | standard_error | 0.061 | | | 0.049 | |
| Seeking Alpha sentiment_{i,t}(z) | coefficient | 0.067*** | | | | 0.067*** |
| Seeking Alpha sentiment_{i,t}(z) | standard_error | 0.013 | | | | 0.013 |
| Seeking Alpha attention_{i,t}(z) | coefficient | -0.061 | | | | -0.071* |
| Seeking Alpha attention_{i,t}(z) | standard_error | 0.038 | | | | 0.037 |
| DJNW sentiment_{i,t}(z) | coefficient | 0.085*** | 0.096*** | 0.097*** | 0.097*** | 0.085*** |
| DJNW sentiment_{i,t}(z) | standard_error | 0.012 | 0.012 | 0.012 | 0.012 | 0.012 |
| DJNW attention_{i,t}(z) | coefficient | -0.037 | -0.056** | -0.017 | -0.028 | -0.036 |
| DJNW attention_{i,t}(z) | standard_error | 0.025 | 0.023 | 0.023 | 0.026 | 0.023 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| Sentiment & Attention_{i,(t-1),...,(t-10)} | Y | Y | Y | Y | Y |
| Firm (i) FE | Y | Y | Y | Y | Y |
| Date (t) FE | Y | Y | Y | Y | Y |
| Outcome Mean | -0.073 | -0.073 | -0.073 | -0.073 | -0.073 |
| Outcome SD | 7.386 | 7.386 | 7.386 | 7.386 | 7.386 |
| Observations | 491,939 | 491,939 | 491,939 | 491,939 | 491,939 |
| R-squared | 0.0350 | 0.0344 | 0.0347 | 0.0344 | 0.0344 |

**Note:** This table reports how next-day returns relate to social signals on Reddit, for comparison with other social signals. The outcome is abnormal returns (AR) on day t+1 in percentage points. Everything else follows Table 6. The sample consists of firm-day observations with at least 10 messages on StockTwits from January 2018 through December 2021, excluding January and February of 2021 (the months surrounding the GME event). (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level.

### Table A9: Relationship between StockTwits Message Length and User Type

- **Table type:** Regression
- **Unit of observation:** Message (message j about firm i on day t)
- **Dependent variable:** Message Length_{j,i,t} — the number of characters in a message
- **Sample:** All messages posted between May 8, 2018 and May 8, 2020 for firm-days with at least 10 messages on StockTwits
- **Estimator:** OLS with firm and date fixed effects
- **Standard errors:** In parentheses; double clustered by firm and by date
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Estimates

| variable | statistic | model_1 | model_2 |
|---|---|---:|---:|
| Post_t × Top 1%_j | coefficient | 0.449 | |
| Post_t × Top 1%_j | standard_error | 1.432 | |
| Post_t × Professional_j | coefficient | | 9.806*** |
| Post_t × Professional_j | standard_error | | 1.485 |
| Post_t × Intermediate_j | coefficient | | 1.894** |
| Post_t × Intermediate_j | standard_error | | 0.939 |
| Post_t × Novice_j | coefficient | | -1.438 |
| Post_t × Novice_j | standard_error | | 1.284 |
| Top 1%_j | coefficient | 0.535 | |
| Top 1%_j | standard_error | 0.722 | |
| Professional_j | coefficient | | 5.270*** |
| Professional_j | standard_error | | 0.522 |
| Intermediate_j | coefficient | | 3.697*** |
| Intermediate_j | standard_error | | 0.366 |
| Novice_j | coefficient | | -1.664** |
| Novice_j | standard_error | | 0.644 |

#### Model statistics

| statistic | model_1 | model_2 |
|---|---:|---:|
| Firm (i) FE | Y | Y |
| Date (t) FE | Y | Y |
| Outcome Mean | 74.793 | 74.793 |
| Outcome SD | 79.773 | 79.773 |
| Observations | 24,575,440 | 24,575,440 |
| R-squared | 0.0319 | 0.0331 |

**Note:** This table presents the relationship between message length and user type on StockTwits. The outcome is the number of characters in a message. $Post_t$ is an indicator for messages being posted on or after May 8, 2020, and zero otherwise. $Top\ 1\%_j$, $Professional_j$, $Intermediate_j$, and $Novice_j$ are indicators for message j being written by influencers, professionals, intermediate experience, and novice users, respectively. The sample consists of all messages posted between May 8, 2018 and May 8, 2020 for firm-days with at least 10 messages on StockTwits. Standard errors are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level.

[Conversion note: The printed table note defines $Post_t$ as "on or after May 8, 2020," which conflicts with the sample window (May 8, 2018 to May 8, 2020) and with the May 8, 2019 character-limit event date used throughout the paper. The note is transcribed exactly as printed; this is likely a typographical error in the source for "May 8, 2019."]

### Table A10: How Do Next-Day Returns Relate to Social Signals? by StockTwits User Group

- **Table type:** Regression
- **Unit of observation:** Firm-day
- **Dependent variable:** $AR_{i,t+1}$ (%) — abnormal returns on day t+1 in percentage points
- **Estimator:** OLS with firm and date fixed effects
- **Standard errors:** In parentheses; double clustered by firm and by date
- **All columns include:** ten lags (t-1 to t-10) of sentiment and attention
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | StockTwits user group |
|---:|---|
| 1 | Top 1% |
| 2 | Professional |
| 3 | Intermediate |
| 4 | Novice |
| 5 | No label |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| Sentiment_{i,t}(z) | coefficient | 0.013* | 0.027*** | 0.011 | 0.003 | 0.034*** |
| Sentiment_{i,t}(z) | standard_error | 0.007 | 0.008 | 0.007 | 0.008 | 0.007 |
| Attention_{i,t}(z) | coefficient | -0.077** | -0.126*** | -0.111** | -0.111*** | -0.155*** |
| Attention_{i,t}(z) | standard_error | 0.035 | 0.044 | 0.044 | 0.038 | 0.049 |
| DJNW sentiment_{i,t}(z) | coefficient | 0.082*** | 0.082*** | 0.082*** | 0.083*** | 0.081*** |
| DJNW sentiment_{i,t}(z) | standard_error | 0.008 | 0.008 | 0.008 | 0.008 | 0.008 |
| DJNW attention_{i,t}(z) | coefficient | 0.002 | 0.008 | 0.002 | 0.002 | 0.006 |
| DJNW attention_{i,t}(z) | standard_error | 0.010 | 0.010 | 0.010 | 0.010 | 0.010 |
| 8-K report date_{i,t} | coefficient | 0.052 | 0.065 | 0.053 | 0.051 | 0.059 |
| 8-K report date_{i,t} | standard_error | 0.043 | 0.044 | 0.043 | 0.042 | 0.043 |
| EA date_{i,t} | coefficient | -0.545*** | -0.545*** | -0.544*** | -0.545*** | -0.544*** |
| EA date_{i,t} | standard_error | 0.091 | 0.091 | 0.091 | 0.091 | 0.091 |
| Volatility_{i,(t-5)→(t-1)} | coefficient | -0.075 | -0.063 | -0.083 | -0.040 | -0.024 |
| Volatility_{i,(t-5)→(t-1)} | standard_error | 0.373 | 0.376 | 0.376 | 0.376 | 0.377 |
| CAR_{i,(t-5)→(t-1)} | coefficient | -0.008*** | -0.008*** | -0.008*** | -0.007*** | -0.007*** |
| CAR_{i,(t-5)→(t-1)} | standard_error | 0.002 | 0.002 | 0.002 | 0.002 | 0.002 |
| CAR_{i,(t-30)→(t-6)} | coefficient | -0.001* | -0.001* | -0.001* | -0.001* | -0.001* |
| CAR_{i,(t-30)→(t-6)} | standard_error | 0.001 | 0.001 | 0.001 | 0.001 | 0.001 |
| Log Google ASVI_{i,t}(z) | coefficient | -0.058*** | -0.054*** | -0.056*** | -0.053*** | -0.051*** |
| Log Google ASVI_{i,t}(z) | standard_error | 0.017 | 0.017 | 0.017 | 0.017 | 0.017 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| Sentiment & Attention_{i,(t-1),...,(t-10)} | Y | Y | Y | Y | Y |
| Firm (i) FE | Y | Y | Y | Y | Y |
| Date (t) FE | Y | Y | Y | Y | Y |
| Outcome Mean | -0.048 | -0.048 | -0.048 | -0.048 | -0.048 |
| Outcome SD | 7.124 | 7.124 | 7.124 | 7.124 | 7.124 |
| Observations | 819,210 | 819,210 | 819,210 | 819,210 | 819,210 |
| R-squared | 0.0319 | 0.0320 | 0.0319 | 0.0320 | 0.0320 |

**Note:** This table repeats Table 6 using social signals from various user groups on StockTwits. Everything else follows Table 6. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level.

### Table A11: How Did Informativeness of StockTwits Signals Change around the StockTwits Character Limit Increase? Firms Discussed in Long vs. Short Messages

- **Table type:** Regression (triple-difference design)
- **Unit of observation:** Firm-day
- **Dependent variable:** $AR_{i,t+1}$ (%) — next day abnormal returns in percentage points
- **Sample:** Firm-day observations with at least 10 messages on StockTwits between May 8, 2018 and May 8, 2020
- **Estimator:** OLS with firm and date fixed effects; controls included
- **Standard errors:** In parentheses; double clustered by firm and by date
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Estimates

| variable | statistic | model_1 |
|---|---|---:|
| Post_t × Treated_i × Sentiment_{i,t}(z) | coefficient | 0.178** |
| Post_t × Treated_i × Sentiment_{i,t}(z) | standard_error | 0.082 |
| Post_t × Treated_i × Attention_{i,t}(z) | coefficient | -0.533* |
| Post_t × Treated_i × Attention_{i,t}(z) | standard_error | 0.302 |
| Post_t × Sentiment_{i,t}(z) | coefficient | -0.039 |
| Post_t × Sentiment_{i,t}(z) | standard_error | 0.071 |
| Post_t × Attention_{i,t}(z) | coefficient | 0.294 |
| Post_t × Attention_{i,t}(z) | standard_error | 0.221 |
| Treated_i × Sentiment_{i,t}(z) | coefficient | -0.023 |
| Treated_i × Sentiment_{i,t}(z) | standard_error | 0.053 |
| Treated_i × Attention_{i,t}(z) | coefficient | 0.255 |
| Treated_i × Attention_{i,t}(z) | standard_error | 0.220 |
| Sentiment_{i,t}(z) | coefficient | 0.038 |
| Sentiment_{i,t}(z) | standard_error | 0.049 |
| Attention_{i,t}(z) | coefficient | -0.642*** |
| Attention_{i,t}(z) | standard_error | 0.175 |
| Post_t × Treated_i | coefficient | 0.090 |
| Post_t × Treated_i | standard_error | 0.119 |
| Treated_i | coefficient | -0.034 |
| Treated_i | standard_error | 0.080 |

#### Model statistics

| statistic | model_1 |
|---|---:|
| Controls | Y |
| Firm (i) FE | Y |
| Date (t) FE | Y |
| Outcome Mean | -0.097 |
| Outcome SD | 8.335 |
| Observations | 107,631 |
| R-squared | 0.033 |

**Note:** This table compares how social signals about firms discussed in long vs. short StockTwits messages changed their predictive power for next day abnormal returns (AR) around the StockTwits character limit increase on May 8, 2019. $Treated_i$ is one for stocks whose daily average number of characters per message is in the top quartile; the comparison group is those in the bottom quartile. $Post_t$ is one if a day is on or after May 8, 2019. Controls are 8-K report date indicators, earnings announcement indicators, lagged return volatility (previous five trading days), lagged cumulative abnormal returns (previous five trading days and the 25 days before that), and Log Google ASVI. The sample consists of firm-day observations with at least 10 messages on StockTwits between May 8, 2018 and May 8, 2020. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level.

### Table A12: How Did the Informativeness of Social Signals for Next-Day Returns Change around Information Experiments? Robustness to Using Self-labeled Sentiment

- **Table type:** Regression
- **Unit of observation:** Firm-day
- **Dependent variable:** $AR_{i,t+1}$ (%) (dependent variable not printed in the column header; inferred from the table note's reference to Tables 8 and 9, whose outcome is next-day abnormal returns in percentage points)
- **Sample:** Firm-day observations with at least 10 messages on StockTwits and at least 5 messages from the corresponding user groups on StockTwits
- **Estimator:** OLS with firm and date fixed effects; controls included
- **Standard errors:** In parentheses; double clustered by firm and by date
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | experiment | signal |
|---:|---|---|
| 1 | StockTwits character-limit experiment | Self-labeled |
| 2 | StockTwits character-limit experiment | Self-labeled, top quartile |
| 3 | GME experiment | Self-labeled, new users |
| 4 | GME experiment | Self-labeled, old users |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 |
|---|---|---:|---:|---:|---:|
| Post_t × Sentiment_{i,t}(z) | coefficient | 0.073 | 0.099 | -0.134** | -0.063 |
| Post_t × Sentiment_{i,t}(z) | standard_error | 0.050 | 0.065 | 0.062 | 0.056 |
| Post_t × Attention_{i,t}(z) | coefficient | 0.146 | -0.316 | 0.025 | -0.002 |
| Post_t × Attention_{i,t}(z) | standard_error | 0.092 | 0.242 | 0.108 | 0.090 |
| Sentiment_{i,t}(z) | coefficient | 0.089*** | -0.005 | 0.077 | 0.179*** |
| Sentiment_{i,t}(z) | standard_error | 0.031 | 0.048 | 0.055 | 0.050 |
| Attention_{i,t}(z) | coefficient | -0.321*** | -0.270 | -0.065 | -0.045 |
| Attention_{i,t}(z) | standard_error | 0.098 | 0.194 | 0.068 | 0.059 |
| DJNW sentiment_{i,t}(z) | coefficient | 0.099*** | 0.096*** | 0.079*** | 0.093*** |
| DJNW sentiment_{i,t}(z) | standard_error | 0.019 | 0.031 | 0.022 | 0.021 |
| DJNW attention_{i,t}(z) | coefficient | 0.013 | -0.044 | -0.079*** | -0.069* |
| DJNW attention_{i,t}(z) | standard_error | 0.028 | 0.089 | 0.027 | 0.038 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 |
|---|---:|---:|---:|---:|
| Controls | Y | Y | Y | Y |
| Firm (i) FE | Y | Y | Y | Y |
| Date (t) FE | Y | Y | Y | Y |
| Outcome Mean | -0.088 | 0.047 | -0.062 | 0.007 |
| Outcome SD | 8.212 | 6.825 | 8.263 | 8.568 |
| Observations | 182,539 | 42,387 | 189,562 | 205,047 |
| R-squared | 0.027 | 0.073 | 0.061 | 0.051 |

**Note:** This table presents robustness tests for Table 8 and Table 9 by using signals based on self-labeled messages on StockTwits. The sample consists of firm-day observations with at least 10 messages on StockTwits and at least 5 messages from the corresponding user groups on StockTwits. Everything else follows Table 8 and Table 9. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors are double double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level.

[Conversion note: "double double clustered" appears as printed in the source note.]

### Table A13: How Did the Informativeness of the Social Signal for Next-Day Returns Change around the GameStop Event? New vs. Old users

- **Table type:** Regression (triple-difference design)
- **Unit of observation:** Firm-day (signals constructed separately by user group j)
- **Dependent variable:** $AR_{i,t+1}$ (%) — next-day abnormal returns in percentage points
- **Sample:** Firm-day observations with at least 10 messages on StockTwits between February 1, 2020 and December 31, 2021, excluding January 2021
- **Estimator:** OLS with firm and date fixed effects; controls included
- **Standard errors:** In parentheses; double clustered by firm and by date
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Estimates

| variable | statistic | model_1 |
|---|---|---:|
| Post_t × New user_j × Sentiment_{i,t}(z) | coefficient | -0.096* |
| Post_t × New user_j × Sentiment_{i,t}(z) | standard_error | 0.049 |
| Post_t × New user_j × Attention_{i,t}(z) | coefficient | 0.038 |
| Post_t × New user_j × Attention_{i,t}(z) | standard_error | 0.032 |
| New user_j × Sentiment_{i,t}(z) | coefficient | 0.058 |
| New user_j × Sentiment_{i,t}(z) | standard_error | 0.041 |
| New user_j × Attention_{i,t}(z) | coefficient | -0.017 |
| New user_j × Attention_{i,t}(z) | standard_error | 0.030 |
| Post_t × Sentiment_{i,t}(z) | coefficient | -0.000 |
| Post_t × Sentiment_{i,t}(z) | standard_error | 0.032 |
| Post_t × Attention_{i,t}(z) | coefficient | -0.021 |
| Post_t × Attention_{i,t}(z) | standard_error | 0.092 |
| Sentiment_{i,t}(z) | coefficient | 0.037 |
| Sentiment_{i,t}(z) | standard_error | 0.026 |
| Attention_{i,t}(z) | coefficient | -0.052 |
| Attention_{i,t}(z) | standard_error | 0.046 |
| Post_t × New user_j | coefficient | -0.027*** |
| Post_t × New user_j | standard_error | 0.010 |
| New user_j | coefficient | 0.025*** |
| New user_j | standard_error | 0.009 |
| DJNW sentiment_{i,t}(z) | coefficient | 0.088*** |
| DJNW sentiment_{i,t}(z) | standard_error | 0.016 |
| DJNW attention_{i,t}(z) | coefficient | -0.063** |
| DJNW attention_{i,t}(z) | standard_error | 0.029 |

#### Model statistics

| statistic | model_1 |
|---|---:|
| Controls | Y |
| Firm (i) FE | Y |
| Date (t) FE | Y |
| Outcome Mean | -0.005 |
| Outcome SD | 7.864 |
| Observations | 578,184 |
| R-squared | 0.049 |

**Note:** This table compares how social signals from new vs. old StockTwits users changed their predictive power for next-day abnormal returns (AR) around the GameStop event on January 28, 2021. $Post_t$ is one if a day is on or after February 1, 2021. $New\ user_j$ is one if the social signals are from users who joined StockTwits in 2020 or 2021; the comparison group is social signals from users who joined before 2020. Controls are 8-K report day and earnings announcement day indicators, lagged return volatility (previous five trading days), lagged cumulative abnormal returns (previous five trading days and the 25 days before that), and Log Google ASVI. The sample consists of firm-day observations with at least 10 messages on StockTwits between February 1, 2020 and December 31, 2021, excluding January 2021. (z) denotes a standardized variable (mean 0, standard deviation 1 using the estimation sample statistics). Standard errors are double clustered by firm and by date. *** 1%, ** 5%, * 10% significance level.
