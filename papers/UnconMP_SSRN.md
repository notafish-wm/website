---
title: "Unconventional Monetary Policy Transmission and Bank Lending Relationships"
authors: ["Christophe Cahn", "Anne Duquerroy", "William Mullins"]
date: "January 2024"
status: "Published"
journal: "Management Science, 2024"
doi: "https://doi.org/10.1287/mnsc.2022.01871"
url: "https://willmullins.net/papers/UnconMP_SSRN.pdf"
ssrn: "https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2970199"
jel: ["E52", "G21", "E58", "E51", "G01"]
keywords: ["Unconventional Monetary Policy Transmission", "Relationship Banking", "SME Finance"]
conversion: "Text-only Markdown for LLM reading. Images omitted. Tables converted to semantic Markdown."
mode: "publication"
---

# Unconventional Monetary Policy Transmission and Bank Lending Relationships

Christophe Cahn (Banque de France), Anne Duquerroy (Banque de France), William Mullins (UC San Diego)

January 2024. Management Science (accepted).

Emails: christophe.cahn@banque-france.fr; anne.duquerroy@banque-france.fr; wmullins@ucsd.edu - corresponding author. Address: University of California San Diego, Rady School of Management, 9500 Gilman Drive 0553, La Jolla, CA 92093. We thank our Editor David Sraer, as well as the anonymous AE and referees. We also thank Carlos Avenancio-Leon, Tobias Berg, Nittai Bergman, Murillo Campello, Claire Celerier, Frederico Cingano, Francesco D'Acunto, Hans Degryse, Michael Faulkender, Laurent Fresard, Florian Heider, Raj Iyer, Stephen Karolyi, Stephan Luck, Jose-Luis Peydro, N. Prabhala, Shrihari Santosh, Antoinette Schoar, David Thesmar, Rick Townsend, Steven Ongena, Guillaume Vuillemey, Ting Xu and participants at the Maryland Finance brownbag, 1st BdF-BdI Workshop on Corporate Finance, FDIC 17th Bank Research Conference, ECB non-standard Monetary Policy Workshop, JFI-Olin Conference, USC Finance, Colorado Finance Summit, MFA, Swiss Winter Conference on Financial Intermediation, SFS Cavalcade, FIRS, WFA, and the Wharton Liquidity Conference. The views in this paper may not reflect those of the Banque de France or the Eurosystem.

## Converter's summary

*This summary was written by the converter (an LLM), not by the authors.* The paper asks whether unconventional monetary policy (UMP) liquidity is transmitted differently by banks to firms with a single bank relationship versus firms with multiple bank relationships. It uses the ECB's 2011-12 Very Long-Term Refinancing Operations (VLTROs) and the Additional Credit Claims (ACC) program, which lowered the minimum Banque de France credit rating (from 4+ to 4) for loans to firms to count as ECB collateral in France, generating within-bank, credit-rating-level variation in the cost of funding loans. Data merge the French national credit register, FIBEN accounting data, and Banque de France credit ratings for independent SMEs. The difference-in-differences design compares newly-eligible (rated 4/ACC) firms to ineligible firms one or two notches below (5+, 5), separately for single- and multi-bank firms, with firm, bank-month, and industry-quarter fixed effects. Headline results: eligible single-bank firms' debt rises about 8% relative to controls and multi-bank firms' about 10% (Table 2, columns 1 and 4); transmission to single-bank firms is selective — concentrated in firms with deep lending relationships (Table 5) and strong observables (Table 7), and tilted toward long-maturity debt (Table 6) — while transmission to multi-bank firms is near-uniform. Ineligible multi-bank firms one notch below the threshold receive "spillover" lending of about 8.5 percentage points (Table 3, column 1), driven by competitive banking markets; single-bank firms receive no spillover. In aggregate, single-bank firms received only 7% of policy-induced lending despite holding 11% of bank credit in 2011.

## Abstract

Firms with only one bank relationship make up the majority of firms in many economies. This paper explores whether policy-driven lending is differentially transmitted to single-bank firms in comparison to the multi-bank firms that are the focus of the literature. Using unique variation in the ECB's Very Long-Term Refinancing Operations (VLTROs), which affected lending to firms discontinuously across credit ratings but within banks, we find selective transmission of VLTRO liquidity to single-bank firms. Banks apply higher lending standards to single-bank firms, with banking relationships determining both new lending and lending maturity. By contrast, banks appear to transmit policy lending near-uniformly across multi-bank firms.

**JEL Classification:** E52, G21, E58, E51, G01

**Keywords:** Unconventional Monetary Policy Transmission, Relationship Banking, SME Finance

## 1 Introduction

Since 2008, central banks have launched novel unconventional monetary policies (UMP) of unprecedented scope. While the banking system itself has been a policy target, banks are also the main conduit through which UMP liquidity is transmitted to all but the largest firms, channeling most policy-driven lending through existing bank-firm relationships. In turn, this has left banks with substantial discretion regarding which firms receive policy pass-through, raising concerns about the distributional consequences of these bank decisions.[^1]

[^1]: For example, press reports and class action lawsuits have argued that banks' allocation of Paycheck Protection Program loans favored larger borrowers and those with more valuable banking relationships (e.g., Balyuk et al., 2020; CBS News, 2020; Financial Times, 2020; Granja et al., 2020; Li and Strahan, 2020).

This paper explores how banks distribute lending across firms by examining a natural fault line in UMP transmission: whether firms with multiple bank relationships have differential access to policy-driven lending vs. firms with only one bank relationship. In times of crisis, firms with multiple banks may receive more fluid pass-through of policy-driven lending because they are not locked into a single bank relationship.

How credit supply shocks are transmitted to single-bank firms has received little attention. The literature has generally employed a within-firm across-bank empirical strategy (e.g., Khwaja and Mian, 2008), which requires firms to have two or more bank relationships, thus dropping all single-bank firms from research samples. But firms with only one bank make up a major segment of many economies: in France they account for over 80 percent of firms and employ around 40 percent of private sector workers. Similarly, in the US FR-Y14 credit registry over 90% of firms had only one bank relationship in 2019.[^2]

[^2]: The share of single-bank firms in research samples is often biased downwards because they are omitted from credit registries due to minimum firm or loan size reporting thresholds. Section 3.3.1 discusses the prevalence of single-bank firms.

Understanding heterogeneity in the pass-through of liquidity is important because current evidence is based on multi-bank firms; if transmission to single-bank firms is different, current estimates likely understate the financial and real effects of credit contractions. Moreover, because single-bank firms tend to be smaller and younger, and such firms are especially sensitive to aggregate shocks, differential pass-through could reduce the efficacy of UMP: the firms in greatest need of liquidity would be the least likely to receive it.[^3] The goal of this paper – to shed light on the differential transmission of UMP to firms – is thus of interest to our understanding of both the distributional effects of credit supply shocks and the effectiveness of policy responses.

[^3]: Small and medium enterprises (SMEs) make up 85% of firms in the US, and employ around half of all workers (Fort et al., 2013). For the impact of contractions on SMEs, see, for example, Chodorow-Reich et al. (2022), Galbraith (1957), and Gertler and Gilchrist (1994).

There are several reasons to expect differences in UMP transmission along the single vs. multi-bank dimension. First, single-bank firms have undiversified exposure to the health of their bank (e.g., Detragiache et al., 2000). Second, single-bank firms are locked into their bank during crises due to the difficulty of establishing new relationships: the monopoly lender scenario in canonical relationship lending models (e.g., Rajan, 1992; Sharpe, 1990). In contrast, firms with multiple banks are in a position to receive greater liquidity pass-through via existing relationships, consistent with recent work showing that competition between banks increases monetary policy transmission (Benetton and Fantino, 2021; Corbae and Levine, 2021; Wang et al., 2020). Strategic considerations that are absent for single-bank firms may also play a role. For example, a firm's main bank may increase lending to pre-empt other banks from cutting lending in response to macroeconomic conditions (e.g., Giannetti and Saidi, 2019).

This paper examines how unconventional European Central Bank (ECB) policies operating through collateralized lending to banks are transmitted to firms in France. This class of central bank liquidity schemes has been in continuous use in the Eurozone since 2011 and constituted a major component of the economic response to COVID-19. To mitigate potential anticipation effects, we focus on the first iteration of this long-maturity liquidity policy at scale, the €1 trillion Very Long-Term Refinancing Operations (VLTROs) of 2011-2012, introduced in response to the European Sovereign Debt Crisis. The VLTROs allowed banks to borrow in quantities limited only by banks' eligible collateral, at a time when French banks were under severe funding stress – they were the third largest recipients of VLTRO funds, after banks in Spain and Italy.

Using a difference in differences design we show that transmission of the VLTRO via lending to single-bank firms is selective, while this is not the case for multi-bank firms. Specifically, we find that for single-bank firms, banks apply higher lending standards, with banking relationship quality determining both new lending and lending maturity, and we show liquidity is not transmitted to the weakest firms. By contrast, banks appear to transmit policy lending nearly uniformly across multi-bank firms. Further, we show that banks choose to also lend to a subset of multi-bank firms – but not single-bank ones – whose debt was ineligible as VLTRO collateral, which we term "spillover" lending. This spillover lending was driven by the most competitive banking markets, consistent with an important role for competition in the transmission of UMP. Both sets of results – selective lending to single-bank firms but not to multi-bank ones and competition-driven spillover lending to multi-bank firms – hold in samples beyond our well-identified treatment and control groups around the credit rating eligibility threshold. For example, we find selective lending across all of the eligible firm credit rating distribution. In addition, we find very similar effects in subsamples defined by firm characteristics, supporting the idea that bank relationships are a key mediator of UMP rather than a correlate of other firm characteristics.

We now describe the setting and our results in more detail. Two policy design features jointly determined the extent of the VLTROs' pass-through to firms. First, the VLTROs made three-year collateralized lending available to banks, at subsidized rates. The long maturity of this lending removed short-term rollover risk, unlike previously available ECB lending, which had typical maturities of three months or less. Second, banks could already use certain "eligible" loans to firms as collateral when borrowing from the ECB. The VLTRO package's ACC program unexpectedly lowered (by one notch) the minimum firm credit rating required for a firm's loans to be collateral-eligible in France. This change meant that a bank's cost of funding a loan to newly-eligible firms dropped suddenly, relative to the cost of lending to ineligible firms. Thus, this policy change created natural treated and control groups for a difference in differences design: firms on either side of the new credit-rating eligibility threshold, before and after the policy change.[^4]

[^4]: The system for managing French banks' collateral at the ECB allowed them to replace any maturing or newly-ineligible loans posted as collateral with different or newly originated eligible loans. Thus, the VLTRO policy was a sustained three-year reduction in the cost of lending to eligible firms, not a one-shot policy. See section 2.2.

The VLTROs provide a unique window into the liquidity transmission process because they involved a policy change at the level of firm credit ratings. This allows us to examine changes within bank lending portfolios – that is, to compare eligible firms to ineligible firms borrowing from the same bank in the same month. This comparison allays identification concerns stemming both from banks being able to choose how much VLTRO funding they received, and from banks and firms matching endogenously. Crucially, the variation provided by the VLTROs means that we are able to include single-bank firms in the analysis.

Throughout the paper we compare the pass-through of VLTRO liquidity to eligible single-bank firms vs. to ineligible firms that are also single-bank. In parallel, we separately perform the same eligible vs. ineligible comparison for multi-bank firms, rather than analyzing them together with single-bank firms. This is both because we have reasons to expect different responses and because the number of bank relationships is endogenous in normal times, although we find that single-bank firms stay single-bank (and vice versa) throughout our sample period. Supporting the need to distinguish between single and multi-bank firms when examining UMP transmission, we show that multi-bank firms are poor controls for single-bank firms: trends in credit growth in the years preceding the policy are negative for single-bank firms, in contrast to a broadly stable pattern for multi-bank firms. However, looking within single- or within multi-bank firms, we find that pre-policy dynamics are very similar across credit ratings, even at a monthly frequency. These indistinguishable pre-trends support our research design, as do a series of robustness tests showing that any confounding factors would have to fail to affect nearby credit ratings. Importantly, all specifications include fixed effects by firm, by bank-month and by industry-quarter, as well as controls for time trends in the main determinants of credit.

We first establish that VLTRO liquidity is transmitted to both single and multi-bank SMEs: credit growth of eligible firms relative to controls increases by approximately 8 percent for single-bank firms, and 10 percent for multi-bank firms in our difference in differences design.[^5] We then examine how liquidity is transmitted. Clear differences emerge when we examine which firms within each group receive policy lending. For single-bank firms this lending is directed almost exclusively towards the strongest eligible borrowers: those with well-developed lending relationships, and those with the strongest observable characteristics, such as high asset tangibility. In short, banks appear to apply high standards for policy-induced lending to single-bank firms. In keeping with this, eligible firms' average interest coverage ratios improve despite their leverage increasing, and lending is tilted towards longer maturity debt, both of which suggest positive selection in lending to single-bank borrowers. In contrast, for multi-bank firms we find that banks transmit liquidity uniformly across the distribution of eligible borrowers. That is, for multi-bank firms: (i) stronger banking relationships do not map to additional lending; (ii) firms with weaker observable characteristics also receive policy-induced lending; and (iii) interest coverage ratios of eligible firms decline following the policy.

[^5]: We estimate similar-sized increases for higher-rated firms further above the eligibility cutoff, and for eligible large firms.

Differential policy transmission to single-bank vs. multi-bank firms in terms of borrower selection is also apparent when we examine the left tail of the credit distribution. Policy-driven lending to single-bank firms remains selective: the share of firms experiencing sharp reductions in their bank debt (a drop of more than twenty percent) remains unchanged even a year after policy implementation. By contrast, the banks quickly ease credit conditions for even the weakest segment of eligible multi-bank borrowers post-VLTRO. Specifically, the share of multi-bank firms that see large cuts in their total bank debt declines within a month of VLTRO rollout, relative to controls.

As well as incentivizing new lending to eligible borrowers, the VLTROs also lowered overall bank funding costs by allowing banks to use some existing loans as collateral. However, banks were not required to use this additional financial slack to lend only to eligible borrowers. We find evidence that banks chose to also lend to a subset of multi-bank firms whose debt was ineligible as collateral: those in the just-ineligible credit rating, i.e., one notch below eligibility.[^6] This spillover lending to multi-bank firms is of comparable magnitude to the main effect and appears to be entirely driven by competitive banking markets, suggesting that competition between banks is an important channel for UMP transmission. Consistent with much more limited bank competition for their business, we find no spillover lending to single-bank firms.[^7]

[^6]: The spillover lending to multi-bank firms in the just-ineligible credit rating means that we define an additional control group for multi-bank firms: the unaffected ineligible rating category directly below the rating receiving spillover lending. The pre-trends of both groups are indistinguishable.

[^7]: The absence of spillover lending for single-bank firms and the existence of positive (rather than negative) spillover for multi-bank firms, indicate that the increased lending we find is not generated by the reallocation of lending away from ineligible firms.

We explore the differential transmission of VLTRO liquidity further to provide support for the bank relationship channel. First, we show that firms with credit ratings above the threshold also show the same pattern of higher lending standards being applied to single, but not multi-bank firms, suggesting that multi-bank status is not seen by the bank as indicating a firm's higher credit quality. Second, we repeat our tests within subsamples defined by firm characteristics typically associated with lending: asset tangibility, age, and leverage. We find evidence of spillover lending to multi-bank – but not single-bank – firms in each subsample. In these subsample splits we also find that lending relationships matter for lending to single-bank – but not multi-bank – firms. These subsample-based tests provide further evidence that, rather than being correlates of firms' observable characteristics, bank UMP transmission is fundamentally different depending on whether firms have only a single bank relationship. Finally, we examine whether differences in the strength of banks' balance sheets also affected the transmission of UMP. We find no material effects, suggesting that the heterogeneous transmission we identify occurs within bank portfolios and so was driven by firm characteristics, not those of banks.

In aggregate, our estimates imply attenuated transmission of VLTRO liquidity to single-bank firms: total policy-induced lending to multi-bank firms as a group grew by over 50% more than did lending to single-bank firms over the following year. Moreover, while single-bank firms in our sample made up 11% of total bank credit in 2011, we estimate they received only 7% of the euro volume of additional lending to firms induced by the VLTROs, with multi-bank firms receiving the remainder.

**Contributions:** This paper is related to the large literature on the pass-through of monetary policy and bank shocks to firms,[^8] but most closely relates to the much smaller literature on the frictions and channels through which UMP is transmitted to SMEs. Benetton and Fantino (2021) shows that local banking competition affects the pass through of the TLTRO, while Adelino et al. (2022) shows that the ECB's corporate bond buying program affects smaller firms via trade credit networks. Chodorow-Reich et al. (2022) provides evidence that smaller firms have different borrowing options and face greater lender discretion in crises than larger firms. This paper contributes by showing that pre-determined bank relationships are key mediators of UMP transmission for a large segment of the firm distribution.

[^8]: See Amiti and Weinstein (2017), Chava and Purnanandam (2011), Chodorow-Reich (2014), Gomez et al. (2021), Iyer et al. (2014), Jiménez et al. (2012), Jiménez et al. (2014), Khwaja and Mian (2008), Paravisini (2008), and Schnabl (2012).

There is also a related literature on the impact of large scale purchase programs of bank assets (e.g., Chakraborty et al., 2019; Di Maggio et al., 2020; Luck and Zimmermann, 2020; Rodnyansky and Darmouni, 2017). The VLTROs were instead a policy intervention aimed at the cost and maturity of banks' debt, and similar policies have grown markedly in importance since 2008.[^9] Papers on the VLTROs themselves focus on cross-bank heterogeneity in loan price effects using repeated cross-section survey data (Mésonnier et al., 2017) or on cross-bank differences in uptake and aggregate effectiveness (Andrade et al., 2018; Carpinelli and Crosignani, 2020; Garcia-Posada and Marchetti, 2016; Jasova et al., 2021). In contrast, we focus on transmission differences across borrowers within each bank's portfolio, and show the empirical importance of single-bank firms.

[^9]: Examples of collateralized central bank lending policies include the Term Asset-Backed Securities Loan Facility (USA, 2008), the Funding for Lending Scheme (UK, 2012), and the Targeted Long-Term Refinancing Operations (TLTROs, Eurosystem, 2014, 2016, 2019). The Bank of Japan implemented a similar policy to the VLTRO in 2009-10. In March 2020 the ECB announced new LTROs designed to dovetail with the TLTRO III and expanded the ACC framework. In April 2020 the Federal Reserve created a liquidity facility to accept bank loans to firms issued under the Paycheck Protection Program as collateral, at face value.

This paper is also related to the recent literature incorporating firm heterogeneity into models of monetary policy (e.g., Ippolito et al., 2018; Jeenas, 2019; Ottonello and Winberry, 2020). In contrast to this focus on heterogeneity of firm responses to a common monetary policy, we show that banks engage in heterogeneous transmission of policy across firms. Our results argue for embedding heterogeneity in terms of single vs. multi-bank relationships in models of monetary policy transmission.

Several papers have examined limits to the effectiveness of UMP, such as liquidity hoarding (Caballero and Krishnamurthy, 2008; Heider et al., 2015), or potential fire sales crowding out lending (Abbassi et al., 2016; Diamond and Rajan, 2011; Drechsler et al., 2016; Shleifer and Vishny, 2010). We add a different channel through which UMP effectiveness may be constrained: differential transmission of lending to the larger firms in the economy. Finally, our results contribute to the understanding of lending relationships over the cycle (e.g., Beck et al., 2018; Bolton et al., 2016; Boualam, 2018; Hachem, 2011; Liberti and Sturgess, 2018).

The structure of the paper is as follows. Section 2 describes the VLTROs, section 3 covers the data, and section 4 the empirical strategy. Sections 5 to 8 discuss results, and section 9 concludes.

## 2 The VLTRO Policy

The European Central Bank has been providing collateralized long-term lending to Eurozone banks continuously since 2011, and such lending constituted a major component of the economic response to COVID-19. Appendix 1 provides suggestive evidence of differential pass-through of UMP liquidity to single- vs. multi-bank firms from TLTROs launched between 2013 and 2020. This section provides information on the 2011-12 VLTROs, the first iteration of this policy at scale and the focus of this paper.

### 2.1 Background: French banks in 2011

In the second semester of 2011 French banks came under severe funding stress during the "Quiet Run of 2011" (Chernenko and Sunderam, 2014). They were directly exposed to Eurozone periphery sovereign debt and were hit especially hard by the withdrawal of over US\$100 billion in funding from the ten largest US money market funds, which constituted the largest drop in such funding in both percentage and absolute terms across the Eurozone in this period (IMF, 2013).

The top panel of Appendix Figure A2 illustrates the dramatic drop in listed French banks' stock prices that occurred in the second semester of 2011: the stock prices of Crédit Agricole and Société Générale, two of the largest French bank groups, fell by 50 percent between July and September, and continued to fall through the end of the year. This was reflected in their debt funding costs, as illustrated by the bottom panel of Figure A2. Towards the end of 2011, bank marginal funding costs were approximately as high as they were at the peak of the US financial crisis.

Since 2008, Eurozone private banks had been able to fund themselves by borrowing unlimited amounts from the Eurosystem, but this borrowing was short maturity and required banks to provide sufficient eligible collateral (Bindseil et al., 2017). Tradeable securities were eligible collateral, but so were bank assets such as loans to firms with strong credit ratings (known as eligible "credit claims"). However, banks throughout the Eurozone were very likely to have been collateral constrained in 2011 (Barthelemy et al., 2017).[^10]

[^10]: Note that the collateral constraint can bind for individual banks even when banks are unconstrained in aggregate. Further, banks may appear to be over-collateralized when this is not the case, because banks' Eurozone collateral pool is also used for intraday payments (both intra- and internationally), but this intraday use is generally not included when measuring banks' collateral constrainedness.

### 2.2 The policy change: VLTROs and Additional Credit Claims

In response to the financial stress faced by banks across the Eurozone, on December 8th, 2011 the ECB announced a package of unconventional monetary policy measures, consisting most notably of two very long-term refinancing operations (VLTROs) with three year maturities. The ECB also granted national central banks the option to choose to lower the credit rating required for bank loans to firms to be eligible as ECB collateral, known as the ACC program.[^11]

[^11]: The VLTROs provided the option to repay after a year, and were fixed rate, with the rate paid at the end and set at the average main refinancing operations rate over the life of loan. The rating required for residential mortgage backed securities to be eligible collateral was also lowered, and banks' minimum reserve ratio was lowered from 2% to 1%. These measures reinforce the overall effect of reducing the overall liquidity constraint of each bank, but do not affect the validity of our research design, which is focused on within-bank comparisons.

The package provided substantially-below-market-rate funding to participating Eurozone banks, allowing them to borrow amounts limited only by their available collateral, at the (low) main refinancing rate and, crucially, at much longer maturity. The VLTROs' three year maturities were unprecedented for the ECB, which regularly lent at weekly and three month maturities only.[^12] Thus, the main ECB liquidity channel was temporarily switched from providing only short-term liquidity to providing three year liquidity, without any increase in cost to borrowers. Further, a large segment of banks' existing loans to firms were eligible to be used as collateral for this borrowing. This was especially valuable because these loans – assets of the bank – were unusable as collateral in any other contexts.

[^12]: In 2009 the ECB first implemented LTROs with a one year maturity. One year lending was not provided again until a one year LTRO was announced on 6 October 2011.

The VLTROs provided massive amounts of collateralized liquidity. The first took place on December 21st, 2011, and provided €489 billion to banks across the Eurozone, while the second (on February 29th, 2012) provided €530 billion. In total, banks in France received at least €153 billion via the VLTRO mechanism (Andrade et al., 2018), making France the third largest recipient after Spain and Italy. The difference between the cost of market debt and the ECB's main refinancing operation (MRO) rate provides an approximate estimate of the effect of the policy on French banks' funding costs. As illustrated in Appendix Figure A2, in early 2012 this difference was almost 400 basis points (calculation details are in Appendix 2).

This paper exploits the combination of the VLTROs' major easing of banks' overall liquidity constraint and the lowering of credit standards for eligible collateral (termed the Additional Credit Claims or ACC framework) to provide pseudo-exogenous variation in the cost of bank funding of loans to some firms. The ECB announcement was largely unexpected. Further, the ECB left the decision of whether and how to participate in the ACC to each country's Central Bank.

The Banque de France (BdF) assigns credit ratings to all French firms with sales above €0.75 million (see section 3). Until February 2012, the firms receiving the bank loans being posted as collateral had to be rated 4+ or higher in the BdF's credit rating scale to be eligible at the ECB. The public announcement that the BdF was choosing to lower the minimum credit rating of collateral-eligible loans occurred on February 9th, 2012, before the second VLTRO round. It provided the critical details that BdF had chosen to lower the minimum eligible credit rating by one notch, from 4+ to 4, and that it would apply the threshold to loans of all sizes. France was the only large Eurozone economy that chose not to impose a minimum size requirement on newly collateral-eligible loans. Figure 1 illustrates the change in eligible ratings.

