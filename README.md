# Clustering Stocks Based on Financial Efficiency

## Overview

This project applies unsupervised machine learning, specifically K-Means clustering, to identify groups of companies with similar levels of financial efficiency. Using key profitability metrics such as Return on Equity (ROE), Return on Assets (ROA), and Return on Investment (ROI), with the dataset of over 5,000 publicly traded companies. The goal is to uncover underlying patterns that help investors or analysts find financially efficient companies, regardless of sector or stock price.

## Objectives

* Group companies based on financial efficiency metrics.
* Identify clusters of firms that are similar in profitability and capital utilization.
* Provide a data-driven foundation for financial screening, benchmarking, or long-term investment decisions.

## Why K-Means Clustering?

K-Means is chosen for its simplicity and speed, especially in dealing with a relatively small number of key financial features. It is effective for uncovering natural groupings when the goal is to identify relative similarity, not prediction.

## Dataset
Data of publicly traded company with 46 features such as bookvalue per share, dividend yield, PE ratio, etc.
* Source: TD Ameritrade (2019)
* Total records: \~5,200 companies
* Features used for clustering:

  * `returnOnEquity`
  * `returnOnAssets`
  * `returnOnInvestment`

## Libraries

* NumPy
* Pandas
* Scikit-learn 
* Matplotlib
* Yellowbrick

## Limitations

While this K-Means model clusters stocks using ROE, ROA, and ROI, it does not account for industry context. As a result, some clusters may group together companies with fundamentally different business models and risk profiles.

However, this model provides a useful first-pass tool for identifying broad financial patterns. It can be refined in the future by:

Incorporating industry segmentation

Including additional financial or market features

Applying domain-specific clustering strategies

Ultimately, this demonstrates how unsupervised learning can uncover hidden structure in financial data — but also the importance of domain knowledge in interpreting the results.

## Use case

Screening Undervalued Stocks in Emerging Markets An investment firm wants to identify financially strong but under-the-radar companies in emerging markets, where data is often incomplete and industry classifications are inconsistent.

They can apply this K-Means clustering model, trained on ROE, ROA, and ROI, across all listed companies in the region—regardless of sector. The goal is to group companies by financial efficiency, not by industry.

One cluster reveals a group of high-ROE, high-ROI firms with low analyst coverage and low market cap. These companies—mostly small manufacturers and logistics firms—are not obvious picks in traditional screens.

Analysts can investigate further and find several promising investment opportunities. These companies are added to a specialized fund focused on emerging market value plays.

Key Value: Helps uncover hidden, high-performing companies that don’t surface in standard filters

Bypasses noisy or unreliable industry classifications

## Conclusion

This project demonstrates how simple unsupervised learning techniques can be leveraged to gain financial insights from large-scale stock data. With minimal features and preprocessing, it's possible to extract meaningful groups of companies that share similar financial efficiency characteristics, providing a valuable lens for investors and analysts alike.
