---
title: "Social Media and Finance"
authors: ["J. Anthony Cookson", "William Mullins", "Marina Niessner"]
date: "2024-05-09"
status: "Published (review article)"
journal: "Oxford Research Encyclopedia of Economics and Finance, 2024"
doi: "10.1093/acrefore/9780190625979.013.957"
url: "https://ssrn.com/abstract=4806692"
jel: ["G00", "G41", "L82"]
keywords: ["Social media", "Social finance", "information environment"]
conversion: "Text-only Markdown for LLM reading. Images omitted. Figures preserved as captions and descriptions; no plotted values inferred."
mode: "publication"
---

# Social Media and Finance

## Converter's summary

This summary was written by the converter, not the authors. The article is a survey of the academic literature on social media and finance by J. Anthony Cookson (CU Boulder), William Mullins (UC San Diego), and Marina Niessner (Indiana), dated May 9, 2024. It organizes the literature around a central distinction: research that uses social media as a lens to study general financial behavior (investor beliefs and disagreement, attention, social networks) versus research that studies the effects of social media itself on financial markets (signal informativeness, informational efficiency, rumors and fake news, coordination). The survey also maps the social media data landscape: the main platforms studied in academic finance (Seeking Alpha, X/Twitter, StockTwits, and Reddit's WallStreetBets), their usage over time (Figures 2-4), and data sources after platforms closed API access to researchers in 2022-2023. It contrasts social media with traditional media, noting the strongly bullish tilt of investor social media (around 80% bullish posts) versus the negative tilt of the financial press. Key themes include the deterioration of the social media signal after the GameStop short squeeze, echo chambers and partisan disagreement among investors, social media's role in the Silicon Valley Bank run, and open questions raised by AI and LLMs for the social media ecosystem. The article contains no regression tables; its four figures are descriptive plots of platform usage.

## Abstract

Social media has become an integral part of the financial information environment, changing the way financial information is produced, consumed and distributed. This article surveys the financial social media literature, distinguishing between research using social media as a lens to shed light on more general financial behavior and research exploring the effects of social media on financial markets. We also review the social media data landscape.

**Keywords:** Social media, Social finance, information environment

**JEL Codes:** G00, G41, L82

**Acknowledgments:** This draft has benefited from conversations and helpful comments from Beth Blankespoor, Alex Chinco, Shanna Cookson, Chukwuma Dim, Rawley Heimer, David Hirshleifer, Byoung-Hyoun Hwang, Russell Jame, Runjing Lu, Karsten Müller, Lin Peng, Jason Sandvik, Johannes Stroebel, and Yongxin Xu. We thank Betty Liu and Shijia Wu for sharing Seeking Alpha data. We also thank Context Analytics for sharing StockTwits and Twitter data.

**Author contact:** Cookson (tony.cookson@colorado.edu), Mullins (wmullins@ucsd.edu), and Niessner (marina.niessner@gmail.com).

## 1 Motivation

> Investing in speculative assets is a social activity. Investors spend a substantial part of their leisure time discussing investments, reading about investments, or gossiping about others' successes or failures in investing. It is thus plausible that investors' behavior (and hence prices of speculative assets) would be influenced by social movements. Shiller (1984)

Social interactions have increasingly moved to online social media platforms over the past 20 years, changing how people acquire information about the world and affecting all domains of life.[^1] There has also been a rapid increase in finance-specific social media use (e.g., StockTwits, FinTwit, SeekingAlpha, Reddit's WallStreetBets) and the concurrent development of apps and online trading platforms that bring financial decisions online (e.g., Robinhood and eToro). As social media grows, it has sparked important events in financial markets and in the real economy, such as GameStop's trading frenzy and potentially the run on Silicon Valley Bank.

[^1]: For example, 53% of users on X (formerly, Twitter) report getting news from the platform. https://www.pewresearch.org/journalism/fact-sheet/social-media-and-news-fact-sheet/

In this article, we review the growing academic literature on financial social media, how it connects to ideas on social economics and information economics, and we outline avenues and challenges for future research. Although recent events naturally drive interest in social media research, the underlying economic mechanisms — such as information cascades, network dynamics and narrative economics — play an important role in financial markets and have been studied by academics since at least the 1980s (e.g., Shiller, 1984; Welch, 1992).

We distinguish between two broad approaches to research on social media and finance: uncovering the effects of social media on financial markets versus using social media as a lens to shed light on more general financial behavior. Of course, most research projects are a blend of these two approaches. We hope this distinction proves useful as an organizing principle for existing work and in orienting new research in this area.

The impact of financial social media can only be understood in the context of the pre-existing information ecosystem, which was dominated by specialized producers, distributors, and consumers of financial information. Credentialed information producers (accountants, analysts, financial journalists) produced the vast majority of financial information. This information was distributed mainly to financial professionals, through a handful of specialized newspapers and TV channels, as well as through in-person social networks.

Financial social media has profoundly altered this equilibrium. On production, social media has led to a broader class of securities 'analysts': now, non-experts routinely produce analyses shared broadly via social media. On information consumption, retail traders regularly source ideas about financial markets from freely available social media posts. In addition, because of the rising importance of social media for these functions, the network structure of information production and consumption can also have a material impact on financial markets. The overall consequence is an information environment that, at least potentially, distills dispersed and decentralized knowledge (Hayek, 1945), and that provides more in-depth coverage of smaller firms and markets. A further consequence is the partial dis-intermediation of traditional information producers, as social media on the one hand removes their ability to monopolize the news coverage and the associated narratives, but on the other hand also sidesteps their quality controls, potentially facilitating the spread of rumors and fake news.

A critical function of investor social media is that it democratizes access to financial information by making it available to those outside the financial sector. However, the resulting deluge of information means that it is no longer possible to consume most of the available information: investors are forced to make choices about which information to consume. Furthermore, rather than traditional media editors determining which stories are featured, thus receiving the most attention, social media attention is driven by popularity, often mediated via algorithms. In turn, this enhances the scope for information cascades (Bikhchandani, Hirshleifer, and Welch, 1992; Welch, 1992; Banerjee, 1992; Bikhchandani, Hirshleifer, Tamuz, and Welch, 2024) and for coordinated sentiment to influence markets.

These changes to information production, consumption and distribution are the major themes of the literature on financial social media. In subsequent sections, we describe these innovations and their economic implications. We begin by describing the social media data landscape, which has made much of the empirical research into financial social media possible.

## 2 Social media data landscape

Although social media platforms have become ubiquitous over the last 15 years, an early incarnation of financial social media appeared over 30 years ago. In this section we describe the evolution of social media platforms, as well as data sources. We also briefly review the differences between social media and traditional media.

### 2.1 Social media platforms

Figure 1 presents the launch year, and in some cases the end-year, of the major financial social media platforms. Two important early platforms were The Motley Fool and Yahoo Finance Message Boards, both founded in the 1990s. While The Motley Fool still operates, Yahoo's message boards ceased to exist in 2019. The Motley Fool consists of lengthy articles written either by contributors or by The Motley Fool's staff. The website further includes a separate platform called CAPS where individuals can forecast the performance of most stocks relative to the S&P500 at various horizons. The CAPS platform, with predictions from individual investors, foreshadowed the subsequent rise of social media.

### Figure 1: Evolution of Social Media Landscape

**Caption:** This figure shows the founding year, and in some cases the ending year, of the main social media platforms that have emerged over the past 30+ years.

**Description (from visible figure labels):** A timeline chart spanning 1992-2023. Platforms shown (as horizontal arrows from founding year): Motley Fool (with CAPS as a sub-segment), Yahoo Finance Message Boards (ending in the late 2010s), Facebook, Seeking Alpha, Reddit (with WSB as a sub-segment from 2013), Twitter (relabeled X at the end), StockTwits, Instagram, and TikTok.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

The next, much larger wave of social media platforms launched between 2004 and 2010. Some were general-use websites like Facebook, Reddit, Twitter, and Instagram, whereas others were specifically financial, such as Seeking Alpha and StockTwits. Over time, both Reddit and Twitter have developed large finance sub components – WallStreetBets (WSB) on Reddit and FinTwit on Twitter. The subreddit WSB was launched in 2013, while in 2012 Twitter introduced the "cashtag" (\$) to be used with tickers, helping to separate finance-related tweets from general conversations. The social video platform TikTok was launched in 2016, and has become a forum for some finance-related content in a video format.

### 2.2 Main Financial Social Media Platforms

The four investor social media platforms that have been studied in academic finance are X (formerly Twitter), StockTwits, Seeking Alpha, and Reddit's WallStreetBets. Each platform has different features and audiences. In this sub-section, we describe each platform and provide some comparisons across the platforms.[^2]

[^2]: Apart from the major U.S. based platforms, there is a growing interest in investor social media platforms from other countries — e.g., Feng and Johansson (2019), Sui and Wang (2022), Lee and Zhong (2022) and Leung and Ton (2015) who study Sino Weibo (China), Snow Ball (China), Interactive Investor Platforms (China), and Hot Copper (Australia) respectively.

#### 2.2.1 Seeking Alpha

Seeking Alpha, which was founded in 2004, is one of the older modern social media platforms geared specifically towards finance audiences: investors and market analysts (e.g., Grennan and Michaely, 2021). A distinguishing feature of Seeking Alpha is that it has an editorial team, which moderates comments and reviews submitted articles for quality before they are posted. The editorial team also ensures that the platform covers a wide range of stocks and topics of interest to investors. The posts on Seeking Alpha tend to be relatively long articles conducting in-depth analysis on single stocks, industries, or macro-economic issues. Articles on Seeking Alpha tend to receive many comments from readers. Figure 2 plots the monthly numbers of unique users and messages from January 2005-December 2023 for Seeking Alpha. The number of unique contributors and messages peaked around 2015, slowly declining thereafter. The number of messages (which includes comments), briefly spiked in 2020 with the influx of retail investors during the COVID lockdown period.

### Figure 2: Seeking Alpha over Time

**Caption:** This figure plots the number of monthly unique contributors and number of monthly messages (articles + comments) on Seeking Alpha from January 2005 - December 2023.

**Description (from visible figure labels):** A dual-axis line chart from Jan-05 to Oct-23. Left axis: "Number of unique Users" (0 to 1,600); right axis: "Number of Messages" (0 to 250,000). Series: "Unique Number of Users" (dashed) and "Number of Messages" (solid).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

#### 2.2.2 X (formerly known as Twitter)

X is a general interest social media platform that was founded in 2006 under the name Twitter and was renamed X in 2022. It quickly became one of the most prominent social media platforms for public discussions on a wide range of topics, with an outsized participation of journalists and leaders in technology and business. Active stock-specific discussions on Twitter started to emerge around 2010.

X consists of short-form messages, commonly referred to as tweets. Users can post tweets of up to 140 characters, later expanded to 280. With the launch of the premium Twitter Blue service, subscribers can post messages of up to 4,000 characters; such long messages remain rare.

While most conversations on Twitter are unrelated to finance or investing, there is a growing number of investors who use "cashtags" with the stock ticker symbol (e.g., "\$AAPL") to link a post to a specific company. The main function of the cashtag is to incorporate the message into a conversation about the company's stock via a hyperlink in the post. Figure 3 (a) plots the number of finance-specific messages over time for Twitter/X, StockTwits, and Reddit's WSB. Each timeseries is scaled to be between 0 and 100, and the maximum values are plotted in subfigure (b). The data for Twitter start in 2011, and the number of tweets increases gradually until the early part of the pandemic, which featured large spikes in 2020 and in 2021 (around the GameStop short squeeze). However, as subfigure (b) demonstrates, both Reddit's WSB and StockTwits had many more messages at their maximum. Figure 4 plots the unique number of users per month on each platform. Similar to the number of messages, the number of unique users who talk about stocks increased in 2016 and then peaked in 2023.

### Figure 3: Number of Messages over Time

**Caption:** This figure plots the number of monthly messages on StockTwits, Twitter, and Reddit's WSB (posts and comments). In subfigure (a) the number of messages are scaled to have maximum = 100 within each time series. Subfigure (b) plots what number of messages the 100 values correspond to.

**Panel (a): Scaled Number of Messages over Time.** Line chart from Jan-10 to Jul-23, y-axis 0 to 120, with series StockTwits, Twitter, and Reddit (WSB).

**Panel (b): Maximum Number of Messages.** Bar chart, y-axis 0 to 8,000,000, with bars for StockTwits, Twitter, and Reddit (WSB).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure 4: Number of Unique Monthly Users over Time

**Caption:** This figure plots the number of unique monthly contributors on StockTwits, Twitter, and Reddit's WSB. In subfigure (a) the number of contributors are scaled to have maximum = 100 within each time series. Subfigure (b) plots what number of contributors the 100 values correspond to.

**Panel (a): Scaled Number of Monthly Users over Time.** Line chart from Jan-10 to Jul-23, y-axis 0 to 120, with series StockTwits, Twitter, and Reddit (WSB).

**Panel (b): Maximum Number of Monthly Users.** Bar chart, y-axis 0 to 1,000,000, with bars for StockTwits, Twitter, and Reddit (WSB).

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

#### 2.2.3 StockTwits

StockTwits is the largest finance-specific social media platform. The website has a format similar to Twitter, where participants post short messages and reference specific assets using cashtags. StockTwits was the first platform to introduce the cashtag notation, which Twitter incorporated in 2012. The character limit started out as 140 and was later increased to 1,000 characters (Cookson, Lu, Mullins, and Niessner, 2024). According to the website analytics tool Alexa, StockTwits was ranked as the 505th most popular website in the US as of June 2021. As Figures 3 and 4 demonstrate, StockTwits usage increased sharply in 2020, peaking in 2021, and then decreasing slightly. In 2021, the number of monthly messages was approximately 5 million and the monthly number of unique active users exceeded 300,000. Interestingly, while the maximum number of messages on StockTwits is much higher than on Twitter, StockTwits only has around a third of the users. This suggests that users on StockTwits are more active, whereas Twitter users are less likely to write about stock investing.

#### 2.2.4 Reddit's WallStreetBets

Reddit's WallStreetBets (WSB) subreddit is a forum where participants discuss stock, crypto, and option trading. The forum gained prominence for its role in the GameStop trading frenzy in early 2021. Because WSB is a forum, the conversation is less structured around discussions of specific securities than the other finance-specific platforms. Individual stocks are often referenced by company name or ticker and are not followed by a cashtag. The character limit for posts is 40,000, even though most posts are quite short. Contributors do have an option to write a 'Due Diligence' post, which tend to be longer, in-depth analyses like those on Seeking Alpha (Bradley, Hanousek Jr, Jame, and Xiao, 2024). The remaining posts tend to be short, similar to StockTwits and Twitter. Unlike StockTwits and Twitter, comments on posts are only accessible via the original post, which creates a forum thread. Figures 3 and 4 plot the number of messages and unique WSB users from its inception in January 2013. In both Figures, usage peaked in late 2020 and early 2021, before decreasing substantially. The maximum unique number of users is similar to StockTwits, whereas the maximum number of messages per month is higher, hitting a maximum of just over 7 million messages per month in early 2021.

### 2.3 Data Sources for Social Media

Unlike traditional media, where many newspapers have put up paywalls over time, social media platforms tend to be publicly viewable without requiring a paid account. Historically, finance-specific social media platforms were also open to sharing data directly with researchers. StockTwits gave researchers free access to their API, as did Twitter and Reddit. However, coincident with the advent of Large Language Models (LLMs), social media websites have removed open access to their information. LLMs are data hungry, and social media companies have responded to a rise in the value of their historical data by putting it behind paywalls.[^3] StockTwits stopped sharing data with academic researchers in 2022, X (formerly Twitter) cut off academic API access in June 2023, and Reddit severely curtailed API access over the course of 2023.

[^3]: The retreat of social media platforms behind paywalls has been linked to AI by the platforms themselves (e.g., see coverage of Reddit in the NYT Isaac, 2023)

As direct access to data from social media platforms has become more difficult, some data vendors have begun organizing data from social media sources in their subscription services, which are available for academic research. For example, Ravenpack offers event and article-level sentiment scores for Seeking Alpha. While blog-like social media sources are easier to analyze and provide at the article level, other vendors offer signals for StockTwits and Twitter at the day-stock level. Some of the vendors that have shared this data with researchers include Context Analytics (formerly SMA) and MarketPsych (now part of Refinitiv), while Bloomberg also has a related product for subscribers (Bloomberg Social Velocity).

Other research in social media and finance has progressed by working with trading platforms that incorporate social features. For example, Heimer and Simon (2015) and Heimer (2016) use data from a platform focused on foreign exchange trading; other research employs data from eToro (Heimer, Iliewa, Imas, and Weber, 2024; Kogan, Makarov, Niessner, and Schoar, 2024). Such collaborations have proven fruitful in other research projects (e.g., Ammann and Schaub, 2021). Trading platforms with social features offer the opportunity to connect trading decisions and social interaction at the individual level.

Academic websites are also a source for social media data, processed in various ways. For example, data is available on the authors' websites for the following papers: Cookson and Niessner (2020) (firm-day StockTwits disagreement and attention data extended through 2021)[^4]; Baker, Bloom, Davis, and Renault (2021) (daily policy uncertainty index derived from the Twitter content); Chen and Hwang (2022) (firm-day Twitter attention and retweet data, 2013-2018); Müller and Schwarz (2023) (county-level number of Twitter users and South by Southwest participants); Cookson, Engelberg, and Mullins (2020) (daily StockTwits sentiment by political party of user, 2017-2020); Cookson, Engelberg, and Mullins (2023) (StockTwits firm-day information siloing and self-stamped disagreement data 2013-2020); Cookson et al. (2024) (firm-day principal components of sentiment and attention across platforms 2012-2021).

[^4]: Cookson and Niessner (2023) shows that this measure performs well outside of the original sample frame (both for a broad cross-section of firms and for over a decade of daily data). Recent research employs these measures in studies of gradual information diffusion via social networks (e.g., Hirshleifer, Peng, and Wang, 2024).

### 2.4 Contrasting Social Media with Traditional Signals

The rise of social media platforms is part of a broader phenomenon known as the "democratization of information production," as regular investors produce the information on these platforms. As a result, the information generated by these platforms tends to convey different information to that available in traditional media. While the information content can be hard to measure directly, the sentiment of financial social media (i.e., the average tone of posts, bullish versus bearish) is quite different to that in traditional financial media. While social media platforms have strongly positive sentiment (with around 80% bullish posts),[^5] research into traditional media highlight its more negative tone (Tetlock, Saar-Tsechansky, and Macskassy, 2008; van Binsbergen, Bryzgalova, Mukhopadhyay, and Sharma, 2024). The difference might be because investors tend to turn to social media platforms for investment advice, and because retail investors are mostly long-only, they pay attention to stocks that they are bullish about. By contrast, individuals turn to traditional media for news, and because conventional wisdom suggests that readers are more likely to read more negative news, journalists – including financial journalists – are incentivized to cover news that tilts negative (Niessner and So, 2024; Cookson, Garcia, and Jarnecic, 2024).

[^5]: The bullish tilt of sentiment has been shown in different samples: StockTwits (Cookson and Niessner, 2020; Cookson et al., 2023; Lopez Avila, Martineau, and Mondria, 2023), Seeking Alpha (Dim, 2023), and Twitter (Müller, Pan, and Schwarz, 2023).

It is also useful to contrast social media "investment research" with more traditional investment research, typically research reports produced by sell-side analysts (e.g., Drake, Moon Jr, Twedt, and Warren, 2023). Unlike sell-side analysts, who often have conflicts of interest, social media evaluations of firms are less likely to be intertwined with the firm. On the other hand, there is greater scope for behavioral biases in social media forecasts (Da, Huang, and Jin, 2021). Researchers have examined these issues across social media platforms. For example, the forecasting platform Estimize has been benchmarked to traditional investment research (Jame, Johnston, Markov, and Wolfe, 2016; Da and Huang, 2020; Jame, Markov, and Wolfe, 2022; Schafhäutle and Veenman, 2024). This research suggests that crowdsourced information on social media provides information beyond the signal extracted from more traditional analyst reports.

## 3 Social media as a lens

An important theme of the literature on social media in finance is the use of social media as a lens to study general economic and financial phenomena, under the view that social media is — in many ways — a microcosm of the broader information environment. This research has contributed insights into classic research questions about how investors update beliefs, the measurement and consequences of investor disagreement, and even how social networks transmit information. It is distinctive that this line of research does not necessarily propose that social media itself has direct effects on financial markets. Rather, this research uses public signals from social media to provide insight into general economic phenomena. This section reviews several of the major areas where this approach has proven fruitful.

### 3.1 Investor beliefs and disagreement

Investors on social media platforms declare their beliefs about individual stocks and the broad market at high frequency, such that belief measures can be constructed at the daily and intra-day levels. Due to reputation-building incentives (together with the inability to delete posts on some platforms), these publicly stated beliefs tend to be a useful reflection of what investors truly believe. A key advantage of high frequency information about beliefs is that it allows researchers to examine investors' response to individual pieces of financial news, in contrast to survey-based measures that are typically updated monthly or quarterly, or to sporadically-updated analyst forecasts, typically studied at the quarterly level.

The literature has employed daily disagreement measures drawn from social media in a variety of contexts. Using the dispersion of bullish versus bearish sentiment about securities on StockTwits, Cookson and Niessner (2020) examines the differences between model-based and information-based disagreement. The article shows that disagreement among people with the same investment philosophy (i.e., employing the same "model," based on StockTwits profile information) is more closely related to trading volume than is disagreement across differing investment approaches. In work that also employs data from StockTwits, Giannini, Irvine, and Shu (2019) measures the disagreement between the sentiment on investor social media and in traditional media around earnings announcements. In so doing, they shed light into how opinions can converge or diverge around the arrival of information, which is central to the literature on belief updating. Hirshleifer et al. (2024) employs a disagreement measure drawn from StockTwits, finding that disagreement persists after earnings announcements, especially in areas with more social transmission of ideas.

Another strand in this literature examines how the beliefs of different types of investors — measured on StockTwits — evolve around major events. Cookson et al. (2020) shows that a partisan gap in investor beliefs emerged around the onset of the Covid-19 pandemic: Republicans remained bullish, in contrast to other investors who became markedly more pessimistic. The article rules out most non-partisan channels, including showing that Republican investors were more optimistic about most stocks except Chinese stocks, after anti-Chinese sentiment became a Republican-identified view. Moreover, the paper shows a tight connection between partisan disagreement and abnormal turnover in the cross-section of stocks. In a series of asset pricing tests, Sheng, Sun, and Wang (2023) employs StockTwits data to show that partisan differences in sentiment can underpin a partisan return gap in which firms favored by Republican investors outperformed firms favored by Democrats during the Covid-19 Pandemic.

### 3.2 Information sources and attention

Social media has also been used as a lens in the study of financial information sources. Social media data frequently contain details about investors' information exposure, as well as their beliefs. For example, a social media user who follows someone makes a decision to place that person's future posts into their feed, shaping their information set. Similarly, users of social media can specify watch lists, which place information about specific stocks into their feed. This literature focuses on both the consequences of investor attention, but also what drives investor attention to one information source versus another.

A major point of emphasis in this broader literature is to measure and understand the implications of attention (see Barber and Odean, 2008; Da, Engelberg, and Gao, 2011; deHaan, Lawrence, and Litjens, 2024; Da, Hua, Hung, and Peng, 2023). Outside of social media, insights into financial attention have been drawn from data on accessing 10-Ks on EDGAR (Drake, Roulstone, and Thornock, 2015), data on logins which show whether users are paying attention to market information (Sicherman, Loewenstein, Seppi, and Utkus, 2016; Gargano and Rossi, 2018), and from data on the timing of Google searches for a stock's ticker (Ben-Rephael, Carlin, Da, and Israelsen, 2021). Within social media, a natural measure of investor attention is the volume of messages or the relative volume of messages posted about some stocks versus others (e.g., Irvine, Shen, and Shu, 2021; Cookson et al., 2024). Moreover, as a result of the sustained growth of investor social media activity over the past decade, stock coverage from these sources encompasses a larger set of firms than those covered by traditional news sources.

Another aspect of the attention literature is the effort to understand what information investors are consuming and how this can shed light onto other economic phenomena. In this respect, social media contains abundant information on the content of posts and users' interactions with them, as well as users' following choices. For example, even in the absence of data on user impressions, if a user likes, retweets, or replies to a post, then the user must have consumed the information in that post. Chen and Hwang (2022) shows that readers of Seeking Alpha posts selectively share them with their personal networks, and discusses implications of selective sharing on the kinds of information investors can expect to see.

Beyond measuring attention and information consumption, social media data on watchlists and follower links can also be used to study how attention itself arises. Modern social media displays information to users in the form of a newsfeed or a collection of recent posts by people or stocks that the user has chosen to follow. Using micro-data on users' following choices, Cookson, Engelberg, and Mullins (2023) documents that users disproportionately follow users who have recently expressed an opinion similar to their own. Since users are persistent in their sentiment about individual stocks over time, the choice to follow like-minded people leads to newsfeeds that reflect users' own prior beliefs — echo chambers. These investor social media echo chambers reduce the variety of information that users see, are related to more trading (likely via increased investor disagreement), and appear to reduce investor returns. Cookson, Engelberg, and Mullins (2023) also provides evidence for a mechanism relevant to the disagreement literature: earnings announcements push users further into their echo chambers, making it more difficult for beliefs to converge. In a similar vein, Levy, Rossi, Shalev, and Zur (2023) examines how Seeking Alpha watchlists are formed and how they relate to price impacts of news. As a stock is included in more watchlists, prices become more sensitive to news without incorporating information more rapidly, reflecting an increase in volatility.

Others have employed likes, retweets, and comments to measure different kinds of information consumption. For example, Alsabah (2024) makes the case that anti-firm sentiment can be captured by whether a firm's non-financial tweets are "ratioed" (i.e., if quote tweets and comments are high relative to retweets and likes), and affects the price reaction to earnings surprises.[^6]

[^6]: In a closely related setting, Da and Huang (2020) study decentralized analyst forecasts on the platform Estimize, finding wisdom of crowd effects similar to those found in the social media literature. This setting also sheds light onto biased belief formation: Da et al. (2021) studies extrapolation in the cross-section.

### 3.3 Social networks

An important strand of the literature uses the connections formed on social media to proxy for in person social networks. This research has antecedents in the broader literature on social economics (Becker, 1974, 1991) and social networks (Jackson and Wolinsky, 2003; Jackson et al., 2008). Indeed, online social platforms provide an abundance of data on connections between people and how these were formed, enabling the analysis of social network mechanisms that would otherwise be unobservable. Kuchler and Stroebel (2021) describes recent developments in this social networks literature, many of which stem from social media revealing both social connections and social interactions.

The introduction of detailed data on Facebook connections at the individual level (Bailey, Cao, Kuchler, and Stroebel, 2018) and between geographic areas (Bailey, Cao, Kuchler, Stroebel, and Wong, 2018) has encouraged new research into social economics, and has allowed the literature to understand mechanisms related to asset pricing. For example, Bailey et al. (2018) uses social connections on Facebook for every user in Los Angeles county to estimate how their friends' house price experiences translate into real estate purchase and valuation decisions. Using the difference between buyers' and sellers' network connections, the article shows that exposure to house price changes through social networks matters for how households form expectations.

Beyond the housing market, these social connections data from Facebook have been employed to study a wide variety of economic phenomena, such as institutional investing patterns (Kuchler, Li, Peng, Stroebel, and Zhou, 2022), economic mobility and socioeconomic status (Chetty et al., 2022a,b; Cannon, Hirshleifer, and Thornton, 2024), urban agglomeration (Bailey, Farrell, Kuchler, and Stroebel, 2020), international trade (Bailey, Gupta, Hillenbrand, Kuchler, Richmond, and Stroebel, 2021), social connection and disease transmission (Charoenwong, Kwan, and Pursiainen, 2020; Bailey, Johnston, Koenen, Kuchler, Russel, and Stroebel, 2024), and transmission of beliefs about stock prices (Hirshleifer et al., 2024).

While Facebook is not primarily an investor social platform, other research has adopted a similar approach toward studying the impacts of social networks that are finance-specific. For example, Cookson, Engelberg, and Mullins (2023) studies network formation — via users' decisions regarding whom to follow — and its relation to prior beliefs, showing sentiment homophily (Jackson et al., 2008). Another example of this kind of research is Cookson, Fox, Gil-Bazo, Imbet, and Schiller (2023), which employs detailed data from Twitter during the run on Silicon Valley Bank to highlight the importance of communication via social networks for banking stability during the 2023 Regional Banking Crisis.

### 3.4 Other uses of social media as a lens

Financial social media has been used to shed light on underlying economic behavior in a variety of other settings.

**Trust in information sources.** Market manipulation and trust in financial markets has been an active area of research for many decades (e.g., Knack and Keefer, 1997; Sapienza and Zingales, 2012). However, little evidence exists of how trust evolves in markets and indirect consequences of changes in trust. Kogan, Moskowitz, and Niessner (2023) uses an SEC investigation into fake news on Seeking Alpha as a shock to market participants' awareness of fraud and trust in the news source. They find that this shock caused market participants to discount all news from Seeking Alpha and The Motley Fool, including legitimate news. This result highlights that if market manipulation can affect U.S. equity markets, which tend to be informationally efficient, it could have even greater influence in settings where information costs are higher and the ability to correct misinformation is more limited (e.g., online consumer or political markets).

**Interactions among different types of investors in market equilibrium.** A classic stream of literature aims to understand the market interactions of different investor types, and is central to models of market clearing and informed trade (e.g., Kyle, 1985). Cookson, Fos, and Niessner (2022) is an example of research that uses social media to study interactions between sophisticated and unsophisticated traders. It explores how informed traders — activists and short sellers — trade in the presence of unsophisticated disagreement, measured using disagreement on StockTwits. Informed buyers and sellers are attracted to stocks with high disagreement because these stocks have greater liquidity. However, informed buyers are discouraged by high disagreement, since disagreement with shorting constraints can drive up prices and lead to overvaluation.

Another contribution in this vein is Ben-Rephael, Cookson, and Izhakian (2024), which shows that disagreement's relation to trading is stronger when there is less ambiguity (Knightian uncertainty) in a firm's trading environment. This result shows that ambiguity places a wedge between disagreement and trading decisions, echoing findings showing that household portfolios display only a weak response to changes in beliefs (e.g., Ameriks, Kézdi, Lee, and Shapiro, 2020; Giglio, Maggiori, Stroebel, and Utkus, 2021).

**Home bias.** Social media can also contain geographic information on its users, which Giannini, Irvine, and Shu (2018) uses to provide evidence on the poor performance of sentiment measured from the messages of non-local investors, relative to investors who are local to a firm's activities — novel evidence on a source of home bias. Such geographic information could potentially be employed in other empirical settings where information diffusion via in-person networks is important.

**Viewpoints of prominent economic agents.** The precise time-stamps of investor social media posts have also been used, together with high frequency price data, to provide better identification about how viewpoints and beliefs shape economic outcomes. Bianchi, Gómez-Cram, Kind, and Kung (2023) develops this approach to study the impact of presidential tweets about the Federal Reserve on financial markets and central bank independence. Relatedly, Bianchi, Cram, and Kung (2023) applies this empirical design to show how firms are affected by Congressional pressure via Twitter. In a different context, Cookson et al. (2023) uses this approach to show that tweets by 'tech Twitter' users had immediate market impacts during the 2023 run on Silicon Valley Bank.

Outside of social media sentiment and attention focused on firm outcomes, social media can be used to form a signal for other important economic phenomena. For example, Born, Dalal, Lamersdorf, and Steffen (2023) collect information from German-language Twitter to generate a high frequency measure of German inflation. Similarly, Baker et al. (2021) construct an economic policy uncertainty index from the text of English language tweets and tweets that originate from the United States. Bhagwat, Dim, Shirley, and Stark (2023) and Blankespoor, Pinto, and Sinha (2024) study gender bias in financial markets through the lens of Seeking Alpha. They find that investors on Seeking Alpha react more negatively to posts by female contributors and provide more negative opinions about female-led firms.

Although financial research using social media platforms emerged as a means to study broader economic phenomena, social media's rapid growth has led to important changes in how we interact. We now turn to the growing literature that studies the effects of social media itself on financial markets.

## 4 The effects of investor social media

Social media has moved beyond its initial role as a leisure activity (Pew Research Center, 2023), and is now a major arena for social interactions and for sharing and consumption of news. As a result, it has become important unto itself, altering the channels of social communication as well as facilitating extremist behavior (e.g., Müller and Schwarz, 2021; Braghieri, Levy, and Makarin, 2022; Acemoglu, 2022; Müller and Schwarz, 2023; Lu and Sheng, 2022).

Mirroring the broader literature on the economics of social media (see Aridor, Jiménez-Durán, Levy, and Song, 2024, for a review), an increasingly important strand of research in investor social media has studied the impact of social media on financial outcomes. This work concerns itself primarily with how social media affects the information environment and how these effects have evolved as social media has become more important. To understand social media's effects, it is useful to recognize both when social media became important and social media's distinctive features in comparison to those of traditional media. Thus, we begin by describing the emergence of modern financial social media.

### 4.1 Modern social media's emergence and distinctive features

Finance-specific social media has grown substantially since the early 2000s. Although social media is a recent technology, early versions — online investor forums and message boards — existed over a decade before Twitter or StockTwits were founded. The early literature investigating these questions (notably Antweiler and Frank, 2004) asked whether the conversations on social media contained useful information or were mostly noise, and concluded that differences in opinions on message boards translated into trading, but information from message boards didn't appear to move markets. However, financial social media changed radically over the past 15 years, with new finance-specific social media platforms, and explosive growth in both the amount of posted content and the number of users actively engaged on these platforms (as we highlight in Figures 2, 3, and 4).

Aside from the increases in participation and content, social media platforms have also changed qualitatively. For example, users have moved to platforms that encourage viral content — i.e., information that is reshared widely beyond one's immediate personal network (Van Bavel, Rathje, Harris, Robertson, and Sternisko, 2021). Relative to message board technology, social platforms with these features have much greater potential to coordinate ideas because each post has greater potential reach and can be much more quickly retransmitted. As a result of emotional content's higher propensity to become viral (Berger and Milkman, 2012), social media tends to amplify emotional narratives while de-emphasizing hard information. In a financial context, the tendency of social media to amplify viral content can have important implications for economic narratives (Shiller, 2017; Hirshleifer, 2020), which can lead to bubbles and other market inefficiencies (e.g., Pedersen, 2022; Chinco, 2023; Bali, Hirshleifer, Peng, and Tang, 2023).[^7]

[^7]: Campbell, Drake, Thornock, and Twedt (2023) studies when earnings announcements go viral on Twitter, finding that these episodes coincide with less liquid markets and with slower price formation.

A related trend in social media is the increasing use of non-textual content: pictures, emojis, videos (Fox, Kelley, and Paolucci, 2023; Hu and Ma, 2023; Blankespoor, Hendricks, and Miller, 2017; Gu, Teoh, and Wu, 2023). Appealing to the idea that a picture is worth a thousand words, their increasing use has allowed social media users to more easily create content that appeals to emotions.

All told, the increasing popularity of financial social media, together with its new features, raises interesting questions about the information content on social media, its evolution over time, and its informativeness for other market participants (e.g., firms and other investors). It is also unclear whether the features of social media are all beneficial innovations. In the subsequent sections, we describe research streams and potential future research along the lines of each of these key ideas.

### 4.2 Is there a signal in social media?

Since the earliest online message boards, scholars have investigated whether there is information content in social media posts (e.g., Antweiler and Frank, 2004). As social media data and the unstructured text of social media posts became more widely available, scholarly and practical interest emerged around the development of an informative social media signal via natural language processing. Investor social media and its relation to financial market outcomes became a natural testing ground for new machine learning methods (e.g., Das and Chen, 2007; Acemoglu, 2022; Sohangir, Petty, and Wang, 2018; Araci, 2019, for early sentiment extraction, the development of VADER, application to StockTwits, and FinBERT, respectively).

The finance literature has studied the social media sentiment signal for at least a decade. Chen, De, Hu, and Hwang (2014) shows that negative tone in Seeking Alpha articles and in the associated comments predict negative market performance and earnings surprises for up to three months. In a similar vein, Avery, Chevalier, and Zeckhauser (2016) finds strong evidence of informativeness on the social platform CAPS (part of The Motley Fool), which is mostly driven by negative stock picks. Other research explores the information content of social media platforms at different horizons. For example, Renault (2017) shows that StockTwits sentiment is informative of intraday price movements; Bartov, Faurel, and Mohanram (2018) shows Twitter can predict imminent earnings announcement returns; while Cookson and Niessner (2020) shows that professional sentiment on StockTwits, at the daily level, predicts positive returns for at least 60 days.

Although there are many settings where social media is informative of future price movements, recent work has shown that market events may affect this informativeness. For example, Bradley et al. (2024) shows that 'Due Diligence' reports on Reddit's WallStreetBets forum used to be strongly and positively informative of future returns. However, after the GameStop short squeeze, these reports became uninformative, mostly driven by reports advocating positions against short sellers. Cookson, Lu, Mullins, and Niessner (2024) finds a similar deterioration of the informativeness of StockTwits sentiment after GameStop, and shows that this deterioration was driven by users who recently joined the platform. More broadly, Cookson, Lu, Mullins, and Niessner (2024) highlights the importance, for the informativeness of investor social media sentiment, of differences in user populations and platform features, consistent with communication theory (McLuhan, 1975).

In a similar vein, recent research has employed social media sentiment data to investigate the degree to which social media users display heterogeneous skill in forecasting future returns. Dim (2023) shows that only 13% of Seeking Alpha authors exhibit high skill: following the recommendations of these users earns risk-adjusted returns of 61 basis points per week. Using StockTwits data through 2016, Kakhbod, Kazempour, Livdan, and Schuerhoff (2023) employs a similar method to find that forecasts made by skilled users on StockTwits have some predictability. These findings echo reduced form evidence in Cookson and Niessner (2020) showing that professional sentiment on StockTwits positively predicts future returns while novice sentiment negatively predicts returns, consistent with evidence on retail investor returns from trading (Coval, Hirshleifer, and Shumway, 2021).[^8] Although one conclusion of this research is that sentiment from a subset of skilled or sophisticated users on social media appears informed, another takeaway is that there is major heterogeneity across users. As detailed information on the identities of social media participants become available (e.g., Cookson, Engelberg, and Mullins, 2020, measures partisanship at the individual level), there is significant scope for understanding this heterogeneity in social media sentiment and its market implications.

[^8]: Apart from variation in the sentiment signal across different types of users, variation in the credibility of the signal matters as well: Campbell, DeAngelis, and Moon (2019) show stronger return predictability of articles in which Seeking Alpha authors disclose a position in the stock.

An under-appreciated dimension of the signal from social media is that tweets, likes, and retweets reflect attention to a particular security. This is an important aspect of the signal because attention motivates social media participation (e.g., see field experiment in Srinivasan, 2023). In the financial domain, Cookson, Lu, Mullins, and Niessner (2024) highlights the difference between social media sentiment and attention, showing that the return dynamics following high attention versus high sentiment are quite distinct. After high-attention days, which tend to coincide with run-ups in stock prices, returns revert for up to 10-15 days; however, there is no reversion following high-sentiment days. Lopez Avila et al. (2023) studies the role of social media attention around earnings announcements, and finds that earnings announcements in the presence of high StockTwits attention are not consistently more efficient in their incorporation of earnings news into prices. Ongoing research by Irvine et al. (2021) investigates the differences between social media attention and what would be predicted via a rational benchmark. Given social media attention's potential market impacts, it would be valuable to see more work investigating how such attention is formed.

New technologies and ways of communicating have the potential to change the nature of the social media signal. For example, as social media becomes more video-based or uses non-word tokens like emojis (Fox et al., 2023), non-textual communication — such as intonation, facial expression, and excitability — may become more important (Hu and Ma, 2023). At the same time, these new forms of communication provide more context and detail, which may contribute to a more informative signal (e.g., see the model in Martel, Van Wesep, and Van Wesep, 2022). Evidence on the differences between video and textual content is emerging; initial studies suggest such content is more persuasive on non-informational dimensions (Hu and Ma, 2023; Blankespoor et al., 2017) and can facilitate coordination (Gu et al., 2023). As these technologies grow within the social media space, their implications deserve more attention.

The rise of artificial intelligence (AI) and large language models (LLMs) also has great potential to shape future research on social media in finance. Sophisticated sentiment classifiers are easier to develop via LLMs (e.g., see work by Chen, Peng, and Zhou (2024)), but how the social media signal will be affected by the introduction of new AI models is an important open question. Will social media information become more siloed as private companies protect it using paywalls? Will AI tools reduce or enhance biases in social media signals? These potential changes to the social media ecosystem present exciting new possibilities for academic research.

### 4.3 Social media and informational efficiency

It is important to understand how financial social media affects the overall financial information environment. This relates to the more general question of whether, as data become more abundant, markets become more informative (Bai, Philippon, and Savov, 2016; Farboodi, Matray, Veldkamp, and Venkateswaran, 2022). Given the tension in the broader literature, it is natural to wonder if financial social media, as an abundant but noisy source of data on retail investors, increases or decreases the noise in the information environment, and how this feeds through to market equilibrium outcomes (Dugast and Foucault, 2018).

Whether social media helps or hurts market efficiency is still an open question. Dessaint, Foucault, and Frésard (2024) shows that social media's rise in the mid-2010s coincided with an improvement in the quality of short-horizon analyst forecasts but not for long-horizon forecasts by the same analysts. Since social media information tends to contain information relevant to shorter horizons, this suggests that social media plays a useful role in informing analyst forecasts. Complementary to this idea, Cookson, Niessner, and Schiller (2024) shows that reactions on social media to merger announcements predict merger withdrawals, and this predictability is unexplained by return reaction, analyst updates, learning through managers' networks, or traditional news. In other words, information from social media appears to be a useful signal of corporate decisions. Relatedly, Ang, Hsu, Tang, and Wu (2021) finds that sentiment on a Chinese internet stock message board is predictive of future merger withdrawals when the mergers are negative NPV.

The firms that are most likely to see improvements in information environment due to social media's rise are smaller firms. Such firms are largely ignored by traditional media, but social media often provides in-depth coverage. Cookson, Lu, Mullins, and Niessner (2024) provides statistics on coverage by firm size and also shows larger price impacts for small firms. Future research would do well to examine the real impacts of social media on the firms whose information environment is most affected.

Firms themselves are not passive with respect to social media. They often maintain Twitter and Facebook accounts, which they use actively to communicate with investors and customers. For example, Wolfskeil (2020) shows that firms tend to tweet more using a positive tone around earnings announcements with negative surprise. Blankespoor, Miller, and White (2014) finds that, at least for tech firms, usage of Twitter to disseminate financial disclosures leads to lower bid-ask spreads, consistent with reduced information asymmetry. Firms can also use social media strategically: Lee, Hutton, and Shu (2015) shows that social media disclosures by firms can dampen negative reactions to consumer product recalls. Mkrtchyan, Sandvik, and Zhu (2023) shows that social media is increasingly used as a forum for CEO activism around social issues, with implications for firm value. Firms' social media disclosures are not restricted to their own firm: Cao, Fang, and Lei (2021) finds that firms also use social media to highlight negative information about their competitors, which has a negative effect on competitors' stock prices.

### 4.4 Concerns about social media

With the democratization of information production through social media comes the risk that social media disseminates incomplete, inaccurate or even false information.

**Rumors and information distortion.** Information on social media often takes the form of rumors and non-verifiable information. As more people rely on social media for their news, it is inevitable that distorted views will be spread (e.g., Jia, Redigolo, Shu, and Zhao, 2020; Kogan, Moskowitz, and Niessner, 2023), stemming from biased beliefs or malicious intent. Understanding social media's role in such misinformation is an active area of research.

Social media often generates siloed information environments or echo chambers in which like-minded people follow one another (Cinelli, De Francisci Morales, Galeazzi, Quattrociocchi, and Starnini, 2021; Cookson et al., 2023). Users on social media frequently selectively share information for impression management purposes (Chen and Hwang, 2022). Capturing a different aspect of biased sharing, Cassella, Dim, and Karimli (2023) uses data from The Motley Fool's CAPS platform to shed light onto how investors maintain optimism by shifting their investment horizon further into the future after seeing news that contradicts their priors. The propensity to update in a way that is favorable to one's own prior is a general phenomenon seen outside of social media (Kapons and Kelly, 2023), but given the structure of social media and the rewards from garnering attention (Srinivasan, 2023), these biases may be more pronounced in social media settings.

Selective sharing and selective sourcing of information on social media are complementary parts of social transmission bias, an idea central to the emerging social finance literature described in Hirshleifer (2020) and further explored in Heimer and Simon (2015), Akçay and Hirshleifer (2021), and Han, Hirshleifer, and Walden (2022). Recent work has turned to social media as a venue to observe both the beliefs users express and the beliefs in their newsfeed in order to quantify how social networks distort the way investors share information with one another (e.g., Han, Liu, and Sui, 2023; Sui and Wang, 2022).

There are many other studies on the social transmission of beliefs, examining how social forces lead to biased expectations. For example, Bailey et al. (2018) shows how Facebook connections transmit distorted house price expectations, changing housing market behavior. Similarly, as people become more exposed to social media, their behaviors tend to be more distorted (Heimer, 2016). However, in some cases, social network sharing can help those in need: Peng and Zhang (2024) highlights how social ties, captured through Facebook social media connections, can help crowdfunding campaigns. This work is complementary to Cookson, Gallagher, and Mulder (2023), which highlights the role of social networks and social sharing in contributing to disparities in crowdfunding outcomes by household incomes.

**Fake news and schemes.** Social media is concerning from an information standpoint because it can create and propagate "fake news" and false narratives about the market. Kogan, Moskowitz, and Niessner (2023) explores the prevalence of fake news on Seeking Alpha and evaluates the market consequences. They estimate a lower bound of approximately 1.5% of articles on Seeking Alpha contain fraudulent information. In subsequent work, Liu and Moss (2022) finds that fraudulent articles are especially common prior to earnings announcements when there is heightened attention on social media, but before hard information is released to the market. In a different context, Li, Shin, and Wang (2021) shows how coordinating around Telegram channels facilitates cryptocurrency pump-and-dump schemes.

An important aspect of schemes that harm the information environment is that they are often propagated by people with many followers. When people gain a following for reasons unrelated to their financial views, this can create distortions in the information on social media. Benetton, Mullins, Niessner, and Toczynski (2024) highlights this point in the context of real-world celebrities whose social media posts about major cryptocurrencies, like Bitcoin and Doge Coin, have notable effects on crypto markets. Using transaction-level data, they show that individuals react to these celebrity tweets as if they were financial advice. In related work, White and Wilkoff (2023) shows that celebrity endorsements of initial coin offerings affect how much money they raise.

While directly eliminating fraudulent or misleading information from social media is impractical, there are ways to mitigate its spread and impact. For example, Kogan, Moskowitz, and Niessner (2023) find that making the presence of fraudulent information on Seeking Alpha salient to investors diminishes their reliance on Seeking Alpha articles for making trading decisions. Future research would do well to examine ways to mitigate of reduce the spread of fraudulent information on social media platforms. [Conversion note: "mitigate of reduce" appears as printed in the source PDF; likely intended "mitigate or reduce". Preserved verbatim.]

**Democratization of finance.** Although retail investors have been a focus of the academic literature for nearly 30 years (Odean, 1998), the rise of social media has coincided with a significant shift toward more market participation by retail investors.

These new investors and their interactions on social media have had clear market impacts: for example, see the recent research on the market consequences of Robinhood investors (Barber, Huang, Odean, and Schwarz, 2022; Eaton, Green, Roseman, and Wu, 2022; Welch, 2022; Fedyk, 2023). Furthermore, different waves of entry into financial markets by retail investors, such as the influx of new investors during Covid-19, have been changing the informativeness of the social media signal over time (Cookson, Lu, Mullins, and Niessner, 2024). This influx of retail investors who source information via social media is a major part of the recent "democratization of finance," studied in Farrell, Green, Jame, and Markov (2022); Dim (2023). Although some of the initial research into this wave of new investors finds negative outcomes (Bradley et al., 2024; Barber et al., 2022), a bright side is that it may promote participation in financial markets themselves. Müller et al. (2023), for example, uses variation in early Twitter adoption to show that it increases stock market participation.

**Coordination and polarization:** The GameStop short squeeze phenomenon called attention to social media's coordinating role, and spawned research into the drivers and consequences of such coordination (Pedersen, 2022; Van Wesep and Waters, 2021; Li, 2022). Bradley et al. (2024) shows that previously-informative 'Due Diligence' reports on Reddit's WallStreetBets became uninformative after the short squeeze. In the context of non-fungible tokens (NFTs), Oh, Rosen, and Zhang (2024) shows how social forces — often played out on social media — can lead to unique coordination and pricing dynamics in NFT markets. Another important real consequence of coordination on social media is the possibility of coordinated and rapid bank runs fueled by social media: Cookson, Fox, Gil-Bazo, Imbet, and Schiller (2023) shows how social media can play a role in propagating fear among depositors in the context of the Silicon Valley Bank collapse.

Social media has long been thought to create information bubbles, or echo chambers, outside of finance. However, Cookson, Engelberg, and Mullins (2023) documents the prevalence of financial echo chambers (i.e., bears following bears, bulls following bulls) on social media, and shows that people who are in a more information siloed environment make lower quality stock market predictions. These echo chambers can create and sustain disagreement while slowing the impact of information, and due to the polarizing nature of social media, the disagreement can take a political tone. In line with this idea, Cookson, Engelberg, and Mullins (2020) shows how investor disagreement along political party lines emerged at the onset of the Covid-19 pandemic, leading to persistent disagreement and a rise in trading volume for months after Covid-19's onset in the U.S.

Building on these efforts, future research would do well to understand the features of social media that facilitate coordination among financial market participants, particularly when people coordinate around false narratives.

## 5 Conclusion

Social media has grown explosively over the past two decades. In this review, we discuss the burgeoning literature on social media in finance. Our review distinguishes between social media research that uses social media as a lens to answer broader finance questions and research that investigates the consequences of social media itself on financial markets.

Although this distinction may appear sharp in our review, the line distinguishing these two types of financial social media research is often less clear-cut. For example, is investors' propensity to place themselves into a financial echo chamber (Cookson et al., 2023) a natural tendency that would exist to the same extent irrespective of social media interactions, or do features of these platforms exacerbate echo chamber behaviors? In reality, social media both shapes us and reflects fundamental aspects of ourselves.

Going forward, sharpening this distinction has the potential to generate new insights into the financial economics of social media, especially as research grapples with novel formats and new ways to communicate within social media platforms.

## References

Acemoglu, D. (2022). The end of real social networks. Project Syndicate.

Akçay, E. and D. Hirshleifer (2021). Social finance as cultural evolution, transmission bias, and market dynamics. Proceedings of the National Academy of Sciences 118(26), e2015568118.

Alsabah, K. (2024). Love me do: Twitter likes and earnings surprise. Journal of Behavioral Finance, 1-20.

Ameriks, J., G. Kézdi, M. Lee, and M. D. Shapiro (2020). Heterogeneity in expectations, risk tolerance, and household stock shares: The attenuation puzzle. Journal of Business & Economic Statistics 38(3), 633-646.

Ammann, M. and N. Schaub (2021). Do individual investors trade on investment-related internet postings? Management science 67(9), 5679-5702.

Ang, J. S., C. Hsu, D. Tang, and C. Wu (2021). The role of social media in corporate governance. The Accounting Review 96(2), 1-32.

Antweiler, W. and M. Z. Frank (2004). Is all that talk just noise? The information content of internet stock message boards. Journal of Finance 59(3), 1259-1294.

Araci, D. (2019). Finbert: Financial sentiment analysis with pre-trained language models. arXiv preprint arXiv:1908.10063.

Aridor, G., R. Jiménez-Durán, R. Levy, and L. Song (2024). The economics of social media. CESifo Working Paper.

Avery, C. N., J. A. Chevalier, and R. J. Zeckhauser (2016). The "CAPS" prediction system and stock market returns. Review of Finance 20(4), 1363-1381.

Bai, J., T. Philippon, and A. Savov (2016). Have financial markets become more informative? Journal of Financial Economics 122(3), 625-654.

Bailey, M., R. Cao, T. Kuchler, and J. Stroebel (2018). The economic effects of social networks: Evidence from the housing market. Journal of Political Economy 126(6), 2224-2276.

Bailey, M., R. Cao, T. Kuchler, J. Stroebel, and A. Wong (2018). Social connectedness: Measurement, determinants, and effects. Journal of Economic Perspectives 32(3), 259-280.

Bailey, M., P. Farrell, T. Kuchler, and J. Stroebel (2020). Social connectedness in urban areas. Journal of Urban Economics 118, 103264.

Bailey, M., A. Gupta, S. Hillenbrand, T. Kuchler, R. Richmond, and J. Stroebel (2021). International trade and social connectedness. Journal of International Economics 129, 103418.

Bailey, M., D. M. Johnston, M. Koenen, T. Kuchler, D. Russel, and J. Stroebel (2024). Social networks shape beliefs and behavior: Evidence from social distancing during the Covid-19 pandemic. Journal of Political Economy: Microeconomics, Forthcoming.

Baker, S. R., N. Bloom, S. Davis, and T. Renault (2021). Twitter-derived measures of economic uncertainty.

Bali, T. G., D. Hirshleifer, L. Peng, and Y. Tang (2023). Attention, social interaction, and investor attraction to lottery stocks. NBER working paper.

Banerjee, A. V. (1992). A simple model of herd behavior. The Quarterly Journal of Economics 107(3), 797-817.

Barber, B. M., X. Huang, T. Odean, and C. Schwarz (2022). Attention-induced trading and returns: Evidence from Robinhood users. Journal of Finance 77(6), 3141-3190.

Barber, B. M. and T. Odean (2008). All that glitters: The effect of attention and news on the buying behavior of individual and institutional investors. The Review of Financial Studies 21(2), 785-818.

Bartov, E., L. Faurel, and P. S. Mohanram (2018). Can Twitter help predict firm-level earnings and stock returns? The Accounting Review 93(3), 25-57.

Becker, G. S. (1974). A theory of social interactions. Journal of Political Economy 82(6), 1063-1093.

Becker, G. S. (1991). A note on restaurant pricing and other examples of social influences on price. Journal of Political Economy 99(5), 1109-1116.

Ben-Rephael, A., B. I. Carlin, Z. Da, and R. D. Israelsen (2021). Information consumption and asset pricing. Journal of Finance 76(1), 357-394.

Ben-Rephael, A., J. A. Cookson, and Y. Y. Izhakian (2024). Do I really want to hear the news? Public information arrival, ambiguity and investor beliefs. Available at SSRN 3631760.

Benetton, M., W. Mullins, M. Niessner, and J. Toczynski (2024). Celebrity tweets: This is not financial advice. Working Paper.

Berger, J. and K. L. Milkman (2012). What makes online content viral? Journal of Marketing Research 49(2), 192-205.

Bhagwat, V., C. Dim, S. Shirley, and J. Stark (2023). Gender bias and crowd-sourced financial information. Available at SSRN 4669864.

Bianchi, F., R. G. Cram, and H. Kung (2023). Using social media to identify the effects of congressional viewpoints on asset prices. Review of Financial Studies, Forthcoming.

Bianchi, F., R. Gómez-Cram, T. Kind, and H. Kung (2023). Threats to central bank independence: High-frequency identification with Twitter. Journal of Monetary Economics 135, 37-54.

Bikhchandani, S., D. Hirshleifer, O. Tamuz, and I. Welch (2024). Information cascades and social learning. Journal of Economic Literature, forthcoming.

Bikhchandani, S., D. Hirshleifer, and I. Welch (1992). A theory of fads, fashion, custom, and cultural change as informational cascades. Journal of Political Economy 100(5), 992-1026.

Blankespoor, E., B. E. Hendricks, and G. S. Miller (2017). Perceptions and price: Evidence from CEO presentations at IPO roadshows. Journal of Accounting Research 55(2), 275-327.

Blankespoor, E., G. S. Miller, and H. D. White (2014). The role of dissemination in market liquidity: Evidence from firms' use of Twitter. The Accounting Review 89(1), 79-112.

Blankespoor, E., J. Pinto, and K. Sinha (2024). Toxic social media opinions and CEO gender. Available at SSRN.

Born, B., H. Dalal, N. Lamersdorf, and S. Steffen (2023). Monetary policy in the age of social media: A Twitter-based inflation analysis. Working paper.

Bradley, D., J. Hanousek Jr, R. Jame, and Z. Xiao (2024). Place your bets? The value of investment research on Reddit's Wallstreetbets. The Review of Financial Studies, Forthcoming.

Braghieri, L., R. Levy, and A. Makarin (2022). Social media and mental health. American Economic Review 112(11), 3660-3693.

Campbell, B., M. Drake, J. Thornock, and B. Twedt (2023). Earnings virality. Journal of Accounting and Economics 75(1), 101517.

Campbell, J. L., M. D. DeAngelis, and J. R. Moon (2019). Skin in the game: Personal stock holdings and investors' response to stock analysis on social media. Review of Accounting Studies 24, 731-779.

Cannon, B., D. Hirshleifer, and J. Thornton (2024). Friends with benefits: Social capital and household financial behavior. NBER working paper.

Cao, S. S., V. W. Fang, and L. G. Lei (2021). Negative peer disclosure. Journal of Financial Economics 140(3), 815-837.

Cassella, S., C. Dim, and T. Karimli (2023). Optimism shifting. Available at SSRN 4557313.

Charoenwong, B., A. Kwan, and V. Pursiainen (2020). Social connections with COVID-19-affected areas increase compliance with mobility restrictions. Science advances 6(47), eabc3054.

Chen, H., P. De, Y. Hu, and B.-H. Hwang (2014). Wisdom of crowds: The value of stock opinions transmitted through social media. The Review of Financial Studies 27(5), 1367-1403.

Chen, H. and B.-H. Hwang (2022). Listening in on investors' thoughts and conversations. Journal of Financial Economics 145(2), 426-444.

Chen, S., L. Peng, and D. Zhou (2024). Wisdom or whims? Decoding investor behavior and market dynamics from social media and large language models. Working Paper.

Chetty, R. et al. (2022a). Social capital I: measurement and associations with economic mobility. Nature 608(7921), 108-121.

Chetty, R. et al. (2022b). Social capital II: determinants of economic connectedness. Nature 608(7921), 122-134.

Chinco, A. (2023). The ex ante likelihood of bubbles. Management Science 69(2), 1222-1244.

Cinelli, M., G. De Francisci Morales, A. Galeazzi, W. Quattrociocchi, and M. Starnini (2021). The echo chamber effect on social media. Proceedings of the National Academy of Sciences 118(9), e2023301118.

Cookson, J. A., J. E. Engelberg, and W. Mullins (2020). Does partisanship shape investor beliefs? Evidence from the COVID-19 pandemic. The Review of Asset Pricing Studies 10(4), 863-893.

Cookson, J. A., J. E. Engelberg, and W. Mullins (2023). Echo chambers. The Review of Financial Studies 36(2), 450-500.

Cookson, J. A., V. Fos, and M. Niessner (2022). Does disagreement facilitate informed trading? Available at SSRN 3765092.

Cookson, J. A., C. Fox, J. Gil-Bazo, J. F. Imbet, and C. Schiller (2023). Social media as a bank run catalyst. Available at SSRN 4422754.

Cookson, J. A., E. Gallagher, and P. Mulder (2023). Money to burn: Crowdfunding wildfire recovery. Available at SSRN 4535190.

Cookson, J. A., D. Garcia, and E. Jarnecic (2024). News consumption in the wild. Available at SSRN.

Cookson, J. A., R. Lu, W. Mullins, and M. Niessner (2024). The social signal. Journal of Financial Economics, Forthcoming.

Cookson, J. A. and M. Niessner (2020). Why don't we agree? Evidence from a social network of investors. Journal of Finance 75(1), 173-228.

Cookson, J. A. and M. Niessner (2023). Investor disagreement: Daily measures from social media. Available at SSRN 4529594.

Cookson, J. A., M. Niessner, and C. Schiller (2024). Can social media inform corporate decisions? Evidence from merger withdrawals. Journal of Finance, Forthcoming.

Coval, J. D., D. Hirshleifer, and T. Shumway (2021). Can individual investors beat the market? The Review of Asset Pricing Studies 11(3), 552-579.

Da, Z., J. Engelberg, and P. Gao (2011). In search of attention. Journal of Finance 66(5), 1461-1499.

Da, Z., J. Hua, C.-C. Hung, and L. Peng (2023). Market returns and a tale of two types of attention. Available at SSRN 3551662.

Da, Z. and X. Huang (2020). Harnessing the wisdom of crowds. Management Science 66(5), 1847-1867.

Da, Z., X. Huang, and L. J. Jin (2021). Extrapolative beliefs in the cross-section: What can we learn from the crowds? Journal of Financial Economics 140(1), 175-196.

Das, S. R. and M. Y. Chen (2007). Yahoo! for Amazon: Sentiment extraction from small talk on the web. Management science 53(9), 1375-1388.

deHaan, E., A. Lawrence, and R. Litjens (2024). Measuring investor attention using Google search. Management Science, Forthcoming.

Dessaint, O., T. Foucault, and L. Frésard (2024). Does alternative data improve financial forecasting? The horizon effect. The Journal of Finance 79(3), 2237-2287.

Dim, C. (2023). Social media analysts' skills: Insights from text-implied beliefs. Available at SSRN 3813252.

Drake, M. S., J. R. Moon Jr, B. J. Twedt, and J. D. Warren (2023). Social media analysts and sell-side analyst research. Review of Accounting Studies 28(2), 385-420.

Drake, M. S., D. T. Roulstone, and J. R. Thornock (2015). The determinants and consequences of information acquisition via EDGAR. Contemporary Accounting Research 32(3), 1128-1161.

Dugast, J. and T. Foucault (2018). Data abundance and asset price informativeness. Journal of Financial Economics 130(2), 367-391.

Eaton, G. W., T. C. Green, B. S. Roseman, and Y. Wu (2022). Retail trader sophistication and stock market quality: Evidence from brokerage outages. Journal of Financial Economics 146(2), 502-528.

Farboodi, M., A. Matray, L. Veldkamp, and V. Venkateswaran (2022). Where has all the data gone? The Review of Financial Studies 35(7), 3101-3138.

Farrell, M., T. C. Green, R. Jame, and S. Markov (2022). The democratization of investment research and the informativeness of retail investor trading. Journal of Financial Economics 145(2), 616-641.

Fedyk, V. (2023). This time is different: Investing preferences in the age of Robinhood. Available at SSRN 4112307.

Feng, X. and A. C. Johansson (2019). Top executives on social media and information in the capital market: Evidence from China. Journal of Corporate Finance 58, 824-857.

Fox, C., E. K. Kelley, and R. Paolucci (2023). How many words is a picture worth? Using emojis from social media to predict future stock returns. Available at SSRN 4427860.

Gargano, A. and A. G. Rossi (2018). Does it pay to pay attention? The Review of Financial Studies 31(12), 4595-4649.

Giannini, R., P. Irvine, and T. Shu (2018). Nonlocal disadvantage: An examination of social media sentiment. The Review of Asset Pricing Studies 8(2), 293-336.

Giannini, R., P. Irvine, and T. Shu (2019). The convergence and divergence of investors' opinions around earnings news: Evidence from a social network. Journal of Financial Markets 42, 94-120.

Giglio, S., M. Maggiori, J. Stroebel, and S. Utkus (2021). Five facts about beliefs and portfolios. American Economic Review 111(5), 1481-1522.

Grennan, J. and R. Michaely (2021). Fintechs and the market for financial analysis. Journal of Financial and Quantitative Analysis 56(6), 1877-1907.

Gu, M., S. H. Teoh, and S. Wu (2023). GIF sentiment and stock returns. Available at SSRN 4110191.

Han, B., D. Hirshleifer, and J. Walden (2022). Social transmission bias and investor behavior. Journal of Financial and Quantitative Analysis 57(1), 390-412.

Han, B., H. Liu, and P. Sui (2023). Social learning and sentiment contagion in the Bitcoin market. Available at SSRN 4543326.

Hayek, F. A. (1945). The use of knowledge in society. American Economic Review 35(4), 519-530.

Heimer, R. Z. (2016). Peer pressure: Social interaction and the disposition effect. The Review of Financial Studies 29(11), 3177-3209.

Heimer, R. Z., Z. Iliewa, A. Imas, and M. Weber (2024). Dynamic inconsistency in risky choice: Evidence from the lab and field. American Economic Review, Forthcoming.

Heimer, R. Z. and D. Simon (2015). Facebook finance: How social interaction propagates active investing. Working paper.

Hirshleifer, D. (2020). Presidential address: Social transmission bias in economics and finance. Journal of Finance 75(4), 1779-1831.

Hirshleifer, D., L. Peng, and Q. Wang (2024). News diffusion in social networks and stock market reactions. The Review of Financial Studies, Forthcoming.

Hu, A. and S. Ma (2023). Persuading investors: A video-based study. Journal of Finance, Forthcoming.

Irvine, P. J., S. Shen, and T. Shu (2021). Aggregate attention. Working paper.

Isaac, M. (2023). Reddit wants to get paid for helping to teach big A.I. systems.

Jackson, M. O. et al. (2008). Social and economic networks, Volume 3. Princeton university press Princeton.

Jackson, M. O. and A. Wolinsky (2003). A strategic model of social and economic networks. Springer.

Jame, R., R. Johnston, S. Markov, and M. C. Wolfe (2016). The value of crowdsourced earnings forecasts. Journal of Accounting Research 54(4), 1077-1110.

Jame, R., S. Markov, and M. C. Wolfe (2022). Can FinTech competition improve sell-side research quality? The Accounting Review 97(4), 287-316.

Jia, W., G. Redigolo, S. Shu, and J. Zhao (2020). Can social media distort price discovery? Evidence from merger rumors. Journal of Accounting and Economics 70(1), 101334.

Kakhbod, A., S. M. Kazempour, D. Livdan, and N. Schuerhoff (2023). Finfluencers. Available at SSRN 4428232.

Kapons, M. M. and P. Kelly (2023). Biased inference due to prior beliefs: Evidence from the field. Available at SSRN 4209631.

Knack, S. and P. Keefer (1997). Does social capital have an economic payoff? A cross-country investigation. Quarterly Journal of Economics 112(4), 1251-1288.

Kogan, S., I. Makarov, M. Niessner, and A. Schoar (2024). Are cryptos different? Evidence from retail trading. Journal of Financial Economics, Forthcoming.

Kogan, S., T. J. Moskowitz, and M. Niessner (2023). Social media and financial news manipulation. Review of Finance 27(4), 1229-1268.

Kuchler, T., Y. Li, L. Peng, J. Stroebel, and D. Zhou (2022). Social proximity to capital: Implications for investors and firms. The Review of Financial Studies 35(6), 2743-2789.

Kuchler, T. and J. Stroebel (2021). Social finance. Annual Review of Financial Economics 13, 37-55.

Kyle, A. S. (1985). Continuous auctions and insider trading. Econometrica 53(6), 1315-1335.

Lee, C. M. and Q. Zhong (2022). Shall we talk? The role of interactive investor platforms in corporate communication. Journal of Accounting and Economics 74(2-3), 101524.

Lee, L. F., A. P. Hutton, and S. Shu (2015). The role of social media in the capital market: Evidence from consumer product recalls. Journal of Accounting Research 53(2), 367-404.

Leung, H. and T. Ton (2015). The impact of internet stock message boards on cross-sectional returns of small-capitalization stocks. Journal of Banking & Finance 55, 37-55.

Levy, H., A. G. Rossi, R. Shalev, and E. Zur (2023). What's in investors' information set? Available at SSRN 4068922.

Li, F. (2022). Retail trading and asset prices: The role of changing social dynamics. Available at SSRN 4236966.

Li, T., D. Shin, and B. Wang (2021). Cryptocurrency pump-and-dump schemes. Available at SSRN 3267041.

Liu, B. and A. Moss (2022). The role of accounting information in an era of fake news. Available at SSRN 4399543.

Lopez Avila, E., C. Martineau, and J. Mondria (2023). When crowds aren't wise: Biased social networks and its price impact. Available at SSRN 4439793.

Lu, R. and S. Y. Sheng (2022). How racial animus forms and spreads: Evidence from the Coronavirus pandemic. Journal of Economic Behavior & Organization 200, 82-98.

Martel, J., E. D. Van Wesep, and R. Van Wesep (2022). Ratings and cooperative information transmission. Management Science 68(12), 9175-9197.

McLuhan, M. (1975). Understanding media: The extensions of man. Routledge & Kegan Paul.

Mkrtchyan, A., J. Sandvik, and V. Z. Zhu (2023). CEO activism and firm value. Management Science.

Müller, K., Y. Pan, and C. Schwarz (2023). Social media and stock market participation. Available at SSRN 4557783.

Müller, K. and C. Schwarz (2021). Fanning the flames of hate: Social media and hate crime. Journal of the European Economic Association 19(4), 2131-2167.

Müller, K. and C. Schwarz (2023). From hashtag to hate crime: Twitter and antiminority sentiment. American Economic Journal: Applied Economics 15(3), 270-312.

Niessner, M. and E. C. So (2024). Bad news bearers: The negative tilt of the financial press. Available at SSRN 3219831.

Odean, T. (1998). Are investors reluctant to realize their losses? Journal of Finance 53(5), 1775-1798.

Oh, S., S. Rosen, and A. L. Zhang (2024). Digital Veblen goods. Available at SSRN 4042901.

Pedersen, L. H. (2022). Game on: Social networks and markets. Journal of Financial Economics 146(3), 1097-1119.

Peng, L. and L. Zhang (2024). Unleashing the crowd: the effect of social networks in crowdfunding markets. Management Science, Forthcoming.

Pew Research Center, A. (2023). Social media fact sheet. 2023.

Renault, T. (2017). Intraday online investor sentiment and return patterns in the us stock market. Journal of Banking & Finance 84, 25-40.

Sapienza, P. and L. Zingales (2012). A trust crisis. International Review of Finance 12(2), 123-131.

Schafhäutle, S. G. and D. Veenman (2024). Crowdsourced forecasts and the market reaction to earnings announcement news. The Accounting Review 99(2), 421-456.

Sheng, J., Z. Sun, and W. Wang (2023). Partisan return gap: The polarized stock market in the time of a pandemic. Management Science, Forthcoming.

Shiller, R. J. (1984). Stock prices and social dynamics. Brookings Papers on Economic Activity 1984(2), 457-510.

Shiller, R. J. (2017). Narrative economics. American Economic Review 107(4), 967-1004.

Sicherman, N., G. Loewenstein, D. J. Seppi, and S. P. Utkus (2016). Financial attention. The Review of Financial Studies 29(4), 863-897.

Sohangir, S., N. Petty, and D. Wang (2018). Financial sentiment lexicon analysis. In 2018 IEEE 12th international conference on semantic computing (ICSC), pp. 286-289. IEEE.

Srinivasan, K. (2023). Paying attention. Working paper.

Sui, P. and B. Wang (2022). Social transmission bias: Evidence from an online investor platform. Available at SSRN 4081644.

Tetlock, P. C., M. Saar-Tsechansky, and S. Macskassy (2008). More than words: Quantifying language to measure firms' fundamentals. Journal of Finance 63(3), 1437-1467.

Van Bavel, J. J., S. Rathje, E. Harris, C. Robertson, and A. Sternisko (2021). How social media shapes polarization. Trends in Cognitive Sciences 25(11), 913-916.

van Binsbergen, J. H., S. Bryzgalova, M. Mukhopadhyay, and V. Sharma (2024). (Almost) 200 years of news-based economic sentiment. NBER Working Paper.

Van Wesep, E. D. and B. Waters (2021). The sky's the limit: Bubbles and crashes when margin traders are all in. Available at SSRN 3785637.

Welch, I. (1992). Sequential sales, learning, and cascades. Journal of Finance 47(2), 695-732.

Welch, I. (2022). The wisdom of the Robinhood crowd. Journal of Finance 77(3), 1489-1527.

White, J. T. and S. Wilkoff (2023). The effect of celebrity endorsements on crypto: Evidence from initial coin offerings (ICOs). Available at SSRN 4380845.

Wolfskeil, I. (2020). Tweeting in the dark: Corporate communication and information diffusion. Available at SSRN 3560551.