Thus, while the possibility that countries might participate in the ACC framework was announced with the VLTROs in December 2011, France's participation was announced two months later, between the first and the second VLTRO rounds. However, these were not separate policy shocks: the newly-eligible ACC credit claims were used as part of the collateral pool for the entirety of each bank's borrowing from the Eurosystem. Further, the VLTRO program functioned as a sustained liquidity injection, because the collateral system allowed banks to swap eligible assets (including newly originated loans) into and out of a collateral pool every day over the three year life of the policy. Importantly, the collateral system did not incentivize French banks to make or pledge negative NPV loans, because they bore the full expected losses.[^13]

[^13]: Eurosystem collateral in France was managed using an automated pool system (which remained in place as of 2023), such that collateral assets were not tied to specific loans. Assets' eligibility for the pool was reviewed daily; if an asset became ineligible the bank had to immediately replace it with an eligible asset. This structure meant that the Eurosystem would only bear default risk on this lending if both the borrowing bank itself defaulted suddenly, and the collateral in the pool was insufficient to cover the bank's liability. Thus, unless the private bank itself was close to default and did not expect to be rescued, the collateral system did not incentivize banks to make or pledge negative NPV loans.

### Figure 1: Banque de France's credit rating scale for firms

The figure shows the full BdF rating scale ordered from highest rating to default: 3++, 3+, 3, 4+, 4, 5+, 5, 6, 7, 8, 9, P. Ratings 3++ through 4+ are labeled "Always eligible"; rating 4 is labeled "Newly Eligible [ACC]" and identified as the treated group; ratings 5+ and 5 are labeled "Never eligible" and identified as the control group(s). Printed annotations: "4+ ≈ BBB-", "4 ≈ BB+".

**Note:** This figure illustrates the Banque de France credit rating scale for firms, as well as whether loans to such firms are eligible as collateral for bank borrowing from the Eurosystem. It also shows the baseline empirical setting for the difference in differences research design (intention-to-treat). Assignment to treatment and control group is based on firms' credit rating in December 2011.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

## 3 Data

### 3.1 Sample composition

We merge the French national credit register, the FIBEN financial statement database, and the credit rating database, all from the Banque de France (BdF). The intersection of these administrative databases contain close to the universe of firms for the segment of the credit rating distribution we examine, but subject to their having at least €750,000 in annual sales (the FIBEN minimum) and total bank debt of at least €25,000 (the credit registry minimum).

We then follow standard practice with this data and drop firms in the finance, agriculture, utility and public sectors. To maximize the external validity of our final sample, we also drop firms without limited liability (i.e., we keep SA and SARL firms), and micro-firms, for which the sales and bank debt minimums mentioned in the preceding paragraph are binding, generating a selected sample. We use the firm size definitions employed by the European Commission and France: SMEs (micro-firms) have fewer than 250 (10) employees, and annual sales or total assets of less than €50 (€2) million or €43 (€2) million respectively.

We focus our attention on SMEs because Khwaja and Mian (2008) and other work has shown that large firms, unlike smaller firms, can find substitutes for bank lending when their banks experience negative shocks. To enable clean inference we also restrict the sample to independent SMEs, because firms that are part of business groups may obtain credit as a result of their holding company's credit rating (via implicit or explicit guarantees), instead of their own rating, invalidating the research design. Using BdF ownership data we identify independent SMEs as firms that are not majority owned by another firm. Accurate consolidation of these firms into business groups is impossible.[^14] However, for completeness we examine the effects of the policy on large firms in section 8.

[^14]: Credit ratings (required by our empirical design) may exist for multiple firms in a group, and there is no clean way to aggregate ratings across them. Moreover, we do not have consolidated balance sheet data for most business groups. While we can combine the firms in a business group into a synthetic single firm by summing their accounting and debt totals, we cannot remove intra-group transfers and transactions, or infer when a firm that is not majority-owned by a group is in fact group-controlled.

### 3.2 Firm credit rating data

Credit ratings are central to our research design, so we describe the data in detail here; further information about the FIBEN (accounting) and French credit registry data is in Appendix 3. BdF assigns credit ratings to all French non-financial companies, public or private, that have FIBEN data. The rating is an assessment of firms' ability to meet their financial commitments over a three-year horizon, and their main use is to determine the eligibility of bank loans as collateral for Eurosystem funding.[^15] Ratings are based on firms' accounting statements, bank loans reported by credit institutions, and legal information, as well as other sources including soft information from local BdF analysts. The latter review ratings whenever a significant new development occurs, as well as on receipt of firms' yearly financial statements.

[^15]: Banks were permitted to use alternative ratings systems to determine loans' collateral eligibility (subject to additional requirements), but internal BdF data indicate that 96% of banks were using the BdF ratings for Eurosystem collateral assessment as of December 2011.

The BdF receives no payments from rated companies, and informs them of their rating. While the rating is not public, banks may access the ratings and make use of them. Thus, BdF has no obvious incentives to inflate firms' ratings, and firms have no leverage over the ratings process. Figure 1 shows that the rating scale has twelve notches, ordered from 3++ (safest), to P (in bankruptcy). A rating of 4+ is approximately equivalent to a long-term rating of BBB-/Baa3 from S&P/Moody's (i.e., just above the investment grade cutoff). The main treatment group is composed of firms rated 4 (ACC firms), and the control groups are one and two notches below (5+, 5). A rating of 4 indicates a 1% probability of default at a 1-year horizon, approximately that of a BBB rated bond in the US. Firms in the 4+, 4 (ACC), and 5+ rating categories represent about 50% of all SMEs with an active credit rating as of December 2011, with 22.1% rated 4 (ACC), and 12.6% rated 5+. Firms that do not provide financials cannot be rated above 6 (making them ineligible as collateral), and thus are not in the sample.

### 3.3 Examining the sample

Table 1 reports sample summary statistics for our main sample, with single-bank firms in the upper and multi-bank in the lower panel. Each panel shows statistics for the treatment group, 4-rated/ACC firms, and for firms rated 5+ (one notch down from ACC) and 5 (two notches down). 5+ is the main control group for single-bank firms and 5 for multi-bank; this choice is supported by evidence presented in later tables that 5+ multi-bank firms also receive policy-driven credit despite their loans being ineligible as collateral, likely as a result of the VLTROs relaxing liquidity constraints at the bank level. Due to this positive "spillover lending," 5+ firms are a partially-treated group, rather than a control group for multi-bank firms. We examine this spillover lending in detail in section 5.4. For transparency we present results using 5+ rated firms as the control group for multi-bank firms, and using 5 rated firms as controls for single-bank firms in Table 2. We also show that our results are robust to using 5 rated firms as the control group for both single and multi-bank firms throughout.

Due to the credit-ratings-based nature of the policy we examine, the SMEs in our sample are slightly larger (average assets of around €2 million) than typical SME samples. As is usual for SMEs, bank loans are their main external funding source: fewer than 1% of the firms in our sample have access to the bond market. In addition, bank market share of corporate credit in France is very concentrated: in our sample 8 banks provide 96% of total credit in 2011.

### Table 1: Summary Statistics

- **Table type:** Summary statistics
- **Sample:** Main sample as of 2011. Panel A: single-bank firms; Panel B: multi-bank firms. Within each panel, statistics are reported separately by credit rating group: 4/ACC (treatment), 5+ (one notch below ACC), and 5 (two notches below).
- **Significance:** not reported in table note

#### Panel A: Single-bank firms

| variable | rating_group | mean | median | std_dev | n_firms |
|---|---|---:|---:|---:|---:|
| Total assets (thousands of Euros) | 4/ACC | 1,820 | 1,031 | 8,126 | 1,913 |
| Total assets (thousands of Euros) | 5+ | 1,977 | 1,422 | 3,568 | 1,139 |
| Total assets (thousands of Euros) | 5 | 1,462 | 871 | 3,016 | 487 |
| # Employees | 4/ACC | 16.83 | 13.00 | 13.72 | 1,877 |
| # Employees | 5+ | 14.62 | 12.00 | 12.03 | 1,112 |
| # Employees | 5 | 16.00 | 13.00 | 16.24 | 475 |
| Bank debt (thousands of Euros) | 4/ACC | 290 | 122 | 512 | 1,913 |
| Bank debt (thousands of Euros) | 5+ | 730 | 304 | 986 | 1,139 |
| Bank debt (thousands of Euros) | 5 | 454 | 186 | 646 | 487 |
| Leverage | 4/ACC | 0.18 | 0.13 | 0.18 | 1,866 |
| Leverage | 5+ | 0.34 | 0.30 | 0.26 | 1,069 |
| Leverage | 5 | 0.28 | 0.20 | 0.27 | 448 |
| Short-term debt / total debt | 4/ACC | 0.21 | 0.00 | 0.35 | 1,862 |
| Short-term debt / total debt | 5+ | 0.17 | 0.00 | 0.32 | 1,118 |
| Short-term debt / total debt | 5 | 0.33 | 0.07 | 0.40 | 480 |
| Length of main bank relationship (years) | 4/ACC | 7.56 | 6.58 | 4.30 | 1,913 |
| Length of main bank relationship (years) | 5+ | 6.25 | 5.42 | 4.21 | 1,139 |
| Length of main bank relationship (years) | 5 | 6.89 | 6.00 | 4.51 | 487 |
| Fixed assets over total assets | 4/ACC | 0.47 | 0.46 | 0.28 | 1,866 |
| Fixed assets over total assets | 5+ | 0.45 | 0.40 | 0.34 | 1,069 |
| Fixed assets over total assets | 5 | 0.57 | 0.57 | 0.35 | 448 |
| Profitability | 4/ACC | 0.11 | 0.10 | 0.12 | 1,913 |
| Profitability | 5+ | 0.10 | 0.10 | 0.10 | 1,139 |
| Profitability | 5 | 0.08 | 0.08 | 0.13 | 487 |
| Investment | 4/ACC | 0.18 | 0.03 | 1.47 | 1,689 |
| Investment | 5+ | 0.38 | 0.02 | 2.53 | 871 |
| Investment | 5 | 0.15 | 0.01 | 0.77 | 365 |
| Interest coverage ratio | 4/ACC | 16.11 | 9.30 | 22.73 | 1,830 |
| Interest coverage ratio | 5+ | 8.44 | 5.42 | 14.65 | 1,121 |
| Interest coverage ratio | 5 | 5.88 | 3.44 | 14.80 | 467 |
| Cost of debt | 4/ACC | 0.06 | 0.04 | 0.06 | 1,900 |
| Cost of debt | 5+ | 0.05 | 0.04 | 0.05 | 1,137 |
| Cost of debt | 5 | 0.06 | 0.04 | 0.06 | 480 |

#### Panel B: Multi-bank firms

| variable | rating_group | mean | median | std_dev | n_firms |
|---|---|---:|---:|---:|---:|
| Total assets (thousands of Euros) | 4/ACC | 2,488 | 1,446 | 4,411 | 3,287 |
| Total assets (thousands of Euros) | 5+ | 2,420 | 1,374 | 5,895 | 1,907 |
| Total assets (thousands of Euros) | 5 | 2,149 | 1,255 | 3,158 | 830 |
| # Employees | 4/ACC | 23.81 | 18.00 | 20.95 | 3,262 |
| # Employees | 5+ | 22.85 | 17.00 | 19.52 | 1,879 |
| # Employees | 5 | 24.44 | 18.00 | 20.10 | 813 |
| Bank debt (thousands of Euros) | 4/ACC | 452 | 218 | 914 | 3,287 |
| Bank debt (thousands of Euros) | 5+ | 535 | 271 | 933 | 1,907 |
| Bank debt (thousands of Euros) | 5 | 534 | 267 | 874 | 830 |
| Leverage | 4/ACC | 0.14 | 0.11 | 0.15 | 3,193 |
| Leverage | 5+ | 0.18 | 0.12 | 0.18 | 1,832 |
| Leverage | 5 | 0.17 | 0.11 | 0.19 | 788 |
| Short-term debt / total debt | 4/ACC | 0.40 | 0.31 | 0.38 | 3,236 |
| Short-term debt / total debt | 5+ | 0.46 | 0.43 | 0.38 | 1,888 |
| Short-term debt / total debt | 5 | 0.55 | 0.62 | 0.38 | 823 |
| Length of main bank relationship (years) | 4/ACC | 7.79 | 7.08 | 4.44 | 3,287 |
| Length of main bank relationship (years) | 5+ | 7.49 | 6.75 | 4.35 | 1,907 |
| Length of main bank relationship (years) | 5 | 7.64 | 7.08 | 4.45 | 830 |
| Fixed assets over total assets | 4/ACC | 0.45 | 0.42 | 0.26 | 3,193 |
| Fixed assets over total assets | 5+ | 0.48 | 0.45 | 0.28 | 1,832 |
| Fixed assets over total assets | 5 | 0.52 | 0.48 | 0.31 | 788 |
| Profitability | 4/ACC | 0.12 | 0.10 | 0.11 | 3,287 |
| Profitability | 5+ | 0.11 | 0.11 | 0.11 | 1,907 |
| Profitability | 5 | 0.08 | 0.08 | 0.14 | 830 |
| Investment | 4/ACC | 0.13 | 0.03 | 0.60 | 2,959 |
| Investment | 5+ | 0.12 | 0.02 | 0.49 | 1,662 |
| Investment | 5 | 0.13 | 0.02 | 0.90 | 705 |
| Interest coverage ratio | 4/ACC | 18.30 | 9.13 | 27.99 | 3,220 |
| Interest coverage ratio | 5+ | 13.08 | 6.67 | 22.03 | 1,886 |
| Interest coverage ratio | 5 | 9.12 | 4.44 | 20.60 | 804 |
| Cost of debt | 4/ACC | 0.06 | 0.05 | 0.05 | 3,281 |
| Cost of debt | 5+ | 0.06 | 0.05 | 0.04 | 1,904 |
| Cost of debt | 5 | 0.06 | 0.05 | 0.05 | 825 |

**Note:** The top panel reports sample summary statistics as of 2011 for single-bank firms, and the bottom panel for multi-bank firms. The panels show statistics for the main treatment group (ACC firms, rated 4), and for two control groups: 5+ (one notch below ACC) and 5 (two notches below). Single-bank (multi-bank) refers to firms with only one (>1) bank relationship throughout 2011.

#### 3.3.1 How prevalent are single-bank firms?

We classify firms as single-bank if they borrow from only one bank throughout 2011, and multi-bank if they borrow from more than one for at least one month in 2011. In 2008, 83% of French firms had a single-bank relationship, but this is highly correlated with firm size: only 21% of large firms were single-bank (Aleksanyan et al., 2010).

Credit registry data, when not truncated by minimum firm or loan size reporting thresholds,[^16] tend to be dominated by single-bank firms. In the US, the reported share of single-bank firms ranges from 82% for the SME sample in Petersen and Rajan (1994, p.16) to 92% in the 2019 FR-Y14 credit registry in Chodorow-Reich et al. (2022).[^17] Other examples include Khwaja and Mian (2008), which reports that 90% of firms in Pakistan are single-bank; in Paravisini (2008) the implied share is 89% (from Table VII) for Argentina; Mullins and Toro (2018) reports 73% for Chile; Benetton and Fantino (2021) reports 70% for Italy; in Bonfim et al. (2021) the share is 64% for Portugal; and in Schnabl (2012) the share is 79% for Peru.[^18] Thus, examining transmission to single-bank firms is important to our understanding of policy's efficacy and distributional effects in many countries. In our sample, because we drop micro-firms and firms in business groups, and require them to have approximately investment-grade credit ratings, we have broadly equal numbers of single and multi-bank firms. This means that the single-bank firms we examine are among the largest and financially strongest firms in this category, making it likely that the selective transmission we find is a lower bound of the true effect.

[^16]: For example, the minimum credit exposure required for a borrower to be captured by Deutsche Bundesbank's German national credit registry was €1.5 million until 2015, and €1 million after.

[^17]: The FR-Y14 statistic is as of the end of 2019 and is calculated from Chodorow-Reich et al. (2022) and confirmed with the authors. The FR-Y14 data may overstate the share of single-bank firms, as smaller banks and loans below \$1 million are not included in the data. However, the statistic shows that such firms make up a large segment of the US firm population.

[^18]: By contrast, over half of firms in Spain appear to be multi-bank, perhaps because there are around 350 banks operating in the country (Jiménez et al., 2012).

#### 3.3.2 Comparing treatment and control groups

The upper panel of Table 1 shows statistics for single-bank ACC and 5+ rated firms in particular. These groups show similarities in terms of assets (total and fixed) and profitability, as well as moderately-sized differences for headcount (13% lower for 5+ firms) and share of short-term debt (19% lower). While 5+ firms have higher investment in fixed assets and leverage, these differences are a direct result of how credit ratings are determined. Importantly, these differences are absorbed by our firm and industry-time fixed effects, and especially by the interaction of pre-period covariates (size, profitability, asset tangibility) with the Post indicator in our empirical specification. A discussion of the pre-trends in credit growth, shown in Figure 2, is provided later.

Comparing multi-bank ACC and 5 rated firms in the lower panel of Table 1 we see that they are broadly similar in terms of size (assets, employees), and length of main bank relationship. However, Table 1 shows some unsurprising differences in characteristics that determine credit ratings. In particular, debt and leverage (around 20% larger for 5 rated firms); dependence on short-term debt (38% more for 5 rated firms); fixed assets as a proportion of total assets (15% more for 5 rated firms); and flow items such as asset growth, and profitability. As discussed above, the fixed effects and pre-period covariate interactions with the Post indicator included in all specifications will absorb both pre-existing and trend differences.

#### 3.3.3 Comparing single and multi-bank firms

The number of bank relationships a firm has is endogenous.[^19] Firms tend to begin life with a single lender and acquire more as they grow (Farinha and Santos, 2002; Petersen and Rajan, 1994) consistent with the evidence in Table 1 that single-bank firms are on average smaller in terms of assets and employees. This is corroborated by unreported cross-sectional regressions comparing single and multi-bank firms in June 2011, including a wide variety of firm characteristics as controls. These regressions also show that multi-bank firms are more profitable on average, consistent with the idea that faster growing firms are more likely to become multi-bank earlier, to minimize hold up and liquidity risks (Ongena and Smith, 2001). Single-bank firms also appear to have substantially more medium/long-term bank debt than multi-bank firms. No other differences (such as leverage or asset tangibility) are consistently statistically significant in these regressions.

[^19]: Extant explanations for why firms develop multiple bank relationships include: bank specialization (Paravisini et al., 2023); reducing bank information rents (Rajan, 1992; Sharpe, 1990); reduced exposure to bank-specific shocks (Detragiache et al., 2000); and improved financing terms resulting from higher ex post debt renegotiation costs (Bolton and Scharfstein, 1996).

## 4 Empirical strategy

### 4.1 Empirical design

Our empirical strategy exploits the fact that the policy package reduced the costs to banks of lending to firms rated 4 or ACC – by making loans to these firms eligible as ECB collateral – but did not reduce the cost of lending to other firms at the same bank with similar credit ratings. Thus, the firms in the adjacent credit rating one notch below (5+), whose loans were just-ineligible as collateral, are our main control group in a difference in differences research design for firm-level outcomes. However, we also show results using firms rated 5 (two notches below) as controls, and for multi-bank firms this is our preferred control group, as discussed in Section 5.[^20]

[^20]: Our main results use 5+ rated firms as controls for single-bank and 5 rated firms for multi-bank. However, we show our results are robust to using 5 as the control group for both types of firms in Tables 2, 9, A1, A4, A8, A9, A10, A13, and A14.

We do not use the firms rated just above the ACC (treatment) group as controls because they were also subject to a large positive shock to their value as collateral: the VLTROs extended ECB loan maturity to three years. Thus, higher-rated firms were themselves "treated." Moreover, they were treated at a higher intensity: loans to such firms were even more attractive as collateral because the higher-rated loans had lower haircuts, and so credit to higher rated firms also increased, which we examine in section 8.

We assign firms to treatment and control groups based on the rating of each firm as of December 2011, when the VLTROs and the possibility of the ACC change had been announced, but specifics were lacking: France's decision to participate in the ACC, and which rating categories were newly-eligible, were announced and implemented in February 2012. We drop observations in January and February 2012. Our results are robust to both of these decisions.[^21] We estimate an Intention-To-Treat (ITT) effect, because firms' ratings make their loans eligible or ineligible for treatment, but we do not observe which loans are pledged as collateral. Self-selection by firms into eligibility can be ruled out, because ratings are assigned by the Banque de France, as described in section 3.

[^21]: Results are unaffected if we define treatment and control groups based on firm credit ratings as of September, October, or November 2011, as shown in Appendix Table A5. They are also not sensitive to including January and February 2012 observations. Firm rating varies over time as firms are re-rated, generating mixing in our treatment and control groups both in the pre and post-treatment periods. The pattern of mixing suggests a downward bias to our estimates: control firms are more likely to be upgraded (i.e., into the treatment group) than treated firms, while the latter are more likely to be downgraded into the control group.

As mentioned in the preceding section, single- and multi-bank firms may differ across several dimensions, and the number of bank relationships is endogenous in normal times. For this reason, we run all regressions for single-bank firms separately from those for multi-bank firms. We also verify that we do not have ex post mixing of single and multi-bank groups: almost all single-bank firms stay single-bank in our post period and so do multi-bank firms. This is unsurprising, as during periods of stress to the financial system it becomes very difficult for firms to establish a new bank relationship, making the number of relationships empirically near-exogenous. Further, (as described later) we find that the two groups have different pre-trends, consistent with different access to bank lending in the run up to the policy intervention. Thus, our empirical strategy is to obtain causally identified estimates of VLTRO policy transmission to eligible firms (relative to ineligible firms), separately for the single-bank and multi-bank firm populations, and to contrast them.

### 4.2 Specification

Our main dependent variable measures the percentage change in a firm's total debt relative to its 2011 (pre-period) average, summed across all banks when a firm has multiple banks:

$$g_{ft} = \left( \sum_b \text{Debt}_{fb(f)t} \,/\, \overline{\text{Debt}}_{f2011} \right) - 1 \tag{1}$$

where $\text{Debt}_{fb(f)t}$ is the outstanding amount of bank debt (short-term plus long-term) for firm $f$ borrowed from bank $b$ in month $t$, and $\overline{\text{Debt}}_{f2011}$ is the firm's 2011 average debt level. To mitigate the effect of outliers and especially to reduce the weight given to firms with low levels of debt in 2011, we top-winsorize $g_{ft}$ at 2% (our estimates are robust, and larger, if we do not do this). Table A2 shows our main results are robust to using alternative dependent variables – ln(debt) and leverage – and to using alternatives to the 2011 base period.

We estimate the following difference in differences specification:

$$g_{ft} = \beta(\text{ACC}_f \times Post_t) + \alpha_f + \Lambda_{b(f)t} + \Upsilon_{i(f)t} + \Gamma(X_f \times Post_t) + \epsilon_{ft} \tag{2}$$

where $f$ indexes firm, $i$ industry, $b$ banks, and $t$ months, and the data is at the firm-month level. $\text{ACC}_f$ is an indicator for any firm with a rating of 4 as of December 2011, and so identifies the newly-eligible firms that make up the treated group. $Post_t$ is a post-treatment indicator equal to 1 in each month after February 2012, when loans to ACC-rated firms were eligible to serve as VLTRO collateral. We include firm fixed effects ($\alpha_f$), bank-month fixed effects ($\Lambda_{b(f)t}$), and industry-quarter fixed effects ($\Upsilon_{i(f)t}$). $X_f$ is a vector of firm-level controls (measured in 2011, the pre-period) and is interacted with $Post_t$. The parameter of interest is $\beta$, the ITT effect on newly-eligible firm debt of the VLTRO, relative to controls and the pre-period. We cluster standard errors at the firm level to address serial correlation, but results are fully robust to double-clustering by firm and bank-month (see Table A3). A two-period pre-post difference in differences specification generates very similar estimates and standard errors.

To examine the dynamics of the effect we use a quarterly specification, interacting the ACC indicator with quarter ($q$) indicators instead of with $Post$ and omitting the first two quarters of 2010. This generates noisier, but higher-frequency estimates of the policy effect over time:

$$g_{fq} = \sum_{q>2010Q2} \beta_q \,(\text{ACC}_f \times Qtr_q) + \alpha_f + \Lambda_{b(f)q} + \Upsilon_{i(f)q} + \Gamma(X_f \times Post_q) + \epsilon_{fq} \tag{3}$$

#### 4.2.1 Absorbing differences between firms and trends by firm characteristics

We include firm fixed effects ($\alpha_f$) to absorb all time-invariant firm characteristics that affect credit. Though risk or investment opportunities may vary over time, our estimation window is limited to two years, centered around the policy introduction, thereby mitigating the impact of time-varying firm-level factors.

To address concerns that policy effects might be driven by differential time trends associated with standard determinants of credit ($X_f$), we also interact them with the $Post_t$ indicator in all specifications. $X_f$ includes ln(total assets), tangible assets over total assets, and profitability (EBITDA/total assets), all 0.5% winsorized at both tails. These credit determinants are measured in the pre-period (i.e., at the end of 2011).

#### 4.2.2 Absorbing Bank and Industry shocks, and differential bank-firm matching

To absorb any industry-level shocks we include industry-quarter ($\Upsilon_{i(f)t}$) fixed effects. Because the VLTRO policy varies at the firm credit-rating level (as opposed to the bank-level variation provided by shocks to banks), we are able to include a full set of bank-month fixed effects ($\Lambda_{b(f)t}$). These absorb all time-varying bank heterogeneity at a high frequency. Crucially, they capture any differences between banks in terms of VLTRO uptake or usage across borrowers – recall that the extent of VLTRO uptake is chosen by banks themselves. Further, bank-month fixed effects also absorb other bank credit supply shocks, such as differences in bank responses to the ECB announcement of outright monetary transactions (OMTs) in August 2012. Finally, by focusing the estimation within-bank, these fixed effects capture any differences driven by the endogenous matching of firms and banks.

#### 4.2.3 Considering correlated differences in credit demand

Our baseline specification compares debt growth for eligible vs. ineligible firms borrowing from the same bank in the same month, with similar credit ratings, and with very similar pre-trends, which greatly reduces the scope for confounding variation to affect our estimates.

The within-bank variation we exploit means we cannot use firm-time fixed effects. However, for our estimates to be biased due to differential demand shocks, the following conditions would all have to hold: (i) either the firms in the treatment group or those in the control group would have to be hit with a large demand shock; (ii) this shock would also have to occur at the same time as the VLTRO policy (because the overlapping pre-trends we observe at a monthly frequency are inconsistent with any differential demand shocks ex-ante); and (iii) this differential shock would have to be uncorrelated with banks or with industries (absorbed by bank-time and industry-time fixed effects), and be uncorrelated with the main determinants of credit demand (absorbed by their interactions with the $Post_t$ indicator, together with the firm fixed effect).

Further, the negative shock to banks that gave rise to the VLTRO policy package worked through French bank holdings of non-core Eurozone sovereign debt, that is, it was a foreign-sourced financial shock, rather than a real domestic shock that might naturally impact credit demand. Together, these considerations make it difficult to develop a differential demand story that would generate a bias in our estimates.

In addition, in section 5.3 we provide estimates for alternate pairs of treatment-control groups, and in alternate time periods, to show that differential credit growth appears only in the credit-rating pairs we identify as affected by the policy, and only in the time period when the policy was introduced. We also provide estimates from specifications that include additional controls for demand based on interacted fixed effects that are consistent with our main results.

### 4.3 How the VLTRO policy differs from shocks to banks

The literature typically uses bank-level shocks for identification of causal effects and has generated important advances in our understanding of bank behavior. However, this strategy has to overcome at least two challenges. The first (challenge 1) is that that more-exposed banks are likely different to less-exposed banks in important ways (e.g., an omitted bank characteristic may determine both bank exposure and its response to the shock); this is normally addressed using bank-level controls. In the VLTRO setting using such controls is not viable, because, unlike most bank shocks (which affect banks to different degrees that are not chosen contemporaneously by the banks themselves), here banks each chose how much subsidized VLTRO lending they received, and controls are unlikely to fully capture the determinants of this choice.

The second challenge encountered by bank shock strategies (challenge 2) is that more-affected banks may have a systematically different population of borrowing firms in comparison to less-affected banks (Paravisini et al., 2023). The literature routinely resolves this by using firm-time fixed effects to compare borrowing by the same firm from at least two banks. Unfortunately, this method means that single-bank firms must be dropped from the sample, making it impossible to estimate causal effects for this population.[^22]

[^22]: The standard firm-time fixed effects strategy assumes that firm credit demand is not bank-specific, but bank specialization may generate bank-specific demand (Paravisini et al., 2023). Careful empirical design has addressed this problem in some settings (Ippolito et al., 2016; Paravisini et al., 2014). Rare cases when single-bank firms do not need to be dropped are strategies requiring only credit applications to multiple banks (Jiménez et al., 2012) and those exploiting policy in a regression discontinuity design (Jiménez et al., 2018).

The ACC-VLTRO policy generates unique identifying variation that differs from the bank shocks used in the literature because it occurs at the firm credit-rating threshold and not across banks. This allows us to absorb across-bank heterogeneity, using only within bank variation (resolving challenge 1 and additionally absorbing any bank-specific shocks), such that we only compare firms that are clients of the same bank (resolving challenge 2). It also means that we can keep single-bank firms in the sample.

## 5 VLTRO transmission

### 5.1 Policy transmission: graphical evidence

Figure 2 shows firm average debt growth around the VLTRO policy announcement for newly-eligible firms (the solid line for ACC/4-rated firms) and for just-ineligible firms one rating notch below (dashed line for firms rated 5+), with separate graphs for single and multi-bank firms. The plots provide strong evidence of parallel (near-indistinguishable) pre-trends, because these lines are drawn prior to including controls, and show the data at a monthly frequency for the two years before the policy introduction. Two additional facts emerge from these graphs: single and multi-bank firms' credit dynamics are different, and the transmission of the policy shock appears to be broader for multi-bank firms, via a "spillover" onto the 5+ rating category.

First, over the two-year period preceding the policy, single and multi-bank firms have clearly different trends in credit: the trend is negative for single-banks, but largely stable for multi-bank firms. Moreover, Figure 5 shows that this difference in pre-period bank lending trends is present across the distribution of firm credit ratings. These differing pre-trends may be driven by differing credit demand or supply, and underpin our empirical strategy of identifying the policy effect separately for single and for multi-bank firms.

Second, at the time of the VLTRO, liquidity appears to be transmitted differently to single-bank firms, with a spillover effect emerging for multi-bank firms only. In the month of policy implementation, we see that in the single-bank panel the debt of the treated/ACC group rises sharply, while just-ineligible firms in the next rating category down (5+) display no change. However, in the multi-bank panel, the debt of the 5+ group also increases discontinuously in the month of the policy shock. The timing and discrete nature of the jump in the credit trend of 5+ firms strongly suggests that 5+ firms are also receiving extra lending as a result of the policy, especially in the context of consistently falling GDP growth over the course of 2012.[^23] This means that 5+ multi-bank firms may be poor counterfactuals in our setting, because they appear to benefit from the policy. By contrast, Figure 3 shows that 5 rated firms, the next credit rating notch down, exhibit no change in trend throughout our sample period for either single or multi-banks. Thus, because 5+ rated multi-bank firms appear to have been treated by the policy we report results using both 5+ and 5 rated firms as separate control groups for single-and multi-bank firms in our main specification. We explore the spillover further in section 5.4, showing that the difference between the multi-bank 5+ group and the 5-rated group persists in the regression evidence.

[^23]: While the ACC program reduced the marginal funding cost of lending to eligible firms, the VLTROs also relaxed each bank's overall funding constraint (Section 2). Increased lending to firms ineligible for the ACC component of the policy package is a possible response to this relaxed constraint.

### Figure 2: Average debt growth for treated and control firms

Panel (a): Single-bank firms. Panel (b): Multi-bank firms. Each panel plots g(Debt) (y-axis, range -.15 to .25) against time (x-axis, 01jan2010 to 01jan2014), with two lines by rating category: ACC (solid) and 5+ (dashed), and a vertical line at the December 2011 announcement.

**Note:** The figures show the percentage change in firms' total bank debt (relative to their 2011 average) around the VLTRO policy (announcement date: December 2011 – vertical line) for the treatment group and the control group. The top panel is for single-bank borrowers and the bottom panel for multi-bank borrowers. Assignment to treatment and control groups is based on firms' credit rating in December 2011. The treated group is composed of 4-rated firms (newly-eligible borrowers or "ACC firms"). The control group is composed of 5+ rated firms (closest ineligible borrowers on the Credit Rating scale of the Banque de France). For each month we plot average firm debt growth: i.e., the cross-firm average of $g_{ft} = \sum_b \text{Debt}_{fb(f)t}/\overline{\text{Debt}}_{f2011} - 1$, where f indexes firms and b banks, and the denominator is average debt in 2011.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### 5.2 Policy transmission: regression evidence

Table 2 presents estimates of the impact of the VLTRO policy on credit, comparing newly-eligible firms to ineligible firms one or two notches below (5+ or 5 respectively) using our baseline empirical specification: equation 2. Estimates for single-bank firms are reported in columns (1) and (2). These show that treated firms have 8.2% and 7.3% higher debt levels on average relative to their controls (firms rated 5+ and 5, respectively) in the year after the introduction of the VLTRO, relative to the preceding year.

Columns (3) - (6) report estimates for multi-bank firms. As is clear from the graphical evidence discussed above, Column (3) provides evidence of a smaller (4.3%) but strongly statistically significant difference between newly-eligible ACC firms and ineligible 5+ rated firms one notch below. Column (4) instead compares ACC firms to those two notches below (rated 5) on the credit rating scale. It shows a much larger difference of 10.2% higher debt.[^24] This difference between the estimates in columns (3) and (4) supports the graphical evidence for the existence of a spillover of the policy onto ineligible multi-bank firms. The fact that the spillover occurs exclusively for multi-bank firms is itself strong evidence that the effects of the VLTRO policy were transmitted differently to single-bank firms.

[^24]: We use drawn credit as our main measure of firm debt (rather than drawn plus undrawn credit) because it reflects the policy measure of interest, and because Chodorow-Reich et al. (2022) shows that the use of undrawn credit by SMEs is highly dependent on bank discretion. Moreover, banks tend to cancel credit lines for covenant-violations in periods of aggregate stress (e.g., Acharya et al., 2014; Thakor, 2005). Nonetheless, if we use drawn plus undrawn credit as our dependent variable we obtain estimates that are somewhat smaller but still statistically significant at the 1% level.

In Appendix Table A1 we find a very similar pattern using leverage as the dependent variable: an increase in leverage of 1.7-1.8 percentage points for single-bank (~9% of the mean for ACC-rated firms), and 2.3 percentage points for multi-bank firms (~16% of the mean) for our main samples. When firms have multiple banks it is not obvious whether policy-induced lending will come mainly from their main bank, or from banks with a smaller share. Columns (5) and (6) of Table 2 show that almost all of the extra lending comes from firms' main bank.

### Table 2: Effect of the VLTRO policy on firm credit growth

- **Table type:** Regression (difference in differences, equation 2)
- **Dependent variable:** $g_{ft}$, firm debt growth: the sum of the firm's debt across all banks, divided by the firm's average debt in 2011 ($\overline{\text{Debt}}_{f2011}$), minus one
- **Unit of observation:** firm-month
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | sample | control_group | dependent_variable_scope |
|---:|---|---|---|
| 1 | Single-bank | 5+ rated firms | debt across all banks |
| 2 | Single-bank | 5 rated firms | debt across all banks |
| 3 | Multi-bank | 5+ rated firms | debt across all banks |
| 4 | Multi-bank | 5 rated firms | debt across all banks |
| 5 | Multi-bank | 5+ rated firms | main bank only |
| 6 | Multi-bank | 5 rated firms | main bank only |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.082*** | 0.073*** | 0.043*** | 0.102*** | 0.030** | 0.081*** |
| ACC×post | standard_error | 0.018 | 0.025 | 0.016 | 0.019 | 0.015 | 0.017 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Covariates x Post | Y | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y | Y |
| N of clusters (firms) | 2,806 | 2,218 | 4,719 | 3,724 | 4,713 | 3,720 |
| Observations | 58,992 | 46,359 | 93,295 | 73,348 | 92,767 | 72,961 |
| R² | 0.44 | 0.44 | 0.47 | 0.47 | 0.43 | 0.43 |

**Note:** This table presents difference in differences estimates of the transmission of VLTRO lending to firms, following equation (2). The dependent variable $g_{ft}$ is debt growth: the sum of the firm's debt across all banks, divided by the firm's average debt in 2011 ($\overline{\text{Debt}}_{f2011}$), minus one (i.e., $g_{ft} = \sum_b \text{Debt}_{fb(f)t}/\overline{\text{Debt}}_{f2011} - 1$). Columns (1), (3) and (5) use 5+ rated firms as the control group; the remaining columns use firms rated 5. Columns (5) and (6) restrict the dependent variable to debt held at multi-bank firms' main bank only (i.e., the bank with highest share of total lending). Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

We then explore the dynamics of the effect around the introduction of the policy. Figure 4 presents the quarterly coefficient estimates from equation (3), providing additional evidence for parallel pre-trends. Note that while we identify the announcement quarter (2011q4) with a vertical red line, implementation began in the following quarter (in February 2012) when the details of the ACC framework were announced and the second VLTRO implemented. The figure also shows that the policy effects are sustained into 2013.

### Figure 4: Quarterly dynamics of the VLTRO effect on firm debt

Panel (a): Single-bank firms. Panel (b): Multi-bank firms. Each panel plots quarterly coefficient estimates (y-axis, range -.1 to .2) by quarter (x-axis, 2010q3 to 2013q1), with 95% confidence intervals as dashed lines and a vertical line at the first VLTRO quarter.

**Note:** The top (bottom) figure displays the evolution in the bank debt of eligible (ACC) single-bank (multi-bank) firms around the VLTRO policy announcement date, relative to the closest rating group of ineligible firms (5+ rated firms, for single-bank firms, 5 for multi-bank firms). Using specification 3, we display the estimated treatment coefficient for each quarter, rather than for a single "Post" period. The omitted periods are quarters 1 and 2 of 2010. The coefficient corresponds to the percentage change in firms' total bank debt (relative to their 2011 average). The dashed lines plot 95% confidence intervals; standard errors are clustered by firm. The vertical line identifies the announcement (and implementation) quarter of the first 3-year VLTRO; the second VLTRO (including the ACC) was implemented in the following quarter.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### 5.3 Robustness tests

**Robustness to changes in the dependent variable.** Columns (1) and (2) of Appendix Table A2 illustrate that our results are not dependent on the measure of debt growth used as the dependent variable, as we run our main specification (equation 2) for our main control groups (5+ and 5 for single- and multi-bank firms respectively) using the natural logarithm of debt and leverage respectively instead. We find very similar estimates in terms of magnitudes and statistical significance for both single and multi-bank populations. The similarity of estimates for leverage is unsurprising because leverage is calculated in the same way as $g_{ft}$, but using 2011 total assets instead of average debt as the denominator. Columns (3) to (5) change the scaling of our debt growth measure: instead of using the firm's average debt in 2011 to scale the firm's current debt we instead use, respectively, average debt in 2010, in the first semester of 2011 and in the second semester. Results are very similar and statistically indistinguishable.[^25]

[^25]: Appendix Table A5 also shows robustness of these results to alternate decisions as to when we measure firms' ratings.

**Robustness to within-bank correlation and switching between banks.** Column (1) of Appendix Table A3 clusters standard errors by firm (as in the main specification), and adds clustering by bank-month. The standard errors are essentially unchanged. Column (2) of the table adds bank-firm fixed effects to focus on the variation in the pre-existing set of bank relationships, ensuring that results are not driven by firms that switch banks. Because very few single-bank firms switch banks or become multi-bank in this period (consistent with the "stickiness" of bank relationships, especially in crises), there is no change in the estimate for single-bank firms. For multi-bank firms the estimate falls by about one percentage point to approximately 9%. Thus, neither firms obtaining new bank relationships, nor switching between existing relationships are driving the estimated effects.

**Robustness to differential credit demand potentially induced by the policy.** A concern is that eligible firms may realize that they have become cheaper to lend to as a result of the policy, which might induce an increase in credit demand that is not fully captured by a firm fixed effect (which is not time varying), and this induced demand could further differ by multi vs. single-bank status. However, if this effect were present, it would be an additional driver of the differential transmission we identify, rather than a threat to identification. Nonetheless, we believe this is unlikely to have occurred in practice, because, anecdotally, firms were largely unaware of the VLTRO policy. It was a complex policy that was directed towards banks, and it was the banks' decision whether to use loans to eligible firms as collateral – the only way to access the subsidy.

Nonetheless, we examine the role of differential demand by replacing the firm fixed effect with alternative time-varying controls that might capture this potential demand effect. Columns (3) and (4) of Appendix Table A3 replace the firm fixed effect with an interacted fixed effect vector that is time varying, following the narrow fixed effects approach in Degryse et al. (2019), which advocates size-industry-location-month fixed effects (used in column (4)) as effective controls for credit demand. Column (3) addresses "induced demand" even more directly, as the fixed effect is rating (the determinant of eligibility that could potentially induce demand) interacted with industry-location-month. Both specifications provide estimates similar to those from the baseline specification. Columns (3) and (4) suggest that there is no induced demand that may be driving our estimates.

Any differential demand (or supply) based on standard drivers of credit, such as firm size, profitability, and asset tangibility should be absorbed by the main specification's firm fixed effect together with the interactions of the pre-period levels of these variables with the $Post$ indicator. As a further robustness test, in column (5) we include the interaction of base-period (2011) leverage with $Post$, to capture differential trends associated with pre-determined leverage. However, because leverage is mechanically a first order determinant of credit ratings, leverage in December 2011 strongly predicts assignment to our rating groups in 2011. This means that we cannot include leverage as one of the covariates interacted with Post in the baseline specification: it is a "bad control," capturing part of the effect of being assigned to the treatment group. The high persistence of leverage also means that even 2010 leverage is a bad control, strongly predicting assignment to treatment groups in 2011. Thus, even though the coefficient in column (5) is still large and strongly statistically significant, it is downward biased and indicative only.

**Robustness to controlling for predicted credit rating upgrades.** Appendix Table A4 adds a control for predicted credit rating upgrades, using six alternate models to generate this measure. Results are statistically indistinguishable from our baseline estimates.

**Placebo treatment groups and placebo timing.** To explore the degree to which potentially confounding variation might be driving our estimated effects, in Figure A3 we show estimates of the effect of the VLTRO policy on firms' bank debt from thirty-six separate placebo analyses which vary (along the y-axis) the credit rating pairs that are being compared ("treated" vs. "control" rating category), and vary (along the x-axis) the policy's timing. We use our baseline specification (eq. 2), reporting the coefficient on $Treated \times Post$ and using a window of 6 months before to 6 months after each policy date (rather than 12 months) to avoid overlapping samples.

Each column reports the result of six different comparisons between credit rating categories. The middle column corresponds to the real timing of the VLTRO policy; the labels on the y-axis identify our main and spillover estimates. All other coefficients are from placebo analyses, in that they are comparisons between two rating categories that are equally eligible or ineligible, or because the timing is a year before or after the introduction of the VLTRO.

The figure indicates that, for single-bank firms, no differential credit flows occurred between any other pairs of credit ratings other than at the eligibility threshold, and this occurred only when the VLTRO was implemented. The multi-bank estimates similarly show large and statistically significant effects only for the expected rating comparisons (main effect and spillover).[^26]

[^26]: The exception to this is in the "5 vs. less" comparison a year after the VLTRO. While this may reflect expected statistical noise, were it to reflect a real relative shift in credit its distance from the eligibility threshold (both in time and rating category) means that it is unlikely to be an identification threat.

These placebo analyses indicate that any potentially confounding shocks or trends would have to affect only the rating categories at the eligibility threshold (and not any other comparison pair), and do so only at the time of VLTRO introduction. This evidence makes a potential "flight to quality" within bank portfolios extremely unlikely, especially given that there is no evidence of a flight from firms rated 5.

**Interpretation concerns: potential reallocation of credit away from control firms.** A potential interpretation of our results is that the policy induced banks to reallocate credit away from ineligible and towards eligible firms, rather than increasing overall credit. This seems implausible in the case of multi-bank firms, because Figure 3 shows a clear increase in debt at exactly the time the policy is implemented for the just-ineligible 5+ rated firms. We examine this spillover effect in detail in the following section.

For single-bank firms we examine whether ACC firms crowd out the credit of the most closely comparable but ineligible firms: those rated 5+. Column (6) of Table A2 compares the effect of the policy on firms rated 5+ with the also-ineligible rating group one notch below (rated 5). The estimated effect is very small and statistically insignificant, suggesting that our result is not driven by crowding out of existing credit to the closest substitute borrowers. The graphical evidence in Figures 2 and 3 also display no change in the credit trends of ineligible single-bank firms.

Finally, we corroborate that the effects we estimate are driven by the policy and not some alternate mechanism. In unreported regressions we replace the dependent variable with the sum of only those components of bank debt that are ineligible as collateral (e.g., leasing, credit lines). We find no effect for these types of bank debt.

### 5.4 Spillover lending

#### 5.4.1 Spillover: graphical evidence

The VLTROs incentivized new lending to eligible borrowers by allowing new debt to be used as ECB collateral, and also relaxed overall bank funding costs, by allowing banks to use some existing loans as collateral. However, banks were not required to use this additional financial slack to lend only to eligible borrowers. In fact, we find evidence that banks chose to also lend to a subset of multi-bank firms whose debt was ineligible as collateral: those in the just-ineligible credit rating one notch below eligibility.

Figure 3 provides clear graphical evidence of this spillover of additional lending onto some ineligible multi-bank firms. The bottom panel of Figure 3 displays debt growth over time for the two highest-rated ineligible categories (5 and 5+) for both single and multi-bank firms. Only just-ineligible multi-bank firms (i.e., rated 5+) see their debt rise sharply after the VLTRO program was introduced.[^27] Unreported regression estimates match the graphical evidence that single-bank firms do not receive spillover lending.

[^27]: We show only one year as a pre-period instead of the two years we have used in previous graphs. We do so because, unlike in our other graphs and tests, here we are comparing single to multi-bank firms, and their pre-trends diverge as we move further from the focal period where assignment to each group is determined (December 2011), and membership of each group becomes noisier. Nonetheless, our regressions all have a one year pre-period and a one year post-period, so this does not affect the regression results that follow.

### Figure 3: Examining the spillover

Panel (a): Multi-bank firms. Plots g(Debt) (y-axis, range -.15 to .25) against time (01jan2010 to 01jan2014) for three rating categories: ACC, 5+, and 5, with a vertical line at December 2011. Panel (b): Firms in the two highest-rated ineligible categories. Plots g(Debt) (y-axis, range -.1 to .3) against time (01jan2011 to 01jan2014) with four lines: 5+ single bank, 5+ multibank, 5 single bank, 5 multibank.

**Note:** The top figure shows the percentage change in firms' total bank debt (relative to their 2011 average) around the VLTRO policy (general announcement date: December 2011 – vertical line) for the treatment group (ACC or 4 rated firms) and for firms in the two credit rating notches below (5+ and 5, both ineligible). Assignment to credit rating groups is based on firms' ratings in December 2011. For each month we plot average firm debt growth: i.e., the cross-firm average $g_{ft} = \sum_b \text{Debt}_{fb(f)t}/\overline{\text{Debt}}_{f2011} - 1$, where f indexes firms and b banks, and the denominator is average debt in 2011. The bottom figure shows the average growth rate in debt around the policy for ineligible firms rated 5 and 5+, with lines for both single and multi-bank firms in a single figure.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

#### 5.4.2 Spillover: regression evidence

Table 3 estimates the size of spillover lending to ineligible firms by comparing just-ineligible 5+ rated multi-bank firms with firms rated 5, the next notch down. In column (1) we estimate the size of the spillover at 8.5 percentage points of additional lending to 5+ rated firms relative to 5 rated firms, mostly provided by the firms' main bank.[^28]

[^28]: In a specification analogous to the main bank ones in Table 2 the coefficient (s.e.) for debt growth from the main bank is 0.080 (0.019).

We then explore competition among banks at the geography × industry level as a potential driver of spillover lending: Di Maggio et al. (2020) shows that QE spillovers depend on the degree of market segmentation. To do this, we construct measures of local lending competition for each employment zone (EZ) in two ways. The first approach, employed in columns (2) and (3) of Table 3, defines a banking market by the firms located in each EZ and computes concentration measures (Herfindahl index and top 3 share) for all the lending to firms in each EZ and 1-digit industry. This approach captures the lending actually received by firms in each geography × industry cell.[^29] The second approach, employed in columns (4) and (5), defines a banking market by the bank branches located in each EZ and computes concentration measures for the lending by all branches in each EZ and industry. This approach captures how easy it might be for a firm to switch banks by finding another bank's local branch.

[^29]: We calculate competition by industry as well as geography following the recent literature showing that industry-based bank lending is a key driver of credit allocation (De Jonghe et al., 2020; Paravisini et al., 2023) and is prevalent in the SME credit market in France (Duquerroy et al., 2022).

To explore the role of competition as a mechanism for spillover lending we extend our baseline into a triple differences specification by adding interactions with above median competition indicators in each firm's geography×industry cell ($D_f$) as follows:

$$\begin{aligned} g_{ft} = \; & \beta_1(D_f \times Post_t) + \beta_2(D_f \times \text{ACC}_f \times Post_t) \\ & + \beta_0(\text{ACC}_f \times Post_t) + \alpha_f + \Lambda_{b(f)t} + \Upsilon_{i(f)t} + \Gamma(X_f \times Post_t) + \epsilon_{ft} \end{aligned} \tag{4}$$

The first row of Table 3 consistently shows that spillover lending is driven by more competitive markets (i.e., those with below-median HHI or top 3 share) for both measures of local banking competition. In unreported regressions we examine whether spillover lending is associated with a variety of observable firm characteristics: it is not. Nor is it associated with measures of banking relationship quality or by banks identifying firms that are subsequently upgraded into eligible credit ratings.[^30]

[^30]: When we estimate this regression on samples of firms with unchanged ratings for at least 6 months or 1 year we obtain coefficients of 0.093 (s.e. of 0.023) and 0.129 (s.e. of 0.028). These slightly larger coefficients push against the idea that the spillover is driven by 5+ firms being more likely to be upgraded than 5 firms. Similarly, Table A6 shows that the spillover estimate is robust to adding a variety of controls for predicted credit rating upgrades based on ex ante information.

This evidence suggests that banking competition is the key channel through which the unconventional monetary policy we examine is transmitted to firms with lower credit ratings. Competition may also play a role in the main effect of the ACC-VLTRO policy. In Table A7 we perform the same competition analysis but for our main samples that compare firms in eligible vs. ineligible rating categories, and find evidence that bank competition is associated with greater policy transmission for multi-bank firms. However, the standard errors on these estimates are large, and so the estimates are only statistically significant for some measures, and at the 10% level. For single-bank firms the point estimates suggest that greater competition reduces policy transmission (consistent with Petersen and Rajan, 1995), but these estimates are not statistically significant.

### Table 3: Policy Spillover onto ineligible Multi-bank firms

- **Table type:** Regression (triple difference, equation 4)
- **Sample:** Multi-bank firms rated 5+ or 5 (both categories are ineligible for the ACC program)
- **Dependent variable:** $g_{ft}$, debt growth, as in Table 2
- **Unit of observation:** firm-month
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | banking_market_definition | D_definition |
|---:|---|---|
| 1 | not applicable (baseline) | not applicable |
| 2 | Firm's industry/Firm's location | D = HHI below median |
| 3 | Firm's industry/Firm's location | D = Top-3 below median |
| 4 | Firm's industry/Branch's location | D = HHI below median |
| 5 | Firm's industry/Branch's location | D = Top-3 below median |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| Rating 5+×post×D | coefficient |  | 0.149** | 0.161** | 0.112** | 0.103** |
| Rating 5+×post×D | standard_error |  | 0.071 | 0.068 | 0.049 | 0.048 |
| Rating 5+×post | coefficient | 0.085*** | -0.050 | -0.060 | 0.001 | 0.008 |
| Rating 5+×post | standard_error | 0.020 | 0.068 | 0.065 | 0.045 | 0.044 |
| post×D | coefficient |  | -0.126** | -0.122** | -0.113*** | -0.081** |
| post×D | standard_error |  | 0.063 | 0.059 | 0.038 | 0.038 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y |
| N of clusters (firms) | 2,387 | 2,387 | 2,387 | 2,387 | 2,387 |
| Observations | 46,221 | 46,221 | 46,221 | 46,221 | 46,221 |
| R² | 0.50 | 0.50 | 0.50 | 0.50 | 0.50 |

**Note:** This is a triple difference estimation as in equation 4; the sample is multi-bank firms which are rated 5+ or 5 (both categories are ineligible for the ACC program). The dependent variable $g_{ft}$ is debt growth, as in Table 2. Columns (2) to (5) explore whether the competitiveness of banking markets within French employment zones (EZ) affect the transmission of the VLTRO to firms. We use the entire 2011Q4 credit registry data (not just our sample firms) to measure banking competition at the geography × industry level in two ways. In columns 2 and 3, we define a banking market by *the firms* located in each EZ, and use concentration measures for all the lending to firms in each EZ and 1-digit industry. In columns 4 and 5, we define a local banking market by *the bank branches* located in each EZ, and use concentration measures for the lending by all branches in each EZ and industry. These banking competitiveness measures are then merged to our sample by industry and "code commune" (~ zip code). D variables denote high competition in the local banking market: in columns (2) and (4), D is an indicator variable for when the HHI is below the sample median, i.e., when concentration is low and thus competition is likely to be high. In columns 3 and 5, D is an indicator for when the share of lending granted by the 3 largest lenders (branches) in the local market is below the sample median. Other variables are defined as in Table 2. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### 5.5 Policy transmission: debt pullbacks

We now examine the firms near the eligibility threshold whose total bank debt falls sharply during a period of macroeconomic stress; these are firms who are likely to be in weak financial health. Table 4 presents estimates using our main specification (equation 2), but with a different dependent variable: an indicator equal to one if a firm's total bank debt (across all banks) declines by more than twenty percent of their pre-period average level in a month. Large reductions in a firm's bank debt during a macroeconomic contraction are more likely to be driven by banks than by firms, consistent with the evidence in Chodorow-Reich et al. (2022) of banks cutting lending to SMEs during periods of financial system turbulence.

Table 4 provides evidence that there is attenuated pass-through of policy-driven lending to such firms when they are single-bank, relative to multi-bank. Column (1) examines outcomes one month after the second VLTRO round was implemented, while column (3) extends the post period to a year. Columns (1) to (3) show no change in the share of single-bank firms that see their total bank credit shrink significantly – that is, the policy appears do nothing to reduce banks materially tightening credit conditions for this set of single-bank firms.[^31] However, for multi-bank firms there is an immediate reduction in the share of firms whose total debt falls by at least one fifth: column (4) shows that even one month after implementation this transmission effect is detectable.

[^31]: Table A8 shows that results are unchanged if we use 5 rated firms as the comparison group for single-bank firms.

### Table 4: Effect of the VLTRO policy on sharp credit reductions

- **Table type:** Regression (difference in differences, equation 2)
- **Dependent variable:** indicator equal to one if a firm's debt falls more than 20 percent below its 2011 (pre-period) average level in a month
- **Unit of observation:** firm-month
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | sample | control_group | post_period_endpoint |
|---:|---|---|---|
| 1 | Single-bank | 5+ rated firms | March 2012 |
| 2 | Single-bank | 5+ rated firms | June 2012 |
| 3 | Single-bank | 5+ rated firms | Feb 2013 |
| 4 | Multi-bank | 5 rated firms | March 2012 |
| 5 | Multi-bank | 5 rated firms | June 2012 |
| 6 | Multi-bank | 5 rated firms | Feb 2013 |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.000 | -0.002 | 0.012 | -0.061*** | -0.051*** | -0.064*** |
| ACC×post | standard_error | 0.017 | 0.015 | 0.016 | 0.021 | 0.018 | 0.017 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Covariates x Post | Y | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y | Y |
| N of clusters (firms) | 2,799 | 2,803 | 2,806 | 3,606 | 3,647 | 3,724 |
| Observations | 29,817 | 37,828 | 58,992 | 36,824 | 46,851 | 73,348 |
| R² | 0.32 | 0.31 | 0.37 | 0.34 | 0.33 | 0.37 |

**Note:** This table presents difference in differences estimates from Equation 2, but with a dependent variable equal to one if a firm's debt falls more than 20 percent below its 2011 (pre-period) average level in a month. Columns 1 to 3 vary the end-point of the post period for single-bank firms; columns 4 to 6 do the same for multi-bank firms. Table A8 shows this analysis using 5 rated firms as the comparison group for single-bank firms. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

## 6 Bank relationships

### 6.1 Bank relationships and UMP transmission

Bank lending relationships have given rise to an expansive literature (Boot, 2000). They allow lenders to develop proprietary information about borrower quality via repeated interactions with the firm across a range of products (e.g., Agarwal and Hauswald, 2010; Becker et al., 2020; Berger and Udell, 2002; Cahn et al., 2023; Liberti and Petersen, 2019) and are especially important for SMEs. There are several reasons to expect differences in transmission along the single versus multi-bank dimension.

To begin with, asymmetric information gives banks greater hold-up power over single-bank borrowers, which is exacerbated in periods of macroeconomic stress when it becomes difficult to establish a new bank relationship (e.g., see Jiménez et al., 2012; Khwaja and Mian, 2008; Paravisini, 2008). Relationship lending models that incorporate aggregate fluctuations (e.g., Bolton et al., 2016; Hachem, 2011) also show banks providing continuation lending to their relationship borrowers in bad times, but prioritizing lending to high-type firms. Thus, these models predict positively selected transmission of monetary policy to single-bank firms, targeted especially to relationship borrowers about which the bank has better information.

By contrast, banks lending to multi-bank firms have less precise information – because each bank does not observe all the interactions between the firm and the financial system – and so have far more limited hold-up power. Multi-bank firms are thus better able to extract continuation lending via competition between their lenders, rather than through relationship lending. Consistent with this, recent theoretical and empirical work suggests that competition between banks affects the transmission of monetary policy to borrowers (Benetton and Fantino, 2021; Corbae and Levine, 2021; Wang et al., 2020). Thus, new lending to multi-bank firms should be less selective and less relationship-based. For example, the Rajan (1992) model predicts that, for firms with multiple lenders, less-informed outside banks will provide continuation lending in bad states with positive probability, regardless of firm quality.[^32]

[^32]: Relatedly, the Detragiache et al. (2000) model shows that multi-bank firms have greater credit access in crises as they are better diversified against bank-level shocks, while Degryse et al. (2019) highlights the importance of including single-bank firms in evaluating the effects of bank shocks over the business cycle.

In addition, strategic considerations that are absent for single-bank firms may play a role in generating differences in transmission to multi-bank firms. For example, a bank may choose to increase lending to a multi-bank borrower to reduce the risk that they strategically default. Alternatively, a firm's main bank may choose to increase lending to pre-empt the increase in default risk that would arise if the firm's other banks cut lending in response to macroeconomic conditions. In turn, this new lending from the main bank could increase other banks' willingness to lend to the firm (Giannetti and Saidi, 2019; Hertzberg et al., 2011).

### 6.2 Policy transmission and relationship quality

We use two measures of the strength of bank lending relationships, corresponding to the length and scope of lending relationships (Degryse and Van Cayseele, 2000). For each we create an indicator D that captures deeper bank relationships and estimate the triple-difference specification of equation 4. The first measure of lending relationship quality is an indicator for relationships of above-median duration.[^33] The second measure captures relationship scope, specifically how many bank products the firm makes use of, and to what extent it does so. We decompose each firm's bank financing into five categories: short-term credit, medium and long-term credit, accounts receivables financing, leasing, and undrawn credit lines. Using the share of each lending type we compute the HHI to measure the concentration of a firm's borrowing across bank products. An HHI measure below median (i.e., less concentrated across product types) thus indicates a lending relationship with a larger scope, with the lender and the borrower interacting across a greater range of financing products, generating more information for the bank. For multi-bank firms the LR and HHI measures are calculated for the main bank, as Table 2 shows that the main bank that drives much of the VLTRO effect.

[^33]: The average length of lending relationship may be longer, as our data is right-censored at 14 years: we cannot measure the length of relationships beginning before 1998.

The results in Table 5 show that – for single-bank firms – the additional lending attributable to the VLTRO policy is transmitted only to firms with deep lending relationships. Banks chose to focus policy-driven lending on single-bank firms about which they have more precise (and likely positive) quality signals. The first row of the table reports the triple-interaction coefficient and shows that treated single-bank firms with longer relationships (column 1) and with wider scope relationships (column 2) benefit more from the policy, with lending 7 to 12 percentage points higher than controls (similar results using 5 rated firms as controls are reported in Table A9). Further, the estimate in the second row suggests that most or all of the policy effect for single-bank firms is driven by firms with above median relationship quality.

However, in sharp contrast to the results for single-bank firms, bank-firm relationships do not appear to mediate VLTRO transmission for multi-bank firms: columns (3) and (4) indicate no appreciable difference for firms with deeper main bank lending relationships.

### Table 5: Effect of the VLTRO policy by depth of bank-firm relationship

- **Table type:** Regression (triple difference, equation 4)
- **Dependent variable:** $g_{ft}$, debt growth, as in Table 2
- **Unit of observation:** firm-month
- **Covariates:** firm characteristics (size, tangibility, profitability) as of 2011, interacted with Post
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | sample | D_definition |
|---:|---|---|
| 1 | Single bank (ACC vs. 5+) | D=1 if LR>median |
| 2 | Single bank (ACC vs. 5+) | D=1 if HHI<median |
| 3 | Multi-bank (ACC vs. 5) | D=1 if LR>median |
| 4 | Multi-bank (ACC vs. 5) | D=1 if HHI<median |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 |
|---|---|---:|---:|---:|---:|
| ACC×post×D | coefficient | 0.070** | 0.120*** | -0.014 | 0.020 |
| ACC×post×D | standard_error | 0.035 | 0.035 | 0.035 | 0.036 |
| ACC×post | coefficient | 0.042* | 0.017 | 0.109*** | 0.090*** |
| ACC×post | standard_error | 0.023 | 0.018 | 0.026 | 0.024 |
| post×D | coefficient | -0.015 | 0.053** | 0.006 | 0.021 |
| post×D | standard_error | 0.024 | 0.027 | 0.029 | 0.031 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 |
|---|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y |
| N of clusters (firms) | 2,806 | 2,806 | 3,724 | 3,724 |
| Observations | 58,992 | 58,992 | 73,348 | 73,348 |
| R² | 0.44 | 0.44 | 0.47 | 0.47 |

**Note:** This is a triple difference estimation (equation 4), and the dependent variable is debt growth, as in Table 2. D indicators capture higher bank-firm relationship quality. LR is the length of the lending relationship between the firm and its bank – above median indicates a relatively long firm-bank relationship. We also decompose each firm's bank financing into five categories: short-term credit, medium and long-term credit, accounts receivables financing, leasing, and undrawn credit lines. Using the share of each lending type we compute the firm's Herfindahl index (HHI) to measure the degree of concentration across products. An HHI measure below median (i.e., less concentrated across product types) is an indicator of a lending relationship with a wider scope, because the lender and the borrower interact across a greater range of financing products, generating more information for the bank. For multi-bank firms the LR and HHI measures are calculated for the main bank. Covariates are firm characteristics (size, tangibility, profitability) as of 2011, interacted with Post. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### 6.3 Lending maturity

Lending at longer horizons is essentially a different product to short-maturity lending: long maturities are riskier for banks, because they relinquish the real option to eliminate their exposure to a borrower in the intervening period. Further, banks' seniority as creditors is undercut if the firm obtains new shorter-term debt (even if it is junior). However, firms tend to prefer long-term debt for the reasons that banks dislike it, and also because it pushes rollover risk further into the future. Here we examine whether the information generated by lending relationships affects the maturity of policy-induced lending.[^34]

[^34]: Loan maturity typically falls during periods of aggregate financial stress, making long-maturity loans especially valuable. For example, in the US between May 2007 and May 2010 the average weighted maturity of new C&I loans with maturity of 1 to 12 months fell by over two thirds, while for loans with maturity over a year it fell by more than a quarter (US Survey of Terms of Business Lending).

The credit registry data separates total bank debt into short-term debt with initial maturity of less than a year (ST in the tables), and medium/long-term debt (MLT). If banks have more precise information about borrowers, as provided by banking relationships, they may be more willing to lend at longer maturities. In line with this logic, Table 6 shows that for single-bank firms the VLTRO drives an increase in longer maturity debt of around 7 percentage points (column 2), but the increase in short term debt (column 1) is not statistically distinguishable from zero. By contrast, for multi-bank firms the VLTRO generates an increase in short-term debt only (columns 5 and 6), despite the three year maturity of the VLTRO's lending to banks.[^35]

[^35]: Note that the magnitudes in Table 6 are higher because: (i) not all firms have short term debt or MLT debt, and so samples are smaller; (ii) because some firms have low amounts of such debt in the base period, magnifying the size of percentage increases.

Columns (3), (4), (7) and (8) in Table 6 include an interaction with an indicator for above median quality banking relationships (using our the scope measure described earlier). We obtain similar results using relationship length, but use lending scope as our main proxy for relationship quality. The results indicate that it is the single-bank firms with deeper lending relationships that receive long-term loans as a result of the policy.[^36] Lending relationships do not appear to affect which multi-bank firms receive additional short or longer-maturity lending.

[^36]: Table A9 shows that the results for single bank firms in Tables 5 and 6 hold if we use 5 rated firms as the control group, instead of 5+ rated firms.

Thus, the evidence in Table 6 reinforces the results from the previous subsection: the transmission of VLTRO liquidity is strongly mediated by bank relationships for single, but not for multi-bank firms. It also shows that multi-bank and single-bank firms receive different products from banks at this margin: those single-bank firms with deeper relationships are granted longer-term debt, while multi-bank firms receive short-term lending only (irrespective of the depth of the lending relationship).

### Table 6: Effect of the VLTRO policy on long and short term debt

- **Table type:** Regression (triple difference, equation 4)
- **Dependent variables:** percentage change in short-term debt, g(ST) (initial maturity below one year), and percentage change in medium/long-term debt, g(MLT)
- **Unit of observation:** firm-month
- **Covariates:** firm characteristics (size, tangibility, profitability) as of 2011, interacted with post
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | sample | dependent_variable | includes_D_interaction |
|---:|---|---|---|
| 1 | Single-bank (ACC vs. 5+) | g(ST) | No |
| 2 | Single-bank (ACC vs. 5+) | g(MLT) | No |
| 3 | Single-bank (ACC vs. 5+) | g(ST) | Yes (D=1 if HHI<median) |
| 4 | Single-bank (ACC vs. 5+) | g(MLT) | Yes (D=1 if HHI<median) |
| 5 | Multi-bank (ACC vs. 5) | g(ST) | No |
| 6 | Multi-bank (ACC vs. 5) | g(MLT) | No |
| 7 | Multi-bank (ACC vs. 5) | g(ST) | Yes (D=1 if HHI<median) |
| 8 | Multi-bank (ACC vs. 5) | g(MLT) | Yes (D=1 if HHI<median) |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| ACC×post×D | coefficient |  |  | 0.355 | 0.129*** |  |  | -0.099 | 0.119 |
| ACC×post×D | standard_error |  |  | 0.361 | 0.042 |  |  | 0.198 | 0.074 |
| ACC×post | coefficient | 0.145 | 0.073*** | -0.051 | 0.007 | 0.295*** | -0.002 | 0.388** | -0.061 |
| ACC×post | standard_error | 0.126 | 0.021 | 0.338 | 0.019 | 0.100 | 0.038 | 0.169 | 0.054 |
| post×D | coefficient |  |  | -1.056*** | 0.047 |  |  | -0.261 | -0.070 |
| post×D | standard_error |  |  | 0.254 | 0.033 |  |  | 0.170 | 0.070 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y | Y | Y | Y |
| N of clusters (firms) | 1,449 | 2,537 | 1,449 | 2,537 | 2,903 | 3,215 | 2,903 | 3,215 |
| Observations | 20,341 | 53,505 | 20,341 | 53,505 | 46,035 | 61,675 | 46,035 | 61,675 |
| R² | 0.51 | 0.59 | 0.51 | 0.59 | 0.53 | 0.62 | 0.53 | 0.62 |

**Note:** This is a triple difference estimation as in equation (4), but in this table we split our main dependent variable (percentage change in a firm's total bank debt) separately into percentage change in short term debt (initial maturity below one year, denoted by g(ST)) and medium/long-term debt (denoted by g(MLT)) respectively. The D variable is an indicator for a relatively deep (wide scope) banking relationship. We decompose each firm's bank financing into five categories: short-term credit, medium and long-term credit, accounts receivables financing, leasing, and undrawn credit lines. Using the share of each lending type we compute the firm's Herfindahl index (HHI) to measure the degree of concentration across products. An HHI measure below median (i.e., less concentrated across product types) is thus an indicator of a lending relationship with a wider scope, because the lender and the borrower interact across a greater range of financing products, generating more information for the bank. For multi-bank firms the HHI measure is calculated for the main bank. Covariates are firm characteristics (size, tangibility, profitability) as of 2011, interacted with post. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### 6.4 Do observable characteristics mediate policy transmission?

Next, we examine if banks are less likely to transmit VLTRO lending to firms with weaker observable characteristics, a simple proxy for lending standards. We use observables measured in the pre-period (2011) and for each we create an indicator D that captures relatively higher risk borrowers based on these variables. Specifically, we look at high leverage firms, those with low asset tangibility, and younger firms.

Table 7 presents the triple difference estimates. For single-bank firms (odd numbered columns) the negative coefficients on ACC × Post × D largely or completely offset the coefficients on ACC × Post. This indicates that the additional credit attributable to the VLTRO only flows, on average, to single-bank firms with stronger observables. The even columns of Table 7 repeat the analysis for multi-bank firms. Unlike for single-bank firms, for multi-bank firms there is no statistically significant effect of weak observables on lending. That is, multi-bank borrowers with weak observables were just as likely to receive policy-driven lending as borrowers with strong observables.

We perform two robustness tests on the finding that single-bank firms with weaker observables receive attenuated policy transmission. First, in Table A10 we show that the finding holds - but only weakly - if we use 5 rated firms as the control group for single-bank firms (instead of 5+). This is because the number of firms in the control group falls from around 1,100 to below 500, and while the coefficients are similar, the standard errors almost double, largely removing statistical significance. The Table also shows that the finding does hold if we add micro-firms to the sample so as to increase statistical power, but this change to the sample should be seen as illustrative only.

Second, we test whether the finding is driven by firms with weaker observables in 2011 being more likely to be downgraded into ineligibility. To do this we repeat the analysis using only those firms that do not change their ratings for 6 or 12 months.[^37] The coefficients in Table A11 are very similar to those in Table 7, suggesting that this finding is not driven by a correlation between observables and ex post downgrades.

[^37]: Note that requiring firms to maintain their rating biases the sample in potentially either direction. For example, if firms are likely to be downgraded on average, then requiring rating stability provides a selected sample of only the strongest firms, because they were not downgraded despite a trend in that direction. Thus, this is a robustness test only.

Summarizing, we find a difference between single vs. multi-bank difference in the importance of observable borrower characteristics for policy transmission, although we view this result as more suggestive than other results in the paper.

### Table 7: Effect of the VLTRO policy conditional on pre-period observables

- **Table type:** Regression (triple difference, equation 4)
- **Dependent variable:** bank debt growth, as in Table 2
- **Unit of observation:** firm-month
- **Covariates:** firm characteristics (size, tangibility, profitability) as of 2011, interacted with Post
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | D_definition | sample |
|---:|---|---|
| 1 | High Leverage | Single |
| 2 | High Leverage | Multi |
| 3 | Low Tangibles | Single |
| 4 | Low Tangibles | Multi |
| 5 | Young | Single |
| 6 | Young | Multi |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| ACC×post×D | coefficient | -0.108*** | 0.006 | -0.067* | 0.024 | -0.089** | 0.059 |
| ACC×post×D | standard_error | 0.031 | 0.035 | 0.035 | 0.043 | 0.038 | 0.065 |
| ACC×post | coefficient | 0.107*** | 0.097*** | 0.101*** | 0.097*** | 0.092*** | 0.097*** |
| ACC×post | standard_error | 0.024 | 0.023 | 0.022 | 0.021 | 0.021 | 0.019 |
| post×D | coefficient | 0.017 | -0.076*** | 0.048 | -0.007 | -0.005 | -0.084* |
| post×D | standard_error | 0.026 | 0.029 | 0.039 | 0.041 | 0.024 | 0.049 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y | Y |
| N of clusters (firms) | 2,806 | 3,724 | 2,806 | 3,724 | 2,806 | 3,724 |
| Observations | 58,992 | 73,348 | 58,992 | 73,348 | 58,992 | 73,348 |
| R² | 0.44 | 0.47 | 0.44 | 0.47 | 0.44 | 0.47 |

**Note:** This is a triple difference estimation as in equation (4), and the dependent variable is bank debt growth, as in Table 2. D indicators are proxies for observable firm characteristics measured in the pre-period. *High Leverage* is an indicator equal to one (D=1) for firm with average leverage in 2011 above the sample median. *Low Tangibles* is an indicator equal to one for firm with ratio of tangible assets to total assets in 2011 in the bottom quartile of the distribution. *Young* is an indicator equal to one if firm age is no greater than five years in 2011. Covariates are firm characteristics (size, tangibility, profitability) as of 2011, interacted with Post. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### 6.5 Differential transmission to single-bank firms in subsamples

If the differential transmission of UMP to single-bank firms we have documented is a structural feature of bank behavior, orthogonal to other firms' characteristics, it should be present even in subsamples defined by observable determinants of credit. If instead the differential transmission is an artifact of some other characteristics associated with our overall population of single-bank firms, then it is much less likely to persist in subsamples. We now turn to this test.

Table A12 splits firms into above and below median subsamples by leverage (the first two columns), asset tangibility (the next two columns) and firm age (final two columns). We run the same spillover analysis as in Table 3 and find consistent results in each of the six pairs of subsamples: spillover lending is present for multi-bank, but not single-bank firms.

We then examine whether deeper lending relationships matter in transmitting lending to firms in each subsample. Consistent with our full sample results in Table 5, Tables A13 and A14 show that relationship depth does not correlate with increased lending for multi-bank firms in any of these subsamples.

In contrast, for single-bank firms we see that relationship depth increases lending for several subsets of single-bank firms, specifically, firms with high leverage or low asset tangibility. Because these subsets capture the least creditworthy firms, ceteris paribus, this suggests that there is some substitutability between publicly and privately observable borrower information, with banks using more precise private information when observable characteristics are less favorable. In addition, Table A14 splits single-bank firms by age and shows that deeper lending relationships are associated with greater lending to older firms, but not younger ones. However, the lack of a positive association for younger firms may be mechanical: it takes time to build up a deep lending relationship.

Overall, we find very similar patterns of differential lending to single-bank firms relative to multi-bank ones in subsamples defined by firm characteristics, consistent with the idea that these patterns reflect pervasive differences in how banks treat these two groups of firms.

## 7 Real and Balance Sheet effects

In this section we use annual accounting data to explore the effects of the VLTRO policy on real and balance sheet outcomes. We combine the data from financial years 2010 and 2011 into a single pre-period (2012 and 2013 are the post-period), and run a two-period difference in differences design using fixed effects for firm, bank-time and industry-time, as well as the same controls interacted with the Post indicator used in the preceding regressions. Results are reported in Table 8.

Single-bank firms see their leverage rise by around 2 percentage points over this period, but despite this, their interest coverage ratio (ICR) rises by approximately 1 (relative to a pre-period mean of 18). That is, ex post, firms in the treatment group have both higher leverage and can more easily cover interest payments than controls. This likely reflects positive selection by banks in terms of which borrowers receive lending, within the group of single-bank firms, consistent with the results in the preceding section. Note that the change in ICR is not driven by a large change in interest rates paid by firms: their all-in cost of debt (calculated as total interest expenses over financial debt) remains unchanged in economic terms, falling by three basis points (column 3). The latter suggests that banks mainly adjusted lending on the quantity (and maturity) margin rather than on price. Turning to how firms employed the additional credit, total assets grow by almost 2 log points for single-bank firms (column 4), with a 2.6 percentage point relative increase in fixed asset investment (column 5).

Multi-bank firms also see their leverage increase, but they see the opposite result for the interest coverage ratio: it declines by around 1 (relative to a pre-period mean of around 20). This does not seem to be a price effect, as interest rates (approximated by cost of debt) also remain unchanged in economic terms (falling by 7bps). Instead it likely reflects a different firm population receiving credit, reinforcing the central finding that multi- and single-bank firms appear to receive differing treatment from banks. In turn, multi-bank firms use the additional resources differently to single-bank firms: perhaps because they receive short term lending only, total assets increase substantially (by over 6 log points), but investment does not.[^38]

[^38]: In unreported results we check for differences between two-bank and three or four bank firms in terms of the outcomes examined in Table 8. We find no robust differences across these sub-populations of multi-bank firms. We also check for evidence of zombie lending, and find no evidence that firms in the bottom quartiles of pre-period profitability or ICR receive more policy-driven lending.

### Table 8: Real and Balance Sheet effects from annual data

- **Table type:** Regression (two-period difference in differences using annual accounting data; fiscal years 2010-11 collapsed into a single pre-period, 2012-13 into a single post-period)
- **Specification:** $\text{LHS}_{ft} = \beta(\text{ACC}_f \times Post_t) + \lambda \text{Bank}_f \times Post_t + \Phi \text{Industry}_f \times Post_t + \Gamma' X_{ft} + \epsilon_{ft}$, where f indexes firm, t indexes time (pre or post)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | dependent_variable | category |
|---:|---|---|
| 1 | Leverage | Balance Sheet effects |
| 2 | ICR | Balance Sheet effects |
| 3 | Cost of Debt | Balance Sheet effects |
| 4 | Ln(Assets) | Real effects |
| 5 | Investment | Real effects |

#### Panel: Single-bank firms (ACC vs 5+)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.024*** | 0.924* | -0.003** | 0.019** | 0.026** |
| ACC×post | standard_error | 0.004 | 0.533 | 0.002 | 0.007 | 0.012 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y | Y |
| Bank-Post FE | Y | Y | Y | Y | Y |
| Industry-Post FE | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y |
| N of clusters (firms) | 2,577 | 2,545 | 2,577 | 2,577 | 1714 |
| Observations | 5,154 | 5,090 | 5,154 | 5,154 | 3,428 |
| R² | 0.95 | 0.81 | 0.82 | 0.99 | 0.59 |

#### Panel: Multi-bank firms (ACC vs 5)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.012*** | -0.889** | -0.007*** | 0.064*** | -0.008 |
| ACC×post | standard_error | 0.004 | 0.389 | 0.002 | 0.011 | 0.012 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y | Y |
| Bank-Post FE | Y | Y | Y | Y | Y |
| Industry-Post FE | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y |
| N of clusters (firms) | 3,882 | 3,865 | 3,882 | 3,882 | 2662 |
| Observations | 7,764 | 7,730 | 7,764 | 7,764 | 5,324 |
| R² | 0.90 | 0.78 | 0.80 | 0.99 | 0.62 |

**Note:** This table presents difference in differences estimates using annual accounting data, where fiscal years 2010-11 are collapsed into a single pre-period, and 2012-13 into a single post-period: $\text{LHS}_{ft} = \beta(\text{ACC}_f \times Post_t) + \lambda \text{Bank}_f \times Post_t + \Phi \text{Industry}_f \times Post_t + \Gamma' X_{ft} + \epsilon_{ft}$. Where f indexes firm, t indexes time (pre or post). Covariates are firm characteristics (size, tangibility, profitability) as of 2011, interacted with Post. Covariates also include lagged sales growth for the regressions on investment, as a proxy for investment opportunities as per standard investment regressions. Ln(Assets)= ln(Total Assets); Interest Coverage Ratio (ICR) = EBITDA / Interest Expenses; Cost of Debt (CoD) = Interest Expenses / Financial debt; Investment = ΔFixed Assets / Fixed Assets. All variables are winsorized at 1% except ICR and CoD that are winsorized at the 2% level, and the investment regression is run on firms that had investment of at least 1.5% of total fixed assets in the preceding year, to remove firms with minimal fixed asset investment. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

## 8 Other groups, across-bank and aggregate effects

Thus far we have compared the effect of the VLTRO policy on newly-eligible firms (rated 4/ACC) with the two never-eligible credit categories (5 and 5+) below it. We now evaluate the effect of the VLTRO policy on lending to firms rated above the newly-eligible category, using the same never-eligible controls (ratings of 5 and 5+).

VLTRO liquidity may have been very relevant to the higher-rated firms (loans to these firms had been eligible as ECB collateral for years) because the policy extended bank borrowing maturity to three years, and the collateral haircuts applied to bank loans were substantially lower for higher-rated firms, making the magnitude of the policy subsidy greater. Note also that always-eligible firms do not have to have been credit constrained ex ante in order to have demand for additional lending in a period of macroeconomic stress: increased precautionary demand for a cash buffer, reduced credit from suppliers, or reduced sales would all generate this demand.

### 8.1 Policy transmission to higher-rated (always-eligible) firms

Figure 5 graphs average debt growth relative to each firm's 2011 mean, by rating category. The figure excludes the 4/ACC category that we have been using thus far as a treatment group in order to focus attention on the higher-rated and always-eligible firms. Note that for this section we define groups using their ratings as of September 2011 (and the post indicator as of December 2011), because firms with ratings above 4/ACC were eligible to be used as collateral for the October 2011 one-year LTRO, and could be used as collateral in the first VLTRO round in late December 2011.

The figure shows a sharp increase in debt for always-eligible single and multi-bank firms after the policy was announced. It also provides strong evidence for parallel and nearly identical trends at a monthly frequency for the two years preceding the VLTRO policy shock for all the credit rating categories in the graph. Importantly, the pre-trends for single-bank are different to those of multi-bank firms for all the investment-grade rating categories, just as they were for ACC-rated firms, suggesting that banks treat single-bank firms differently across the ratings distribution.

### Figure 5: The VLTRO effect for higher rated (always eligible) firms

Panel (a): Single-bank firms. Panel (b): Multi-bank firms. Each panel plots g(Debt) (y-axis, range -.1 to .3) against time (01jan2010 to 01jan2014) with lines for rating categories 3+, 3, 4+, 5+, and 5, and a vertical line at December 2011.

**Note:** The figures show the average growth rate of debt around the VLTRO policy (general announcement date: December 2011 – vertical line) for always eligible firms (4+, 3 and 3+ rated firms which are, respectively, one, two and three notches higher than newly-eligible 4/ACC firms) and ineligible firms (5 and 5+ rated – one and two notches lower). 4/ACC rated firms are omitted for clarity. Firms are assigned to credit rating categories based on their credit rating in September 2011, because always-eligible firms were eligible for use as collateral for the October 2011 one-year LTRO. For each month we plot average firm debt growth: i.e., the cross-firm average of $g_{ft} = \sum_b \text{Debt}_{fb(f)t}/\overline{\text{Debt}}_{f2011} - 1$, where f indexes firms and b banks, and the denominator is average debt in 2011.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

Table 9 reports estimates of VLTRO pass-through to always-eligible categories of firms. Columns (1) and (5) show that the VLTROs induced a differential increase in debt of 10-12 percentage points for always-eligible firms relative to controls, which is of approximately the same magnitude as the effect for ACC firms. Columns (2) and (6) split the always-eligible firms into two groups, defined by the haircuts applied by the Eurosystem: the highest rated firms (rated 3++ and 3+), and the next two credit ratings (3 and 4+). The estimates for both groups are not statistically distinguishable. Columns (3) and (4) show that the estimates are almost identical if we use 5 rated firms as the control group for single-bank firms.

In addition, in the Appendix we present results showing that the same differences in policy transmission that we find between single- and multi-bank firms around the threshold are also present for higher-rated firms, with the natural exception of the spillover effect. Table A15 shows that deeper lending relationships increase the lending impact of the policy for single-bank firms, but not for multi-bank firms. Table A16 shows that additional lending to eligible single-bank firms is concentrated in medium and long term debt, while multi-bank firms instead receive shorter term debt. Finally, consistent with the results in Table 7, Table A17 shows that low tangibility and younger single-bank firms receive less credit than older single-bank firms and those with higher asset tangibility following the policy.[^39] Thus, the results in Tables 5, 6 and 7 for firms around the threshold appear to extend all the way up the credit rating distribution, supporting the idea that the single vs. multi-bank distinction is a structural feature of bank lending.

[^39]: The only result that does not generalize from Table 7 is for high leverage firms: for higher-rated firms, higher leverage reduces lending even for multi-bank firms.

### Table 9: Effect of the VLTRO policy on always-eligible higher-rated firms

- **Table type:** Regression (difference in differences, equation 2)
- **Dependent variable:** debt growth, as in Table 2
- **Treatment group:** firms rated above 4/ACC (always eligible as ECB collateral); groups defined using ratings as of September 2011
- **Covariates:** firm characteristics (size, tangibility, profitability) as of 2010, interacted with Post (defined as beginning in Dec. 2011 instead of Feb. 2012)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | sample | control_group | treated_group_structure |
|---:|---|---|---|
| 1 | Single-bank | 5+ rated firms | single treated group (all always-eligible) |
| 2 | Single-bank | 5+ rated firms | two treated groups (3++ and 3+; 3 and 4+) |
| 3 | Single-bank | 5 rated firms | single treated group (all always-eligible) |
| 4 | Single-bank | 5 rated firms | two treated groups (3++ and 3+; 3 and 4+) |
| 5 | Multi-bank | 5 rated firms | single treated group (all always-eligible) |
| 6 | Multi-bank | 5 rated firms | two treated groups (3++ and 3+; 3 and 4+) |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Eligible ×post | coefficient | 0.122*** |  | 0.118*** |  | 0.098*** |  |
| Eligible ×post | standard_error | 0.019 |  | 0.027 |  | 0.022 |  |
| Rating(3++ and 3+)×post | coefficient |  | 0.129*** |  | 0.132*** |  | 0.082*** |
| Rating(3++ and 3+)×post | standard_error |  | 0.027 |  | 0.035 |  | 0.031 |
| Rating(3 and 4+)×post | coefficient |  | 0.119*** |  | 0.116*** |  | 0.100*** |
| Rating(3 and 4+)×post | standard_error |  | 0.020 |  | 0.027 |  | 0.022 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Covariates x post Dec | Y | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y | Y |
| N of clusters (firms) | 3,838 | 3,838 | 3,357 | 3,357 | 4,232 | 4,232 |
| Observations | 87,061 | 87,061 | 75,702 | 75,702 | 92,131 | 92,131 |
| R² | 0.47 | 0.47 | 0.47 | 0.47 | 0.51 | 0.51 |

**Note:** This table presents difference in differences estimates as in Equation 2, and the dependent variable is debt growth, as in Table 2. The treatment group is firms rated above 4/ACC; loans to these firms were always eligible as ECB collateral. Note that here we define groups using their ratings as of September 2011, because firms with ratings above 4/ACC were eligible to be used as collateral for the October 2011 one-year LTRO. Columns 2, 4, and 6 extend the specification to have two treated groups (3++ and 3+ rated firms; and separately, 3 and 4+ rated firms) but they retain a single control group (firms rated 5+ in columns (1) and (2), the remaining columns use firms rated 5). Each rating within a treatment group has the same haircut applied when loans from those firms are used as collateral in the Eurosystem. Columns (1), (3), and (5) collapse both treated groups into a single group. Covariates are firm characteristics (size, tangibility, profitability) as of 2010, interacted with Post (defined as beginning in Dec. 2011 instead of Feb. 2012). Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### 8.2 Policy transmission to mid-sized and large firms

We now turn to the VLTRO policy's effect on larger, non-SME firms. These firms are almost always part of a business conglomerate, so we examine the debt growth of those group members with available accounting and rating data.

Using the same research design we used with always-eligible firms we find that the VLTRO caused an increase of around 10 percentage points in total bank debt for large and intermediate sized always-eligible firms (significant at the 1% level in unreported results). However, the effect seems to be driven by the very highest-rated firms, by multi-bank firms, and also by mid-sized firms (approximately, firms with 250 to 5,000 employees and sales (assets) below €1.5bn (€2bn)), rather than by the large firms, which are likely to be the least constrained. We find no debt increase for ACC-rated firms, or any spillover effects.

### 8.3 Cross-Bank heterogeneity of policy effects

Differences in the health of bank balance sheets could also have affected their transmission of VLTRO liquidity to borrowers. However, while France may appear to have many banks (as identified by their code interbancaire or CIB), in fact these banks are sub-entities of a handful of large banking groups. Moreover, the regulatory and financial constraints determining VLTRO uptake bind at the banking-group level rather than at the CIB level, and banking groups have active internal capital markets.[^40] This means that we have limited power to detect effects in a research design focused on cross-bank balance-sheet differences, because there are essentially only six bank groups in France.

[^40]: We thus measure all balance sheet strength variables (such as regulatory capital, funding costs, market value of equity) using the consolidated balance sheets of bank groups, instead of at the CIB level.

The columns in Appendix Table A18 display the results of adding an interacted indicator for several measures of bank group balance sheet strength (for the 6 largest banking groups, capturing over 97% of our sample) following equation 4. Data sources are listed in the Appendix. The estimates show that the main policy effect is not driven by cross-sectional differences in measures of bank-group-level balance sheet strength: funding cost, regulatory capital, or change in the market value of equity.

We also do not find that the policy effect is stronger for borrowers of bank groups with more VLTRO-eligible borrowers in their lending portfolios before the policy was implemented (columns 4 and 11), or with more ex ante un-pledged collateral (columns 5 and 12). We do find weak evidence that the banks that engaged in greater maturity extension as a result of the ECB's policy were more able to transmit more lending to their multi-bank borrowers (column 14), supporting the idea that the maturity extension component of the policy was at least as important as the magnitude of liquidity provided (as measured in columns 6 and 13). Overall, the coefficients on the interaction terms are small relative to the main effects, suggesting that cross-bank heterogeneity is not an important driver of the effects we find.

### 8.4 Aggregate VLTRO pass-through

Using our estimates of policy-induced debt growth for each combination of credit rating and single/multi-bank status we are able to calculate and compare the growth rates of total lending to the single and multi-bank firm categories, relative to December 2011 levels.

We observe weaker overall transmission of VLTRO liquidity to single-bank firms than to multi-bank firms: total lending to multi-bank firms grew 9.4% as a result of the policy, relative to growth of 6.1% for single bank firms. That is, growth of lending to multi-bank firms as a group grew by almost 60% more than lending to single-bank firms, largely (but not exclusively) driven by the absence of spillover lending to the latter group. Moreover, single-bank firms in the rating categories we examine received only 7% of the additional euro volume of lending to firms induced by the policy, despite accounting for around 11% of bank debt in 2011. Multi-bank firms received the rest.

While our methods are not ideally suited to this type of aggregate exercise, our estimates imply, ceteris paribus, that the VLTROs generated an additional €35bn of lending to firms by December 2012 (relative to total borrowing by French banks of €150bn). That is, absent the VLTROs, total credit to these firms would have decreased by around 10%, whereas the actual decrease was only 4%.

## 9 Conclusion

Large-scale unconventional central bank interventions have become a feature of the policy landscape since 2008, and banks serve as the main conduit through which central bank liquidity reaches most of the real economy. Understanding how banks choose to transmit policy funding, and whether there are differences in transmission across types of borrowers, is crucial for improving policy design and efficacy.

This paper examines ECB interventions that provided long-term debt to banks with the aim that this liquidity would be also be passed through to firms, especially SMEs. We show that a key determinant of policy transmission is whether firms have one or more banking relationships, consistent with standard models of relationship lending. In particular, we find that liquidity transmission is selective for single-bank firms, in contrast to the pass through to multi-bank firms, which are the focus of the empirical literature. Indeed, we show that policy-driven lending to single-bank firms is targeted at relationship borrowers, about whom the bank has better information, and at firms with stronger observables. While such patterns do not hold for multi-bank borrowers, our results suggest that the latter may be able to obtain credit through competition among their lenders.

Single-bank firms make up the majority of firms in many advanced and developing economies and employ a large share of the workforce, underlining their macroeconomic and political importance. They are also especially dependent on bank finance. Our findings highlight the need for greater attention to single-bank firms when studying the transmission of shocks in general, and of monetary policy in particular.

## References

Abbassi, Puriya, Rajkamal Iyer, Jose-Luis Peydro, and Francesc R. Tous (2016), "Securities trading by banks and credit supply: Micro-evidence from the crisis", Journal of Financial Economics 121.3, pp. 569–594.

Acharya, Viral, Heitor Almeida, Filippo Ippolito, and Ander Perez-Orive (2014), "Bank lines of credit as contingent liquidity: A study of covenant violations and their implications", Working Paper.

Adelino, Manuel, Miguel A Ferreira, Mariassunta Giannetti, and Pedro Pires (2022), "The role of trade credit in the transmission of unconventional monetary policy", Review of Financial Studies.

Agarwal, Sumit and Robert Hauswald (2010), "Distance and private information in lending", The Review of Financial Studies 23.7, pp. 2757–2788.

Aleksanyan, Lilia, Louis-Marie Harpedanne de Belleville, and Dominique Lefilliatre (2010), "Les déterminants de la multibancarité des entreprises en France", Bulletin de la Banque de France 180, pp. 33–47.

Amiti, Mary and David E. Weinstein (2017), "How much do idiosyncratic bank shocks affect investment? Evidence from matched bank-firm data", Journal of Political Economy.

Andrade, Philippe, Christophe Cahn, Henri Fraisse, and Jean-Stéphane Mésonnier (2018), "Can the Provision of Long-term Liquidity Help to Avoid a Credit Crunch? Evidence from the Eurosystem's LTRO", Journal of the European Economic Association.

Balyuk, Tetyana, Nagpurnanand R Prabhala, and Manju Puri (2020), "Indirect Costs of Government Aid and Intermediary Supply Effects: Lessons From the Paycheck Protection Program", NBER WP 28114.

Barthelemy, Jean, Vincent Bignon, and Benoit Nguyen (2017), "Illiquid Collateral and Bank Lending during the European Sovereign Debt Crisis", Banque de France Working Paper.

Beck, Thorsten, Hans Degryse, Ralph De Haas, and Neeltje Van Horen (2018), "When arm's length is too far: Relationship banking over the credit cycle", Journal of Financial Economics 127.1, pp. 174–196.

Becker, Bo, Marieke Bos, and Kasper Roszbach (2020), "Bad times, good credit", Journal of Money, Credit and Banking 52.S1, pp. 107–142.

Benetton, Matteo and Davide Fantino (2021), "Targeted Monetary Policy and Bank Lending Behavior", Journal of Financial Economics.

Berger, Allen N and Gregory F Udell (2002), "Small business credit availability and relationship lending: The importance of bank organisational structure", The Economic Journal 112.477, F32–F53.

Bignon, Vincent, Frederic Boissay, Christophe Cahn, and Louis-Marie Harpedanne de Belleville (2016), "Extended eligibility of credit claims for Eurosystem refinancing: Consequences for the supply of credit to companies", Banque de France Bulletin Quarterly Selection 43, pp. 15–23.

Bindseil, Ulrich, Marco Corsi, Benjamin Sahel, and Ad Visser (2017), "The Eurosystem collateral framework explained", ECB Occasional Paper.

Bolton, Patrick, Xavier Freixas, Leonardo Gambacorta, and Paolo Emilio Mistrulli (2016), "Relationship and Transaction Lending in a Crisis", Review of Financial Studies 29.10, pp. 2643–2676.

Bolton, Patrick and David S Scharfstein (1996), "Optimal debt structure and the number of creditors", Journal of Political Economy 104.1, pp. 1–25.

Bonfim, Diana, Gil Nogueira, and Steven Ongena (2021), ""Sorry, We're Closed" Bank Branch Closures, Loan Pricing, and Information Asymmetries", Review of Finance 25.4, pp. 1211–1259.

Boot, Arnoud WA (2000), "Relationship Banking: What Do We Know?", Journal of Financial Intermediation.

Boualam, Yasser (2018), "Credit markets and relationship capital", Working paper.

Caballero, Ricardo J. and Arvind Krishnamurthy (2008), "Collective risk management in a flight to quality episode", Journal of Finance 63.5, pp. 2195–2230.

Cahn, Christophe, Mattia Girotti, and Federica Salvade (2023), "Credit ratings and the hold-up problem in the loan market", Management Science.

Carpinelli, Luisa and Matteo Crosignani (2020), "The Design and Transmission of Central Bank Liquidity Provisions", forthcoming, Journal of Financial Economics.

CBS News (2020), "Biggest banks "prioritized" larger clients for small business loans, lawsuits claim", in: www.cbsnews.com/news/paycheck-protection-program-big-banks-loans-larger-clients-over-smaller-businesses (accessed 10/14/2021).

Chakraborty, Indraneel, Itay Goldstein, and Andrew MacKinlay (2019), "Monetary stimulus and bank lending", Journal of Financial Economics (Forthcoming).

Chava, Sudheer and Amiyatosh Purnanandam (2011), "The effect of banking crisis on bank-dependent borrowers", Journal of Financial Economics 99.1, pp. 116–135.

Chernenko, Sergey and Adi Sunderam (2014), "Frictions in shadow banking: Evidence from the lending behavior of money market mutual funds", The Review of Financial Studies 27.6, pp. 1717–1750.

Chodorow-Reich, Gabriel (2014), "The Employment Effects of Credit Market Disruptions: Firm-level Evidence from the 2008-09 Financial Crisis", Quarterly Journal of Economics 129.1, pp. 1–59.

Chodorow-Reich, Gabriel, Olivier Darmouni, Stephan Luck, and Matthew Plosser (2022), "Bank liquidity provision across the firm size distribution", Journal of Financial Economics, issn: 0304-405X, doi: https://doi.org/10.1016/j.jfineco.2021.06.035.

Corbae, Dean and Ross Levine (2021), "Competition, stability, and efficiency in the banking industry", Working Paper.

De Jonghe, Olivier, Hans Dewachter, Klaas Mulier, Steven Ongena, and Glenn Schepens (2020), "Some borrowers are more equal than others: Bank funding shocks and credit reallocation", Review of Finance 24.1, pp. 1–43.

Degryse, Hans, Olivier De Jonghe, Sanja Jakovljević, Klaas Mulier, and Glenn Schepens (2019), "Identifying credit supply shocks with bank-firm data: Methods and applications", Journal of Financial Intermediation 40, p. 100813.

Degryse, Hans and Patrick Van Cayseele (2000), "Relationship lending within a bank-based system: Evidence from European small business data", Journal of Financial Intermediation 9.1, pp. 90–109.

Detragiache, Enrica, Paolo Garella, and Luigi Guiso (2000), "Multiple versus Single Banking Relationships: Theory and Evidence", Journal of Finance 55.3, pp. 1133–1161.

Di Maggio, Marco, Amir Kermani, and Christopher J Palmer (2020), "How quantitative easing works: Evidence on the refinancing channel", The Review of Economic Studies 87.3, pp. 1498–1528.

Diamond, Douglas W. and Raghuram G. Rajan (2011), "Fear of fire sales, illiquidity seeking, and credit freezes", Quarterly Journal of Economics 126.2, pp. 557–591.

Drechsler, Itamar, Thomas Drechsel, David Marques-Ibanez, and Philipp Schnabl (2016), "Who borrows from the lender of last resort?", The Journal of Finance 71.5, pp. 1933–1974.

Duquerroy, Anne, Clément Mazet-Sonilhac, Jean-Stéphane Mésonnier, and Daniel Paravisini (2022), "Bank Local Specialization", Working paper.

Farinha, Luısa A and Joao AC Santos (2002), "Switching from single to multiple bank lending relationships: Determinants and implications", Journal of Financial Intermediation 11.2, pp. 124–151.

Financial Times (2013a), "An ECB funding for lending trial balloon", in: www.ft.com/content/3817dea5-cc87-3291-879a-607b62149e0c (accessed 10/14/2021).

Financial Times (2013b), "ECB considers further liquidity boost for European banks", in: www.ft.com/content/2103231a-2a99-11e3-8fb8-00144feab7de (accessed 10/14/2021).

Financial Times (2015), "Mario Draghi vindicated as court backs ECB bond-buying plan.", in: www.ft.com/content/c200c62e-1402-11e5-9bc5-00144feabdc0 (accessed 10/14/2021).

Financial Times (2018), "ECB to end QE at end of 2018", in: www.ft.com/content/4f459f68-6fc3-11e8-92d3-6c13e5c92914 (accessed 10/14/2021).

Financial Times (2020), "Where is my loan? Small businesses miss out on US rescue funds", in: www.ft.com/content/e6a06f94-5d2f-43a0-8aac-c7adddca0b0e (accessed 10/14/2021).

Fort, Teresa C, John Haltiwanger, Ron S Jarmin, and Javier Miranda (2013), "How firms respond to business cycles: The role of firm age and firm size", IMF Economic Review 61.3, pp. 520–559.

Galbraith, John Kenneth (1957), "Market structure and stabilization policy", Review of Economics and Statistics, pp. 124–133.

Garcia-Posada, Miguel and Marcos Marchetti (2016), "The bank lending channel of unconventional monetary policy: The impact of the VLTROs on credit supply in Spain", Economic Modelling 58, pp. 427–441.

Gertler, Mark and Simon Gilchrist (1994), "Monetary policy, business cycles, and the behavior of small manufacturing firms", Quarterly Journal of Economics 109.2, pp. 309–340.

Giannetti, Mariassunta and Farzad Saidi (2019), "Shock propagation and banking structure", Review of Financial Studies 32.7, pp. 2499–2540.

Gilchrist, Simon and Benoit Mojon (2017), "Credit risk in the euro area", The Economic Journal 128.608, pp. 118–158.

Gomez, Matthieu, Augustin Landier, David Sraer, and David Thesmar (2021), "Banks exposure to interest rate risk and the transmission of monetary policy", Journal of Monetary Economics 117, pp. 543–570.

Granja, Joao, Christos Makridis, Constantine Yannelis, and Eric Zwick (2020), "Did the Paycheck Protection Program Hit the Target?", NBER WP 27095.

Hachem, Kinda (2011), "Relationship lending and the transmission of monetary policy", Journal of Monetary Economics 58.6-8, pp. 590–600.

Heider, Florian, Marie Hoerova, and Cornelia Holthausen (2015), "Liquidity hoarding and interbank market rates: The role of counterparty risk", Journal of Financial Economics 118.2, pp. 336–354.

Hertzberg, Andrew, Jose Maria Liberti, and Daniel Paravisini (2011), "Public information and coordination: evidence from a credit registry expansion", Journal of Finance 66.2, pp. 379–412.

IMF (2013), "European Union: Publication of Financial Sector Assessment Program Documentation - Technical Note on Financial Integration and Fragmentation in the European Union", IMF Country Report No. 13/71.

Ippolito, Filippo, Ali K Ozdagli, and Ander Perez-Orive (2018), "The transmission of monetary policy through bank lending: The floating rate channel", Journal of Monetary Economics 95, pp. 49–71.

Ippolito, Filippo, Jose-Luis Peydro, Andrea Polo, and Enrico Sette (2016), "Double bank runs and liquidity risk management", Journal of Financial Economics 122.1, pp. 135–154.

Iyer, Rajkamal, Jose-Luis Peydro, Samuel da-Rocha-Lopes, and Antoinette Schoar (2014), "Interbank liquidity crunch and the firm credit crunch: Evidence from the 2007–2009 crisis", Review of Financial Studies 27.1, pp. 347–372.

Jasova, Martina, Caterina Mendicino, and Dominik Supera (2021), "Policy uncertainty, lender of last resort and the real economy", Journal of Monetary Economics 118, pp. 381–398.

Jeenas, Priit (2019), "Firm balance sheet liquidity, monetary policy shocks, and investment dynamics", Working paper.

Jiménez, Gabriel, Steven Ongena, José-Luis Peydró, and Jesús Saurina (2012), "Credit Supply and Monetary Policy: Identifying the Bank Balance-Sheet Channel with Loan Applications", American Economic Review 102.5, pp. 2301–2326.

Jiménez, Gabriel, Steven Ongena, José-Luis Peydró, and Jesús Saurina (2014), "Hazardous times for monetary policy: What do twenty-three million bank loans say about the effects of monetary policy on credit risk-taking?", Econometrica 82.2, pp. 463–505.

Jiménez, Gabriel, José-Luis Peydró, Rafael Repullo, and Jesus Saurina Salas (2018), "Burning Money? Government Lending in a Credit Crunch", CEPR Discussion Paper No. DP13267.

Khwaja, Asim Ijaz and Atif Mian (2008), "Tracing the impact of bank liquidity shocks: Evidence from an emerging market", American Economic Review 98.4, pp. 1413–1442.

Li, Lei and Philip E Strahan (2020), "Who Supplies PPP Loans (And Does It Matter)? Banks, Relationships and the COVID Crisis", NBER WP 28286.

Liberti, José María and Mitchell A Petersen (2019), "Information: Hard and soft", Review of Corporate Finance Studies 8.1, pp. 1–41.

Liberti, José María and Jason Sturgess (2018), "The anatomy of a credit supply shock: evidence from an internal credit market", Journal of Financial and Quantitative Analysis 53.2, pp. 547–579.

Luck, Stephan and Tom Zimmermann (2020), "Employment effects of unconventional monetary policy: Evidence from QE", Journal of Financial Economics 135.3, pp. 678–703.

Mésonnier, Jean-Stéphane, Charles O'Donnell, and Olivier Toutain (2017), "The Interest of Being Eligible", Working Paper.

Mullins, William and Patricio Toro (2018), "Credit Guarantees and New Bank Relationships", Working paper.

Ongena, Steven and David C Smith (2001), "The duration of bank relationships", Journal of Financial Economics 61.3, pp. 449–475.

Ottonello, Pablo and Thomas Winberry (2020), "Financial heterogeneity and the investment channel of monetary policy", Econometrica 88.6, pp. 2473–2502.

Paravisini, Daniel (2008), "Local bank financial constraints and firm access to external finance", Journal of Finance 63.5, pp. 2161–2193.

Paravisini, Daniel, Veronica Rappoport, and Philipp Schnabl (2023), "Specialization in bank lending: Evidence from exporting firms", Journal of Finance 78.4, pp. 2049–2085.

Paravisini, Daniel, Veronica Rappoport, Philipp Schnabl, and Daniel Wolfenzon (2014), "Dissecting the effect of credit supply on trade: Evidence from matched credit-export data", The Review of Economic Studies 82.1, pp. 333–359.

Petersen, Mitchell and Raghuram Rajan (1994), "The Benefits of Lending Relationships: Evidence from Small Business Data", Journal of Finance 49.1, pp. 3–37.

Petersen, Mitchell A. and Raghuram G. Rajan (1995), "The Effect of Credit Market Competition on Lending Relationships", Quarterly Journal of Economics 110.2, pp. 407–443.

Rajan, Raghuram G. (1992), "The Choice between Informed and Arm's-Length Debt", Journal of Finance 47.4, pp. 1367–1400.

Reuters (2018), "ECB considers further liquidity boost for European banks", in: www.reuters.com/article/us-eurozone-markets-ecb/r-i-p-quantitative-easing-five-questions-for-the-ecb-idUSKBN1O90LX (accessed 10/14/2021).

Rodnyansky, Alexander and Olivier M. Darmouni (2017), "The Effects of Quantitative Easing on Bank Lending Behavior", Review of Financial Studies 30.11.

Schnabl, Philipp (2012), "The International Transmission of Bank Liquidity Shocks: Evidence from an Emerging Market", Journal of Finance 67.3, pp. 897–932.

Sharpe, Steven A. (1990), "Asymmetric Information, Bank Lending, and Implicit Contracts: A Stylized Model of Customer Relationships", Journal of Finance 45.4, pp. 1069–1087.

Shleifer, Andrei and Robert W Vishny (2010), "Unstable banking", Journal of Financial Economics 97.3, pp. 306–318.

Thakor, Anjan V (2005), "Do loan commitments cause overlending?", Journal of Money, Credit and Banking, pp. 1067–1099.

Wang, Yifei, Toni M Whited, Yufeng Wu, and Kairong Xiao (2020), "Bank market power and monetary policy transmission: Evidence from a structural estimation", NBER Working Paper.

## Appendix to "Unconventional Monetary Policy and Bank Lending Relationships"

### Figure A1: Single- and multi-bank firm debt growth around the TLTROs

Four panels: TLTRO I (x-axis apr2013 to apr2015), TLTRO II (jan2015 to jan2017), TLTRO III (jan2018 to jan2020), and PELTRO (jan2019 to jan2021). Each panel plots g(Debt) (y-axis, range -.05 to .15) for two lines: Multi-bank (dashed) and Single-bank (solid). Printed vertical-line annotations: TLTRO I panel — "Draghi announces possible VLTRO", "Announcement", "1st implementation"; TLTRO II panel — "OMT declared legal", "Announcement", "1st implementation"; TLTRO III panel — "End of QE and Forward Guidance", "Announcement", "1st implementation"; PELTRO panel — "TLTRO III maturity extended from 2 to 3 years", "Announcement", "1st implementation".

**Note:** These plots are discussed in Appendix 1. The figure shows the percentage changes (between 0 and 1) in firms' total bank debt for eligible firms around the ECB's three TLTROs and the pandemic emergency LTRO (PELTRO). For each we define a one-year base period T (beginning two months before the announcement) and plot the monthly average change in firm debt (short plus long-term drawn debt) relative to the base period. Eligibility is defined by a firm's credit rating at the end of the base period. We classify firms as multi-bank if they borrow from >1 bank for at least one month during the base period. To prevent confounding from the State-guaranteed loan scheme (PGE) of March 2020, the base period for the PELTRO ends three months before the announcement, and we exclude short-term credit. Other sample constraints match those described in section 3.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A2: French Banks' equity and market funding cost

Panel (a): Equity values for listed French bank groups, 2010-2013. Lines for Crédit Agricole, Société Générale, Groupe BPCE, BNP Paribas, HSBC, indexed so December 2011 = 1.0; y-axis range 0.5 to 3.0. Vertical lines identify the two 3-year VLTROs. Panel (b): Market funding cost for French and Eurozone Banks, 2007-2013. Three lines: "Cost of market debt for Euro Area banks", "Cost of market debt for French banks", "ECB main refinancing operations rate"; y-axis range 0.0% to 6.5%.

**Note:** Panel (a) plots the monthly average stock price for the 5 largest publicly-listed French banking groups, as a fraction of each bank's December 2011 equity market value. The vertical lines identify the two 3-year VLTROs (Dec. 2011 and Feb. 2012). Panel (b) plots market funding costs for French and Euro area banks extracted from bond issues from Gilchrist and Mojon, 2017 – a proxy for banks' marginal longer-term funding cost. The ECB main refinancing rate (used for the bulk of Eurosystem liquidity) was the rate for VLTRO borrowing.

**Numerical data:** Not recovered from the plotted image. No plotted values are inferred.

### Figure A3: Placebo tests of main effect

Heatmap-style figures of coefficient estimates. Panel (a): Single-bank firms. Rows (credit rating comparison, "treated" rating vs "control" rating): 3++/3+ vs 3; 3 vs 4+; 4+ vs 4(ACC); 4(ACC) vs 5+ (Main comp.); 5+ vs 5; 5 vs less. Columns (policy date): 2011m2; 2012m2 (actual timing); 2013m2. Printed coefficient values by row (columns in order 2011m2, 2012m2, 2013m2): 3++/3+ vs 3: 0.039, 0.021, 0.018; 3 vs 4+: 0.006, 0.004, -0.020; 4+ vs 4(ACC): 0.018, 0.034, 0.012; 4(ACC) vs 5+ (Main comp.): -0.011, 0.075***, -0.006; 5+ vs 5: 0.019, -0.025, 0.042*; 5 vs less: -0.039, 0.023, 0.003.

Panel (b): Multi-bank firms. Rows: 3++/3+ vs 3; 3 vs 4+; 4+ vs 4(ACC); 4(ACC) vs 5 (Main comp.); 5+ vs 5 (Spillover); 5 vs less. Printed coefficient values by row (columns in order 2011m2, 2012m2, 2013m2): 3++/3+ vs 3: 0.004, 0.006, -0.003; 3 vs 4+: 0.032, 0.012, -0.030; 4+ vs 4(ACC): 0.004, 0.027*, 0.024; 4(ACC) vs 5 (Main comp.): 0.028, 0.064***, -0.003; 5+ vs 5 (Spillover): 0.033*, 0.059***, -0.027; 5 vs less: 0.030, 0.006, 0.074***.

**Note:** The figures show estimates of the effect of the VLTRO policy on firms' bank debt from multiple placebo analyses which vary (along the y-axis) the credit rating categories that are being compared ("treated" vs "control" rating category), and vary (along the x-axis) the policy's timing. The middle column corresponds to the true timing of the VLTRO policy; the comparisons of 4 vs 5+ and 4 vs 5 (for the multi-bank spillover) correspond to our main estimates (over a 6 month window). All other comparisons are placebo analyses. We use the baseline specification (Eq 2), but to avoid overlapping samples, we use a window of 6 months before to 6 months after each policy date (rather than 12 months). Firm ratings are determined two months before each policy date and the treated indicator identifies firms with the highest rating in each comparison pair. For consistency with the baseline, observations in January and February of each year are dropped. Cell shading reflects coefficient magnitude. We group ratings below five due to low firm density in these categories. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

*Conversion note: the in-figure coefficient values above are printed annotations transcribed from the figure cells, not values inferred from a plot.*

### Table A1: Robustness: Leverage as the dependent variable

- **Table type:** Regression (baseline specification, eq. 2)
- **Dependent variable:** firm leverage, $L_{ft} = (\sum_{b=1} \text{Debt}_{fb(f)t})/TA_{f2011}$, where $TA_{f2011}$ is the firm's total asset value in 2011
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | sample | control_group |
|---:|---|---|
| 1 | Single-bank | vs. 5+ |
| 2 | Single-bank | vs. 5 |
| 3 | Multi-bank | vs. 5+ |
| 4 | Multi-bank | vs. 5 |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 |
|---|---|---:|---:|---:|---:|
| ACC×post | coefficient | 0.017*** | 0.018*** | 0.010*** | 0.023*** |
| ACC×post | standard_error | 0.003 | 0.004 | 0.003 | 0.003 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 |
|---|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y |
| N of clusters (firms) | 2,855 | 2,277 | 4,746 | 3,751 |
| Observations | 58,709 | 49,574 | 92,625 | 72,886 |
| R² | 0.93 | 0.91 | 0.86 | 0.86 |

**Note:** This table presents estimates from our baseline specification (eq. 2) using firm leverage as the dependent variable: Leverage is the sum of the firm's debt across all banks, scaled by total assets: $L_{ft} = (\sum_{b=1} \text{Debt}_{fb(f)t})/TA_{f2011}$, where $TA_{f2011}$ is the firm's total asset value in 2011. All other variables follow those in Table 2. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A2: Robustness: Alternate dependent variables

- **Table type:** Regression (equation 2)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level
- All models include: Covariates x post, Bank-Month FE, Industry-Qtr FE, Firm FE

#### Panel: Single-bank firms (ACC vs 5+)

##### Column metadata

| model | dependent_variable | notes |
|---:|---|---|
| 1 | Ln(Debt) |  |
| 2 | Leverage | using 2011 total assets |
| 3 | debt growth | alternate scaling: average debt in 2010 |
| 4 | debt growth | alternate scaling: average debt in 2011s1 |
| 5 | debt growth | alternate scaling: average debt in 2011s2 |
| 6 | debt growth | crowding out test: 5+ vs. 5 (single-bank firms only) |

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.051*** | 0.017*** | 0.079*** | 0.082*** | 0.060*** |  |
| ACC×post | standard_error | 0.016 | 0.003 | 0.022 | 0.017 | 0.016 |  |
| Rating 5+×post | coefficient |  |  |  |  |  | -0.016 |
| Rating 5+×post | standard_error |  |  |  |  |  | 0.024 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 2,793 | 2,855 | 2,618 | 2,746 | 2,775 | 1,453 |
| Observations | 58,265 | 58,709 | 55,427 | 58,370 | 58,773 | 30,898 |
| R² | 0.93 | 0.93 | 0.76 | 0.51 | 0.36 | 0.44 |

#### Panel: Multi-bank firms (ACC vs 5)

##### Column metadata

| model | dependent_variable | notes |
|---:|---|---|
| 1 | Ln(Debt) |  |
| 2 | Leverage | using 2011 total assets |
| 3 | debt growth | alternate scaling: average debt in 2010 |
| 4 | debt growth | alternate scaling: average debt in 2011s1 |
| 5 | debt growth | alternate scaling: average debt in 2011s2 |

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.088*** | 0.023*** | 0.113*** | 0.110*** | 0.088*** |
| ACC×post | standard_error | 0.019 | 0.003 | 0.022 | 0.018 | 0.017 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| N of clusters (firms) | 3,711 | 3,751 | 3,515 | 3,498 | 3,540 |
| Observations | 72,615 | 72,886 | 69,468 | 70,987 | 71,931 |
| R² | 0.90 | 0.86 | 0.77 | 0.56 | 0.40 |

**Note:** This table presents results from estimating equation 2. Columns 1-2 use alternate dependent variables: ln(debt) and leverage (using 2011 total assets). Columns 3-5 present alternate formulations of our main dependent variable: instead of using the firm's average debt in 2011 to scale the firm's current debt (i.e., $\overline{\text{Debt}}_{f,2011}$ in the formula $g_{f,t} = \sum_b \text{Debt}_{f,b(f),t}/\overline{\text{Debt}}_{f,2011} - 1$), we use average debt in 2010, the first semester of 2011 and the second semester, respectively. Column 6, for single-bank firms only, compares the effect of the policy on the control group (rated 5+) with a similarly ineligible rating group one notch below (rated 5), to examine whether ACC firms are receiving credit by crowding out the most closely comparable but ineligible firms (i.e., the 5+ firms). Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A3: Robustness: Alternate fixed effects and clustering

- **Table type:** Regression (variants of baseline specification, equation 2)
- **Dependent variable:** firm debt growth
- **Standard errors:** clustered by firm unless otherwise noted, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | variant |
|---:|---|
| 1 | Double clusters (by firm and by bank-month) |
| 2 | Bank-firm FE added |
| 3 | Rating-plus FE (Rating-Ind-Loc-Time FE replaces firm FE) |
| 4 | Size-plus FE (Size-Ind-Loc-Time FE replaces firm FE) |
| 5 | Lev.x Post (2011 leverage added to covariates interacted with Post) |

#### Panel: Single-bank firms (ACC vs 5+)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.082*** | 0.082*** | 0.093*** | 0.071*** | 0.062*** |
| ACC×post | standard_error | 0.018 | 0.017 | 0.035 | 0.024 | 0.019 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| N of clusters (firms) | 2,806 | 2,806 | 2,541 | 2,286 | 2,806 |
| N of clusters (Bank-Month) | 372 | . | . | . | . |
| Observations | 58,992 | 58,934 | 45,886 | 47,525 | 58,992 |
| R² | 0.44 | 0.47 | 0.61 | 0.58 | 0.44 |

#### Panel: Multi-bank firms (ACC vs 5)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.102*** | 0.089*** | 0.117* | 0.138*** | 0.099*** |
| ACC×post | standard_error | 0.019 | 0.019 | 0.061 | 0.026 | 0.019 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| N of clusters (firms) | 3,724 | 3,719 | 3,382 | 3,191 | 3,724 |
| N of clusters (Bank-Month) | 483 | . | . | . | . |
| Observations | 73,348 | 72,483 | 56,954 | 61,003 | 73,348 |
| R² | 0.47 | 0.58 | 0.63 | 0.62 | 0.47 |

#### Fixed effects and controls by model (both panels)

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y |  |  | Y |
| Firm FE | Y |  | Y | Y | Y |
| Bank-Firm FE |  | Y |  |  |  |
| Rating-Ind-Loc-Time FE |  |  | Y |  |  |
| Size-Ind-Loc-Time FE |  |  |  | Y |  |
| Leverage x post |  |  |  |  | Y |

**Note:** This table presents results from estimating variants of our baseline specification (equation 2); the dependent variable is firm debt growth. Column 1 clusters standard errors by both firm and by bank-month. Column 2 adds a bank-firm fixed effect. Columns 3 and 4 replace the firm fixed effect with alternative fixed effects: respectively Rating notches or Size terciles x Industry x Location x Month, where location is Département (~ US county). Column 5 adds 2011 leverage to the covariates interacted with Post. Unless otherwise noted, standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A4: Robustness: Controlling for predicted credit rating upgrades

- **Table type:** Regression (equation 2, with predicted upgrade control)
- **Dependent variable:** firm debt growth as in Table 2
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level
- All models include: Covariates x Post, Bank-Month FE, Industry-Qtr FE, Firm FE

#### Column metadata

| model | predictive_model | variable_set |
|---:|---|---|
| 1 | Baseline (no upgrade control) | not applicable |
| 2 | LPM | not applicable |
| 3 | GSReg | not applicable |
| 4 | Lasso | set #1 |
| 5 | Lasso | set #2 |
| 6 | Ridge | set #1 |
| 7 | Ridge | set #2 |

#### Panel: Single-bank firms (ACC vs 5+)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.082*** | 0.075*** | 0.083*** | 0.083*** | 0.083*** | 0.083*** | 0.083*** |
| ACC×post | standard_error | 0.018 | 0.020 | 0.021 | 0.018 | 0.018 | 0.018 | 0.018 |
| P(Upgrade)×post | coefficient |  | 0.117 | -0.008 | -0.125 | -0.150 | -0.124 | -0.155 |
| P(Upgrade)×post | standard_error |  | 0.144 | 0.144 | 0.136 | 0.194 | 0.139 | 0.195 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---:|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 2,806 | 2,806 | 2,704 | 2,806 | 2,694 | 2,806 | 2,694 |
| Observations | 58,992 | 58,992 | 56,832 | 58,992 | 56,693 | 58,992 | 56,693 |
| R² | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 |

#### Panel: Single-bank firms (ACC vs 5)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.073*** | 0.050* | 0.066** | 0.090*** | 0.082*** | 0.090*** | 0.082*** |
| ACC×post | standard_error | 0.025 | 0.029 | 0.030 | 0.029 | 0.031 | 0.029 | 0.031 |
| P(Upgrade)×post | coefficient |  | 0.290* | 0.107 | 0.161 | 0.075 | 0.168 | 0.072 |
| P(Upgrade)×post | standard_error |  | 0.149 | 0.145 | 0.160 | 0.196 | 0.161 | 0.197 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---:|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 2,218 | 2,218 | 2,140 | 2,218 | 2,124 | 2,218 | 2,124 |
| Observations | 46,359 | 46,359 | 44,695 | 46,359 | 44,446 | 46,359 | 44,446 |
| R² | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 |

#### Panel: Multi-bank firms (ACC vs 5)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.102*** | 0.101*** | 0.107*** | 0.094*** | 0.083*** | 0.095*** | 0.083*** |
| ACC×post | standard_error | 0.019 | 0.019 | 0.020 | 0.022 | 0.025 | 0.022 | 0.025 |
| P(Upgrade)×post | coefficient |  | 0.011 | -0.082 | -0.067 | -0.160 | -0.058 | -0.164 |
| P(Upgrade)×post | standard_error |  | 0.103 | 0.099 | 0.095 | 0.132 | 0.096 | 0.133 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---:|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 3,724 | 3,724 | 3,656 | 3,724 | 3,648 | 3,724 | 3,648 |
| Observations | 73,348 | 73,348 | 71,908 | 73,348 | 71,735 | 73,348 | 71,735 |
| R² | 0.47 | 0.47 | 0.47 | 0.47 | 0.47 | 0.47 | 0.47 |

**Note:** The dependent variable is firm debt growth as in Table 2. Column (1) reproduces the specification in Table 2 before adding the predicted likelihood of a credit rating upgrade within a year (as of 2011), interacted with the post indicator. P(Upgrade) is an indicator at date N equal to 1 if the firm's credit rating was raised in year N + 1 and 0 otherwise. We use a firm-year dataset which parallels the data sources and cleaning procedures used in the paper, covering 2004-2011. We use four alternative predictive models to generate P(Upgrade). (i) a Linear Probability Model (LPM), using the following independent variables (from Cahn et al., 2023): operating margin, interest coverage, debt-equity ratio, and ln(assets), both in levels and first differences, as well as fixed effects for rating category, firm and industry-by-year. (ii) a Global Search Regression (GSreg) model, in which we employ the four main variables from the LPM in levels, the same fixed effects, and also the investment rate, ln(headcount), capital expenditure, trade credit, and cash holdings. (iii) LASSO and (iv) Ridge models. For the latter two models the training subset contains all years but 2011. The models are then applied to the second subsample (2011) to calculate the predicted probability of upgrade. We use two sets of variables for these models. The primary set (set #1) uses the four variables from the LPM in levels, plus rating and industry variables, alongside all variable interactions (including second-order terms). Set #2 uses the nine GSReg model variables plus six others (dividends, cash flows, leasing, securities, bonds, and bank loans) and their first differences, as well as ratings and sector classifications. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A5: Robustness: Differing sample definitions

- **Table type:** Regression (baseline specification, equation 2)
- **Dependent variable:** firm debt growth as in Table 2
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | sample | rating_assignment_month |
|---:|---|---|
| 1 | Single-bank (ACC vs. 5+) | Baseline (December 2011) |
| 2 | Single-bank (ACC vs. 5+) | Nov11 |
| 3 | Single-bank (ACC vs. 5+) | Oct11 |
| 4 | Single-bank (ACC vs. 5+) | Sep11 |
| 5 | Multibank (ACC vs. 5) | Baseline (December 2011) |
| 6 | Multibank (ACC vs. 5) | Nov11 |
| 7 | Multibank (ACC vs. 5) | Oct11 |
| 8 | Multibank (ACC vs. 5) | Sep11 |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| ACC×post | coefficient | 0.082*** | 0.081*** | 0.084*** | 0.078*** | 0.102*** | 0.106*** | 0.105*** | 0.089*** |
| ACC×post | standard_error | 0.018 | 0.018 | 0.018 | 0.018 | 0.019 | 0.019 | 0.018 | 0.019 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y | Y | Y | Y |
| N of clusters (firms) | 2,806 | 2,756 | 2,725 | 2,700 | 3,724 | 3,673 | 3,652 | 3,605 |
| Observations | 58,992 | 57,897 | 57,252 | 56,753 | 73,348 | 72,309 | 71,794 | 70,866 |
| R² | 0.44 | 0.44 | 0.43 | 0.43 | 0.47 | 0.47 | 0.47 | 0.47 |

**Note:** This table presents results from estimating our baseline specification (equation 2); the dependent variable is firm debt growth as in Table 2. Columns 1 and 5 provide our baseline results based on firms being assigned to rating groups (i.e., treatment and control categories) based on their ratings as of December 2011. The other columns estimate the same equation using samples defined by firms' ratings as of earlier months: September, October, and November 2011. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A6: Robustness: Controlling for predicted credit rating upgrades in Spillover analysis

- **Table type:** Regression (spillover analysis of Table 3 with predicted upgrade control)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level (stars appear in table; legend follows the paper's convention as stated in Table A4's note)
- All models include: Covariates x Post, Bank-Month FE, Industry-Qtr FE, Firm FE

#### Column metadata

| model | predictive_model | variable_set |
|---:|---|---|
| 1 | Baseline (no upgrade control) | not applicable |
| 2 | LPM | not applicable |
| 3 | GSReg | not applicable |
| 4 | Lasso | sample #1 |
| 5 | Lasso | sample #2 |
| 6 | Ridge | sample #1 |
| 7 | Ridge | sample #2 |

#### Panel: Single-bank firms (5 vs 5+)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| Rating 5+×post | coefficient | -0.016 | -0.022 | -0.022 | -0.014 | -0.010 | -0.013 | -0.011 |
| Rating 5+×post | standard_error | 0.024 | 0.025 | 0.026 | 0.025 | 0.027 | 0.025 | 0.027 |
| P(Upgrade)×post | coefficient |  | 0.201 | 0.189 | 0.020 | 0.063 | 0.025 | 0.061 |
| P(Upgrade)×post | standard_error |  | 0.130 | 0.137 | 0.119 | 0.151 | 0.121 | 0.152 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---:|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 1,453 | 1,453 | 1,387 | 1,453 | 1,379 | 1,453 | 1,379 |
| Observations | 30,898 | 30,898 | 29,481 | 30,898 | 29,348 | 30,898 | 29,348 |
| R² | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 |

#### Panel: Multi-bank firms (5+ vs 5)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| Rating 5+×post | coefficient | 0.085*** | 0.085*** | 0.086*** | 0.079*** | 0.070*** | 0.079*** | 0.070*** |
| Rating 5+×post | standard_error | 0.020 | 0.020 | 0.020 | 0.022 | 0.023 | 0.023 | 0.023 |
| P(Upgrade)×post | coefficient |  | 0.011 | -0.038 | -0.056 | -0.151 | -0.053 | -0.152 |
| P(Upgrade)×post | standard_error |  | 0.106 | 0.096 | 0.103 | 0.117 | 0.104 | 0.117 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---:|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 2,387 | 2,387 | 2,322 | 2,387 | 2,316 | 2,387 | 2,316 |
| Observations | 46,221 | 46,221 | 44,906 | 46,221 | 44,776 | 46,221 | 44,776 |
| R² | 0.50 | 0.50 | 0.50 | 0.50 | 0.50 | 0.50 | 0.50 |

**Note:** This Table employs the same analysis described in the note to Table A4 to explore whether the spillover analysis in Table 3 is robust to including the predicted probability of a credit rating upgrade as of 2011 as a control.

### Table A7: Does Bank Competition mediate the transmission of lending to eligible firms?

- **Table type:** Regression (triple difference; reproduces the bank competition analysis of Table 3 for the main effect)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level
- All models include: Covariates x Post, Bank-Month FE, Industry-Qtr FE, Firm FE

#### Column metadata

| model | banking_market_definition | D_definition |
|---:|---|---|
| 1 | not applicable (baseline) | not applicable |
| 2 | Firm's industry/Firm's location | D = HHI below median |
| 3 | Firm's industry/Firm's location | D = Top-3 below median |
| 4 | Firm's industry/Branch's location | D = HHI below median |
| 5 | Firm's industry/Branch's location | D = Top-3 below median |

#### Panel: Single-bank firms (ACC vs 5+)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| ACC×post×D | coefficient |  | -0.063 | -0.080 | -0.068 | -0.039 |
| ACC×post×D | standard_error |  | 0.052 | 0.049 | 0.044 | 0.045 |
| ACC×post | coefficient | 0.082*** | 0.140*** | 0.154*** | 0.135*** | 0.112*** |
| ACC×post | standard_error | 0.018 | 0.048 | 0.045 | 0.040 | 0.040 |
| post×D | coefficient |  | 0.054* | 0.072** | 0.027 | 0.001 |
| post×D | standard_error |  | 0.031 | 0.028 | 0.028 | 0.029 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| N of clusters (firms) | 2,806 | 2,806 | 2,806 | 2,806 | 2,806 |
| Observations | 58,992 | 58,992 | 58,992 | 58,992 | 58,992 |
| R² | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 |

#### Panel: Multi-bank firms (ACC vs 5)

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---|---:|---:|---:|---:|---:|
| ACC×post×D | coefficient |  | 0.084 | 0.109* | 0.074* | 0.061 |
| ACC×post×D | standard_error |  | 0.069 | 0.066 | 0.044 | 0.044 |
| ACC×post | coefficient | 0.102*** | 0.025 | 0.004 | 0.046 | 0.056 |
| ACC×post | standard_error | 0.019 | 0.067 | 0.064 | 0.041 | 0.041 |
| post×D | coefficient |  | -0.125** | -0.124** | -0.119*** | -0.102*** |
| post×D | standard_error |  | 0.061 | 0.058 | 0.037 | 0.038 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 |
|---|---:|---:|---:|---:|---:|
| N of clusters (firms) | 3,724 | 3,724 | 3,724 | 3,724 | 3,724 |
| Observations | 73,348 | 73,348 | 73,348 | 73,348 | 73,348 |
| R² | 0.47 | 0.47 | 0.47 | 0.47 | 0.47 |

**Note:** This reproduces the bank competition-based analysis of Table 3 to explore the main effect of the ACC-VLTRO policy examined in Table 2. D indicates above-median competitiveness of the geography× industry banking market. In columns (2) and (4), D is an indicator for when the HHI is below the sample median, i.e., when banking concentration is low. In columns 3 and 5, D is an indicator for when the share of lending granted by the 3 largest lenders (branches) in the local market is below the sample median. The top panel uses single-bank firms and compares eligible firms (ACC rated) to 5+ rated firms. The bottom panel uses multi-bank firms and compares eligible firms (ACC rated) to 5 rated firms. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level

### Table A8: Robustness for Table 4 (Single-bank firms). Control group: 5-rated firms

- **Table type:** Regression (replicates Table 4 for single-bank firms using 5-rated firms as the control group)
- **Sample:** Single-bank (ACC vs. 5)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | post_period_endpoint |
|---:|---|
| 1 | March 2012 |
| 2 | June 2012 |
| 3 | Feb 2013 |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 |
|---|---|---:|---:|---:|
| ACC×post | coefficient | -0.016 | 0.016 | 0.023 |
| ACC×post | standard_error | 0.023 | 0.020 | 0.021 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 |
|---|---:|---:|---:|
| Covariates x Post | Y | Y | Y |
| Bank-Month FE | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y |
| Firm FE | Y | Y | Y |
| N of clusters (firms) | 2,210 | 2,212 | 2,218 |
| Observations | 23,443 | 29,736 | 46,359 |
| R² | 0.32 | 0.31 | 0.35 |

**Note:** This Table replicates Table 4 for single-bank firms using 5-rated firms as the control group in place of 5+ rated firms. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A9: Robustness for Tables 5 and 6 (Single-bank firms). Control group: 5-rated firms

- **Table type:** Regression (reproduces main single-bank analyses of Tables 5 and 6 using 5-rated firms as the control group)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level
- D=1 if HHI<median (columns 2-5)

#### Column metadata

| model | dependent_variable | includes_D_interaction |
|---:|---|---|
| 1 | g(Total D) | No |
| 2 | g(Total D) | Yes |
| 3 | g(ST) | Yes |
| 4 | ST/TotalDebt | Yes |
| 5 | g(MLT) | Yes |
| 6 | g(ST) | No |
| 7 | ST/TotalDebt | No |
| 8 | g(MLT) | No |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| ACC×post×D | coefficient |  | 0.126*** | -0.120 | -0.025 | 0.146** |  |  |  |
| ACC×post×D | standard_error |  | 0.048 | 0.370 | 0.039 | 0.058 |  |  |  |
| ACC×post | coefficient | 0.073*** | 0.005 | 0.660* | 0.039 | 0.012 | 0.513*** | 0.024 | 0.085*** |
| ACC×post | standard_error | 0.025 | 0.032 | 0.350 | 0.036 | 0.035 | 0.132 | 0.016 | 0.032 |
| post×D | coefficient |  | 0.033 | -0.497** | 0.066* | 0.023 |  |  |  |
| post×D | standard_error |  | 0.041 | 0.252 | 0.035 | 0.052 |  |  |  |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y | Y | Y | Y |
| N of clusters (firms) | 2,218 | 2,218 | 1,176 | 1,176 | 1,936 [printed as "1,936 s)" in source] | 1,176 | 1,176 | 1,936 |
| Observations | 46,359 | 46,359 | 16,632 | 16,632 | 40,596 | 16,632 | 16,632 | 40,596 |
| R² | 0.44 | 0.44 | 0.52 | 0.70 | 0.62 | 0.52 | 0.70 | 0.61 |

**Note:** This Table reproduces the main analyses for single-bank firms in Tables 5 and 6 using 5-rated firms as the control group (in place of 5+ rated firms). Columns (1) and (2) focus on Table 5; the remaining columns on Table 6. Columns (4) and (7) scale ST debt by total debt (instead of ST debt) in the pre-period, because many firms have very little pre-period ST debt, pushing measured increases upwards. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level. [Conversion note: the N of clusters cell in column 5 is printed in the source PDF as "1,936 s)", which appears to be a typesetting artifact; the value is transcribed as 1,936 and flagged here.]

### Table A10: Robustness for Table 7 (Single-bank firms). Control group: 5-rated firms

- **Table type:** Regression (triple difference; reproduces Table 7 for single-bank firms using 5-rated control group, and adding micro firms)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10%, + 15% significance level

#### Column metadata

| model | sample | D_definition |
|---:|---|---|
| 1 | ACC vs. 5 | High Leverage |
| 2 | ACC vs. 5 | Low Tangibles |
| 3 | ACC vs. 5 | Young |
| 4 | Adding micro firms | High Leverage |
| 5 | Adding micro firms | Low Tangibles |
| 6 | Adding micro firms | Young |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| ACC×post×D | coefficient | -0.054 | -0.102* | -0.092+ | -0.065* | -0.096*** | -0.089*** |
| ACC×post×D | standard_error | 0.050 | 0.054 | 0.058 | 0.038 | 0.031 | 0.034 |
| ACC×post | coefficient | 0.087* | 0.091*** | 0.082*** | 0.094*** | 0.094*** | 0.083*** |
| ACC×post | standard_error | 0.045 | 0.029 | 0.028 | 0.036 | 0.022 | 0.021 |
| post×D | coefficient | -0.098** | 0.065 | 0.003 | -0.101*** | 0.032 | 0.009 |
| post×D | standard_error | 0.043 | 0.058 | 0.050 | 0.033 | 0.035 | 0.029 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y | Y |
| N of clusters (firms) | 2,218 | 2,218 | 2,218 | 3,556 | 3,556 | 3,556 |
| Observations | 46,359 | 46,359 | 46,359 | 74,938 | 74,938 | 74,938 |
| R² | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 |

**Note:** This Table reproduces the analysis for single-bank firms in Table 7 using 5-rated firms as the control group (in place of 5+ rated firms). Columns (4) - (6) add micro firms to the sample in order to increase statistical power, as an illustrative exercise. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10%, + 15% significance level.

### Table A11: Robustness: conditioning on observables with rating stability (Single-bank firms)

- **Table type:** Regression (triple difference; reproduces Table 7 for single-bank firms with rating-stability requirements)
- **Dependent variable:** firm debt growth as in Table 2
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | rating_stability_requirement | D_definition |
|---:|---|---|
| 1 | 6-month | High leverage |
| 2 | 6-month | Low Tangibles |
| 3 | 6-month | Young |
| 4 | 12-month | High leverage |
| 5 | 12-month | Low Tangibles |
| 6 | 12-month | Young |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| ACC×post×D | coefficient | -0.116*** | -0.088** | -0.082* | -0.126*** | -0.106** | -0.099** |
| ACC×post×D | standard_error | 0.034 | 0.039 | 0.043 | 0.038 | 0.042 | 0.043 |
| ACC×post | coefficient | 0.106*** | 0.104*** | 0.086*** | 0.098*** | 0.100*** | 0.076*** |
| ACC×post | standard_error | 0.028 | 0.025 | 0.023 | 0.033 | 0.030 | 0.027 |
| post×D | coefficient | 0.032 | 0.097** | 0.013 | 0.023 | 0.097** | 0.002 |
| post×D | standard_error | 0.029 | 0.043 | 0.028 | 0.034 | 0.045 | 0.030 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Covariates x post | Y | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y | Y |
| N of clusters (firms) | 2,301 [printed as "2.301" in source] | 2,301 | 2,301 | 1,734 | 1,734 | 1,734 |
| Observations | 48,375 | 48,375 | 48,375 | 36,456 | 36,456 | 36,456 |
| R² | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 | 0.44 |

**Note:** This Table reproduces the analysis of Table 7 for single-bank firms (there was no result for multi-bank firms), adding a requirement that firms maintain stable ratings for 6 or 12 months. The dependent variable is firm debt growth as in Table 2. *High Leverage* is an indicator for firms with average 2011 leverage above the sample median; *Low Tangibles* is an indicator for firms whose ratio of tangible to total assets is in the bottom quartile in 2011; *Young* is an indicator for firm age below 6 years in 2011. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level. [Conversion note: the column-1 N of clusters cell is printed "2.301" in the source (period instead of comma); transcribed as 2,301 and flagged.]

### Table A12: Robustness: Exploring the Spillover effect on subsamples

- **Table type:** Regression (spillover analysis of Table 3 in subsamples)
- **Treatment group:** 5+ rated firms; **control group:** 5 rated firms
- **Dependent variable:** firm debt growth
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level
- All models include: Covariates x Post, Bank-Month FE, Industry-Qtr FE, Firm FE

#### Panel A: Low Leverage / Low Tangible / Young subsamples

##### Column metadata

| model | subsample | bank_status |
|---:|---|---|
| 1 | Low Leverage | Single |
| 2 | Low Leverage | Multi |
| 3 | Low Tangible | Single |
| 4 | Low Tangible | Multi |
| 5 | Young | Single |
| 6 | Young | Multi |

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Rating 5+×post | coefficient | -0.029 | 0.130*** | 0.008 | 0.090*** | -0.014 | 0.106*** |
| Rating 5+×post | standard_error | 0.067 | 0.038 | 0.033 | 0.032 | 0.028 | 0.027 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 345 | 949 | 671 | 1,015 | 968 | 1,160 |
| Observations | 6,916 | 17,105 | 14,318 | 18,673 | 20,695 | 21,874 |
| R² | 0.44 | 0.53 | 0.40 | 0.52 | 0.47 | 0.53 |

#### Panel B: High Leverage / High Tangible / Old subsamples

##### Column metadata

| model | subsample | bank_status |
|---:|---|---|
| 1 | High Leverage | Single |
| 2 | High Leverage | Multi |
| 3 | High Tangible | Single |
| 4 | High Tangible | Multi |
| 5 | Old | Single |
| 6 | Old | Multi |

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Rating 5+×post | coefficient | 0.017 | 0.062*** | -0.020 | 0.073*** | -0.011 | 0.065** |
| Rating 5+×post | standard_error | 0.024 | 0.024 | 0.032 | 0.025 | 0.043 | 0.029 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 799 | 1,120 | 774 | 1,305 | 482 | 1,158 |
| Observations | 17,222 | 21,534 | 16,349 | 25,100 | 10,047 | 21,982 |
| R² | 0.48 | 0.55 | 0.49 | 0.54 | 0.42 | 0.53 |

**Note:** This Table uses 5+ rated firms as the treatment group and 5 rated firms as the control group. The dependent variable is firm debt growth. High/Low Leverage, Tangibility, and age are defined as in Table 7. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A13: Robustness: Exploring the Lending Relationship effect on subsamples. Leverage & Tangibles

- **Table type:** Regression (triple difference; reproduces columns 2 and 4 of Table 5 in subsamples based on firms' leverage and asset tangibility, defined as in Table 7)
- **D:** indicator for above-median relationship depth, as in Table 5
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level
- All models include: Covariates x Post, Bank-Month FE, Industry-Qtr FE, Firm FE

#### Panel A: Low Leverage and Low Tangible subsamples

##### Column metadata

| model | subsample | bank_status | comparison |
|---:|---|---|---|
| 1 | Low Leverage | Single Bank | ACC vs 5+ |
| 2 | Low Leverage | Single Bank | ACC vs 5 |
| 3 | Low Leverage | Multi-bank | ACC vs 5+ |
| 4 | Low Leverage | Multi-bank | ACC vs 5 |
| 5 | Low Tangible | Single Bank | ACC vs 5+ |
| 6 | Low Tangible | Single Bank | ACC vs 5 |
| 7 | Low Tangible | Multi-bank | ACC vs 5+ |
| 8 | Low Tangible | Multi-bank | ACC vs 5 |

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| ACC×post×D | coefficient | 0.036 | 0.172 | 0.005 | -0.005 | 0.198*** | 0.286*** | -0.065 | -0.030 |
| ACC×post×D | standard_error | 0.090 | 0.147 | 0.063 | 0.067 | 0.050 | 0.079 | 0.050 | 0.059 |
| ACC×post | coefficient | 0.059 | -0.043 | 0.029 | 0.143*** | -0.044** | -0.085* | 0.075** | 0.126*** |
| ACC×post | standard_error | 0.074 | 0.131 | 0.051 | 0.050 | 0.022 | 0.048 | 0.037 | 0.042 |
| post×D | coefficient | 0.068 | -0.077 | -0.017 | -0.010 | -0.025 | -0.127* | 0.071* | 0.027 |
| post×D | standard_error | 0.074 | 0.138 | 0.053 | 0.056 | 0.042 | 0.074 | 0.042 | 0.050 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 945 | 856 | 2,082 | 1,675 | 1,319 | 960 | 2,233 | 1,762 |
| Observations | 18,718 | 16,913 | 38,732 | 31,433 | 27,297 | 19,494 | 41,901 | 32,883 |
| R² | 0.41 | 0.41 | 0.48 | 0.48 | 0.43 | 0.43 | 0.47 | 0.47 |

#### Panel B: High Leverage and High Tangible subsamples

##### Column metadata

| model | subsample | bank_status | comparison |
|---:|---|---|---|
| 1 | High Leverage | Single Bank | ACC vs 5+ |
| 2 | High Leverage | Single Bank | ACC vs 5 |
| 3 | High Leverage | Multi-bank | ACC vs 5+ |
| 4 | High Leverage | Multi-bank | ACC vs 5 |
| 5 | High Tangible | Single Bank | ACC vs 5+ |
| 6 | High Tangible | Single Bank | ACC vs 5 |
| 7 | High Tangible | Multi-bank | ACC vs 5+ |
| 8 | High Tangible | Multi-bank | ACC vs 5 |

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| ACC×post×D | coefficient | 0.117*** | 0.115** | 0.023 | 0.061 | 0.050 | 0.049 | 0.070 | 0.072 |
| ACC×post×D | standard_error | 0.041 | 0.046 | 0.037 | 0.049 | 0.050 | 0.061 | 0.043 | 0.050 |
| ACC×post | coefficient | -0.010 | 0.004 | 0.011 | 0.035 | 0.079*** | 0.070 | -0.004 | 0.074** |
| ACC×post | standard_error | 0.020 | 0.025 | 0.024 | 0.026 | 0.031 | 0.043 | 0.032 | 0.031 |
| post×D | coefficient | 0.022 | 0.021 | 0.059* | 0.017 | 0.109*** | 0.113** | 0.010 | 0.011 |
| post×D | standard_error | 0.031 | 0.034 | 0.030 | 0.046 | 0.036 | 0.048 | 0.036 | 0.044 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 1,455 | 1,070 | 2,120 | 1,615 | 1,481 | 1,257 | 2,408 | 1,896 |
| Observations | 31,464 | 23,124 | 42,044 | 31,810 | 31,372 | 26,618 | 47,506 | 37,391 |
| R² | 0.50 | 0.52 | 0.54 | 0.54 | 0.46 | 0.45 | 0.52 | 0.51 |

**Note:** This Table reproduces columns 2 and 4 of Table 5 in sub-samples based on firms' leverage and asset tangibility, defined as in Table 7. D is an indicator for above-median relationship depth, as in Table 5. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A14: Robustness: Exploring the Lending Relationship effect on subsamples. Firm Age

- **Table type:** Regression (triple difference; reproduces columns 2 and 4 of Table 5 in subsamples based on firms' age, defined as in Table 7)
- **D:** indicator for above-median relationship depth, as in Table 5
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level
- All models include: Covariates x Post, Bank-Month FE, Industry-Qtr FE, Firm FE

#### Column metadata

| model | subsample | bank_status | comparison |
|---:|---|---|---|
| 1 | Young | Single Bank | ACC vs 5+ |
| 2 | Young | Single Bank | ACC vs 5 |
| 3 | Young | Multi-bank | ACC vs 5+ |
| 4 | Young | Multi-bank | ACC vs 5 |
| 5 | Old | Single Bank | ACC vs 5+ |
| 6 | Old | Single Bank | ACC vs 5 |
| 7 | Old | Multi-bank | ACC vs 5+ |
| 8 | Old | Multi-bank | ACC vs 5 |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| ACC×post×D | coefficient | 0.075 | 0.047 | -0.013 | 0.067 | 0.162*** | 0.249*** | 0.021 | 0.024 |
| ACC×post×D | standard_error | 0.047 | 0.060 | 0.049 | 0.051 | 0.061 | 0.088 | 0.046 | 0.052 |
| ACC×post | coefficient | 0.020 | 0.024 | 0.062* | 0.105*** | 0.015 | -0.059 | 0.018 | 0.064* |
| ACC×post | standard_error | 0.020 | 0.034 | 0.033 | 0.035 | 0.043 | 0.074 | 0.036 | 0.036 |
| post×D | coefficient | 0.072** | 0.083* | 0.076* | -0.014 | 0.031 | -0.060 | 0.003 | 0.005 |
| post×D | standard_error | 0.035 | 0.049 | 0.041 | 0.041 | 0.047 | 0.078 | 0.039 | 0.046 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 1,610 | 1,187 | 2,156 | 1,622 | 1,188 | 1,025 | 2,481 | 2,048 |
| Observations | 34,110 | 24,942 | 41,192 | 30,853 | 24,522 | 21,075 | 48,403 | 39,737 |
| R² | 0.44 | 0.44 | 0.49 | 0.49 | 0.45 | 0.44 | 0.49 | 0.49 |

**Note:** This Table reproduces columns 2 and 4 of Table 5 in sub-samples based on firms' age, defined as in Table 7. D is an indicator for above-median relationship depth, as in Table 5. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A15: Table 5 for higher rated firms

- **Table type:** Regression (triple difference; reproduces Table 5 with always-eligible treated group)
- **Treated group:** always-eligible, higher-rated firms (3++, 3+, 3 and 4+ rated firms)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | sample | D_definition |
|---:|---|---|
| 1 | Single-bank (All Eligible vs. 5+) | D=1 if LR>median |
| 2 | Single-bank (All Eligible vs. 5+) | D=1 if HHI<median |
| 3 | Multibank (All Eligible vs. 5) | D=1 if LR>median |
| 4 | Multibank (All Eligible vs. 5) | D=1 if HHI<median |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 |
|---|---|---:|---:|---:|---:|
| Eligible×post×D | coefficient | 0.104*** | 0.078** | 0.015 | -0.001 |
| Eligible×post×D | standard_error | 0.037 | 0.034 | 0.043 | 0.031 |
| Eligible×post | coefficient | 0.039 | 0.078*** | 0.087** | 0.098*** |
| Eligible×post | standard_error | 0.033 | 0.021 | 0.041 | 0.027 |
| post×D | coefficient | -0.023 | 0.054** | -0.005 | 0.062** |
| post×D | standard_error | 0.024 | 0.026 | 0.036 | 0.028 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 |
|---|---:|---:|---:|---:|
| Covariates x post Dec | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y |
| N of clusters (firms) | 3,838 | 3,838 | 4,232 | 4,232 |
| Observations | 87,061 | 87,061 | 92,131 | 92,131 |
| R² | 0.47 | 0.47 | 0.51 | 0.51 |

**Note:** This Table reproduces Table 5 but with a treated group composed of always-eligible, higher-rated firms (3++, 3+, 3 and 4+ rated firms). The control group is 5+ for single-bank firms and 5 for multi-bank firms. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A16: Table 6 for higher rated firms

- **Table type:** Regression (triple difference; reproduces Table 6 with always-eligible treated group)
- **Treated group:** always-eligible, higher-rated firms (3++, 3+, 3 and 4+ rated firms)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level
- All models include: Covariates x post, Bank-Month FE, Industry-Qtr FE, Firm FE

#### Column metadata

| model | sample | dependent_variable | includes_D_interaction |
|---:|---|---|---|
| 1 | Single-bank (All Eligible vs. 5+) | g(ST) | No |
| 2 | Single-bank (All Eligible vs. 5+) | g(MLT) | No |
| 3 | Single-bank (All Eligible vs. 5+) | g(ST) | Yes (D=1 if HHI<median) |
| 4 | Single-bank (All Eligible vs. 5+) | g(MLT) | Yes (D=1 if HHI<median) |
| 5 | Multi-bank (All Eligible vs. 5) | g(ST) | No |
| 6 | Multi-bank (All Eligible vs. 5) | g(MLT) | No |
| 7 | Multi-bank (All Eligible vs. 5) | g(ST) | Yes (D=1 if HHI<median) |
| 8 | Multi-bank (All Eligible vs. 5) | g(MLT) | Yes (D=1 if HHI<median) |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Eligible×post×D | coefficient |  |  | 0.448 | 0.078** |  |  | 0.070 | 0.109 |
| Eligible×post×D | standard_error |  |  | 0.312 | 0.039 |  |  | 0.219 | 0.070 |
| Eligible×post | coefficient | 0.072 | 0.133*** | -0.230 | 0.092*** | 0.440*** | 0.020 | 0.412** | -0.039 |
| Eligible×post | standard_error | 0.134 | 0.022 | 0.291 | 0.022 | 0.117 | 0.037 | 0.199 | 0.054 |
| post×D | coefficient |  |  | -0.680*** | 0.045 |  |  | -0.295 | -0.025 |
| post×D | standard_error |  |  | 0.254 | 0.031 |  |  | 0.187 | 0.067 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 | model_8 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| N of clusters (firms) | 1,532 | 3,524 | 1,532 | 3,524 | 2,538 | 3,847 | 2,538 | 3,847 |
| Observations | 21,349 | 81,210 | 21,349 | 81,210 | 38,954 | 82,933 | 38,954 | 82,933 |
| R² | 0.45 | 0.57 | 0.45 | 0.58 | 0.49 | 0.62 | 0.49 | 0.62 |

**Note:** This Table reproduces Table 6 but with a treated group composed of always-eligible, higher-rated firms (3++, 3+, 3 and 4+ rated firms). The control group is 5+ for single-bank firms and 5 for multi-bank firms. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

### Table A17: Table 7 for higher rated firms

- **Table type:** Regression (triple difference; reproduces Table 7 with always-eligible treated group)
- **Treated group:** always-eligible, higher-rated firms (3++, 3+, 3 and 4+ rated firms)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level

#### Column metadata

| model | D_definition | sample |
|---:|---|---|
| 1 | High Leverage | Single |
| 2 | High Leverage | Multi |
| 3 | Low Tangibles | Single |
| 4 | Low Tangibles | Multi |
| 5 | Young | Single |
| 6 | Young | Multi |

#### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---|---:|---:|---:|---:|---:|---:|
| Eligible×post×D | coefficient | -0.135*** | -0.079** | -0.060* | 0.051 | -0.163*** | -0.010 |
| Eligible×post×D | standard_error | 0.034 | 0.033 | 0.036 | 0.050 | 0.058 | 0.083 |
| Eligible×post | coefficient | 0.161*** | 0.124*** | 0.132*** | 0.090*** | 0.123*** | 0.093*** |
| Eligible×post | standard_error | 0.023 | 0.025 | 0.021 | 0.023 | 0.021 | 0.022 |
| post×D | coefficient | 0.001 | -0.051* | -0.006 | -0.035 | -0.006 | -0.089** |
| post×D | standard_error | 0.025 | 0.029 | 0.030 | 0.046 | 0.026 | 0.043 |

#### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 |
|---|---:|---:|---:|---:|---:|---:|
| Covariates x post Dec | Y | Y | Y | Y | Y | Y |
| Bank-Month FE | Y | Y | Y | Y | Y | Y |
| Industry-Qtr FE | Y | Y | Y | Y | Y | Y |
| Firm FE | Y | Y | Y | Y | Y | Y |
| N of clusters (firms) | 3,838 | 4,232 | 3,838 | 4,232 | 3,838 | 4,232 |
| Observations | 87,061 | 92,131 | 87,061 | 92,131 | 87,061 | 92,131 |
| R² | 0.47 | 0.52 | 0.47 | 0.51 | 0.47 | 0.51 |

**Note:** This Table reproduces Table 7 but with a treated group composed of always-eligible, higher-rated firms (3++, 3+, 3 and 4+ rated firms). The control group is 5+ for single-bank firms and 5 for multi-bank firms. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level. [Conversion note: the source prints the "Covariates x post Dec" row label without Y/N entries visible across columns in the PDF bottom panel layout; the row is reproduced as printed in the original (label row present), with the FE rows below marked Y as printed.]

### Table A18: Bank heterogeneity

- **Table type:** Regression (triple difference, equation 4)
- **Dependent variable:** percentage change in a firm's total bank debt
- **Sample:** all SMEs in eligible credit ratings except for the ACC group (i.e., 4+ to 3++), and the control groups (5+ for single-bank, 5 for multi-bank)
- **Covariates:** firm characteristics (size, tangibility, profitability) as of 2010, interacted with Post (defined as beginning in Dec. 2011 instead of Feb. 2012)
- **Standard errors:** clustered by firm, in parentheses
- **Significance:** *** 1%, ** 5%, * 10% significance level
- All models include: Covariates × post, Bank-Time FE, Industry-Qtr FE, Firm FE

#### Panel: Single-Bank (All Eligible vs 5+)

##### Column metadata

| model | interaction_variable |
|---:|---|
| 1 | Funding Cost |
| 2 | Core Tier 1 |
| 3 | Drop in Stock Price |
| 4 | Eligible Share |
| 5 | Free Collateral |
| 6 | Quantitative Easing |
| 7 | Maturity Swap |

##### Estimates

| variable | statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| Eligible ×post | coefficient | 0.111*** | 0.115*** | 0.120*** | 0.109*** | 0.114*** | 0.113*** | 0.116*** |
| Eligible ×post | standard_error | 0.024 | 0.021 | 0.022 | 0.023 | 0.021 | 0.021 | 0.022 |
| (All Eligible)×post×Interaction | coefficient | 0.023 | -0.014 | 0.002 | -0.025 | -0.013 | 0.010 | 0.005 |
| (All Eligible)×post×Interaction | standard_error | 0.026 | 0.018 | 0.032 | 0.029 | 0.018 | 0.015 | 0.023 |

##### Model statistics

| statistic | model_1 | model_2 | model_3 | model_4 | model_5 | model_6 | model_7 |
|---|---:|---:|---:|---:|---:|---:|---:|
| N clusters (firm) | 3,015 | 3,747 | 3,015 | 3,747 | 3,747 | 3,747 | 3,747 |
| N clusters (bank-month) | 444 | 524 | 444 | 524 | 524 | 524 | 524 |
| Observations | 68,918 | 85,020 | 68,918 | 85,020 | 85,020 | 85,020 | 85,020 |
| R² | 0.47 | 0.47 | 0.47 | 0.47 | 0.47 | 0.47 | 0.47 |

#### Panel: Multibank (All Eligible vs 5)

##### Column metadata

| model | interaction_variable |
|---:|---|
| 8 | Funding Cost |
| 9 | Core Tier 1 |
| 10 | Drop in stock price |
| 11 | Eligible share |
| 12 | Free Collateral |
| 13 | Quantitative Easing |
| 14 | Maturity Swap |

##### Estimates

| variable | statistic | model_8 | model_9 | model_10 | model_11 | model_12 | model_13 | model_14 |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| Eligible ×post | coefficient | 0.084*** | 0.110*** | 0.091*** | 0.103*** | 0.105*** | 0.107*** | 0.093*** |
| Eligible ×post | standard_error | 0.023 | 0.021 | 0.023 | 0.021 | 0.021 | 0.021 | 0.021 |
| (All Eligible)×post×Interaction | coefficient | 0.028 | 0.013 | -0.003 | -0.011 | -0.005 | -0.001 | 0.029* |
| (All Eligible)×post×Interaction | standard_error | 0.018 | 0.012 | 0.022 | 0.018 | 0.013 | 0.011 | 0.015 |

##### Model statistics

| statistic | model_8 | model_9 | model_10 | model_11 | model_12 | model_13 | model_14 |
|---|---:|---:|---:|---:|---:|---:|---:|
| N clusters (firm) | 3,226 | 3,991 | 3,226 | 3,991 | 3,991 | 3,991 | 3,991 |
| N clusters (bank-month) | 4,249 | 5,046 | 4,249 | 5,046 | 5,046 | 5,046 | 5,046 |
| Observations | 70,363 | 87,186 | 70,363 | 87,186 | 87,186 | 87,186 | 87,186 |
| R² | 0.53 | 0.52 | 0.53 | 0.52 | 0.52 | 0.52 | 0.52 |

**Note:** This is a triple difference estimation as in equation (4), with percentage change in a firm's total bank debt as the dependent variable. The interaction terms are named above each column. The first three are proxies for balance sheet robustness of the firm's (main) bank; specifically, funding costs (cols 1 and 8), Core Tier 1 ratio (cols 2 and 9), and drop in stock prices in the pre-period (cols 3 and 10). The next two interactions identify firms whose (main) bank has differential ability to take advantage of the VLTRO funding: share of eligible loans in their December 2011 lending portfolio (cols 4 and 11), and unused collateral (cols 5 and 12). Finally, the last two interactions are proxies for the (main) bank use of the 3-year maturity funding as described by Andrade et al. (2018): the increase in total borrowed liquidity at the time of the VLTRO - i.e., a pure quantitative easing effect (cols 6 and 13), and a measure of the amount of shorter-term central bank liquidity that has been swapped by the (main) bank for the 3-year borrowing (cols 7 and 14). All bank variables are standardized and expressed as a standard score. The sample consists of all SMEs in eligible credit ratings except for the ACC group (i.e., 4+ to 3++), and the control groups (5+ for single-bank, 5 for multi-bank). This matches the sample in Table 10. Covariates are firm characteristics (size, tangibility, profitability) as of 2010, interacted with Post (defined as beginning in Dec. 2011 instead of Feb. 2012). Data sources and details for this table are in the Appendix. Standard errors in parentheses are clustered by firm; *** 1%, ** 5%, * 10% significance level.

## Appendix 1: Motivating evidence from the TLTROs

In this section we provide motivating evidence for the claim that single-bank firms receive differential transmission of collateral-based UMP. To do so we examine the ECB's Targeted Long-Term Refinancing Operations, which were announced in June 2014 (TLTRO I), March 2016 (TLTRO II) and March 2019 (TLTRO III). These schemes allowed banks to borrow from the ECB at favorable rates, and at relatively long maturities for this type of borrowing (two to four years). Importantly, the amount banks were allowed to borrow depended on banks' record of lending to firms.

Figure A1 plots the monthly change in bank debt (relative to the year before the announcement) for single and multi-bank firms separately for each TLTRO. Both the announcements and the implementations appear to generate relatively little change in lending to both groups, suggesting that these policies may have been anticipated, at least partially, by banks and firms, consistent with press reports (e.g., Financial Times, 2013a; Reuters, 2018).[^A1]

[^A1]: Original footnote number 1 in the appendix. Banks also had an incentive to increase lending before policy was announced if they anticipated that the TLTRO I structure (which had the total subsidy increasing with the size of a bank's firm lending portfolio) was likely to be maintained in subsequent iterations.

However, 2014-2020 was a period of extraordinary unconventional policy activism during which the ECB also introduced forward guidance, negative rates, and asset purchase programs, making it difficult to isolate the impact of a specific policy. We include additional vertical lines for major ECB announcements occurring in the pre-announcement periods. For example, in September 2013 ECB President Draghi told the European Parliament that the ECB stood ready to launch "another LTRO" (Financial Times, 2013b), which appears to lead to an immediate and sustained increase in lending to multi-bank firms, but not to single-bank firms. Similarly, in June 2015 the European Court of Justice ruled the OMT asset purchase program was legal and in June 2018 the ECB announced the end of quantitative easing, together with dovish forward guidance (Financial Times, 2015 and Financial Times, 2018). In both of these cases the graphs show lending to multi-bank borrowers rising relative to single-bank firms.

The most marked divergence between single and multi-bank firms in these graphs occurs for the Pandemic Emergency LTRO (PELTRO) which was announced April 2020. While the announcement triggered sharp increases in lending to firms, this increase was markedly larger for multi-bank firms. Furthermore, in August 2019 the ECB announced the extension of the maturity of TLTRO III loans from two to three years, triggering a large and sustained increase in lending to multi-bank firms, but no appreciable change for single-bank firms, despite closely parallel pre-trends.

The four panels of Figure A1 present a consistent picture: across eight years and four ECB liquidity policies, bank lending to multi-bank firms increases earlier and by substantially more than lending to single-bank firms. While this evidence is from time-series averages only, it is suggestive of a systematic difference in liquidity transmission between single and multi-bank firms. To make causal claims, and to avoid potential policy anticipation by banks and the effects of other policies confounding our analysis, we move to examine the first iteration of these long-maturity liquidity policies at scale, the Very Long-Term Refinancing Operations (VLTROs) of 2011-2012.

## Appendix 2: Estimating the effect of the VLTRO policy on bank funding costs

Credit claims made up 36% of the €413 billion of collateral pledged with the Banque de France by 54 banks at the end of 2011. In France, the ACC made available an additional pool of corporate credit claim collateral of about €90 billion after haircuts, which according to Bignon et al. (2016) corresponds to a collateral shock for French banks of between 4.8% and 15.1% of their drawn loans.[^A2]

[^A2]: Original footnote number 2 in the appendix. In practice, the use of the ACC-rated loans in France as pledged Eurosystem collateral totaled €9 billion, while for firms rated above ACC it stood at €126 billion as of June 2012, with both totals being after haircuts. Haircuts on eligible credit claims range from 17% to 70% depending on loan maturity and rating, making the total value of the underlying loans correspondingly larger.

An estimate for the size of the fall in the marginal cost of funding for French banks at the time the VLTRO program was announced is the difference between the cost of market debt for these banks, and the ECB main refinancing rate at which they could obtain financing using the newly-eligible collateral. The bottom panel of Figure A2 displays the cost of market debt from Gilchrist and Mojon (2017) and the ECB's main refinancing operation (MRO) rate, which is the rate paid by banks borrowing in the VLTROs. Bank marginal funding costs rose throughout 2011, but this rise intensified in the second semester. The cost of market funding reached about 5.2% on average in the last quarter of 2011, whereas the main refinancing rate was 1% at the end of the year, making the spread over 400 basis points.[^A3]

[^A3]: Original footnote number 3 in the appendix. This is an approximation, because the maturity of borrowing from the Eurosystem could be lower than that of the Gilchrist and Mojon (2017) data, which is a weighted average of different bond maturities. Further, market rates reflect rates for partly unsecured lending, while the ECB refinancing rate is fully secured. Finally, the banks in the market data are likely riskier than the average bank, as they were constrained enough to issue expensive market debt.

However, over the course of 2012 the spread between the cost of market debt and the MRO rate fell in response to the massive injections of liquidity by the ECB via the VLTROs; by the end of 2012 the advantage of the VLTRO in terms of below-market-cost funding had largely disappeared.

## Appendix 3: Description of Additional Data Used

### Firm accounting data

Accounting data mainly consists of firm balance sheets from the BdF's FIBEN database, which is compiled from tax returns. It includes all French firms with sales of €750,000 or greater.[^A4] We drop firms with negative debt, negative or zero total assets, or missing number of employees. All firm characteristics are winsorized at the 0.5 and 99.5 percentile.

[^A4]: Original footnote number 4 in the appendix. In 2004, FIBEN covered 80% of the firms with 20 to 500 employees, and 98% of those employing more than 500 employees.

### Firm-bank credit registry data

Monthly firm-bank debt data comes from the French national Central Credit Register (CCR), which captures the total exposure (i.e. the sum of all credit of any kind) of a credit institution to a firm that exceeds €25,000.[^A5] Because we drop micro-firms and so only have firms with sales exceeding €2 million we do not view this truncation of the left tail as a consequential data constraint.

[^A5]: Original footnote number 5 in the appendix. The reporting threshold on credit data applied at the branch level until April 2012, and at the bank level afterwards. Following Andrade et al. (2018), we drop all branch-firm links with a total exposure below €25,000 and then collapse this database to the bank-firm level.

We aggregate credit exposures at the level of banking groups (henceforth referred to as a "banks"), and identify the main lender of each firm as the bank with the largest average share of drawn credit in 2011. We also require banking groups to be present in the sample each month, limiting attrition due to bankruptcy, restructuring or mergers.[^A6] Finally, an implicit requirement of a valid difference in differences strategy is that firms must be present before and after the VLTRO policy. Thus, our main sample spans a two year period centered on the announcement date (i.e., between March 2011 and February 2013) and we require firms to maintain a bank relationship throughout.

[^A6]: Original footnote number 6 in the appendix. Dexia bank entered a resolution process in October 2011, after reporting large losses. To avoid potential effects on our estimates resulting from the disappearance of a bank, we drop all firms that had credit from Dexia or from banking entities in its group at any point in the period January 2010-December 2014.

## Appendix 4: Variables used in Table A18: Bank heterogeneity

The set of bank groups consists of 3 mutual banks (Credit Mutuel (CM), Credit Agricole (CASA), BPCE), and 3 commercial banks (Societe Generale (SG), BNP-Paribas (BNPP), HSBC). These bank groups capture over 97% of observations in our final sample, and over 90% of total drawn credit in the French Credit Registry as of December 2011.

- **Funding Cost:** Bank funding cost expressed in basis points as of December 2010. Source: Results of the 2011 European Bank Assessment EU-wide stress tests. Missing information for Credit Mutuel.
- **Core Tier 1 capital:** the ratio of a bank's core tier 1 capital (equity plus reserves) to total risk-weighted assets. Source: Bank groups' Financial Reports.
- **Stock price.** Source: Bloomberg. Missing information for Credit Mutuel (unlisted).
- **Eligible Share in Loan Portfolio:** for each bank, this is the ratio of drawn credit to eligible firms (ratings 4/ACC and higher) over drawn credit to all non-financial corporations (SMEs, intermediate, and large firms, excluding real estate companies). The source is the French Credit Register, hence this variable does not take into account loans abroad.
- **Free Collateral:** This is computed as 1-RO/Collateral, where RO is each bank's ECB liquidity as of Dec. 2011 (computed as the sum of all the bank's outstanding refinancing operations with the ECB, i.e. MRO, LTRO1M, LTRO3M, LTRO6M, LTRO1Y, VLTRO-3Y) and Collateral is the total posted collateral, valued after haircut. Source: Banque de France Market Operation data.
- **Quantitative Easing:** the increase in total borrowed liquidity between September 2011 and December 2011 (i.e., at the time of the first 3-year VLTRO), normalized by the total assets of the bank.
- **Maturity Swap:** the amount of shorter-term central bank liquidity that has been swapped by a bank for 3-year borrowing from the ECB, divided by the bank's total assets. The amount swapped is equal to zero if the bank did not tap the facility; otherwise it is the maximum of zero and the total borrowed liquidity in December 2011 minus the pure quantitative easing effect described in preceding point (see Andrade et al., 2018).
