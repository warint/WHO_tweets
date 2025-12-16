# Dataset on Public Engagement with the World Health Organization on X (Twitter) from 2008 to 2021

This repository contains the dataset described in the *Data in Brief* article: “Dataset on Public Engagement with the World Health Organization on X (Twitter) from 2008 to 2021”. The dataset enables a longitudinal analysis of the WHO's public communications and audience engagement.

## Dataset Overview

* **Subject:** Social Sciences (Social media metrics, Data Science, Public Health Communication).
* **Time Period:** April 23, 2008 – November 8, 2021 (Pre- and Post-COVID-19).
* **Total Records:** 46,667 unique posts.
* **Data Format:** .csv (standard) and .qs (serialized R format).
* **DOI:** 10.5281/zenodo.17457000.

## Repository Structure

The data is available in two formats to ensure broad utility and ease of use:

* `tweets_who_2008_2021.csv`: Standard CSV file for universal compatibility across analytical platforms (Python, Excel, etc.).
* `tweets_who_2008_2021.qs`: Lightweight QS file optimized for rapid processing in R.

## Data Dictionary

Each row in the dataset represents a unique tweet. The variables included are:

| Attribute | Description |
| :--- | :--- |
| **id** | Unique identifier for a tweet post (Tweet ID). |
| **conversation_id** | Unique identifier for the conversation thread to which the tweet belongs. |
| **replies_count** | Number of replies received by the tweet. |
| **retweets_count** | Number of times the tweet was retweeted. |
| **likes_count** | Number of likes received by the tweet. |
| **date** | Date of the tweet in YYYY-MM-DD format. |
| **retweets_reply_ratio** | Retweet-to-reply ratio (Calculated metric for engagement polarity). |
| **likes_reply_ratio** | Like-to-reply ratio (Calculated metric for engagement polarity). |

## Methodology & Usage Notes

### Data Collection
The data was collected using the X (Twitter) Application Programming Interface (API) using R and Python software.

### Privacy and “Dehydration”
In compliance with X's Developer Policy and content redistribution guidelines (https://developer.x.com/en/developer-terms/policy), this dataset has been **dehydrated**.
* Personal metadata (usernames, profile images) and raw text content have been removed to protect user privacy.
* **Rehydration:** Researchers can restore the full set of fields (including the text of the tweets) by "hydrating" the provided Tweet IDs using the X API.

### Ratiometrics
The dataset includes two novel metrics: `retweets_reply_ratio` and `likes_reply_ratio`. These are used to distinguish between public support (high retweets/likes relative to replies) and public controversy (high replies relative to retweets).

## Related Publications

If you use this dataset in your research, please cite the following articles:

1.  **Data Article (Data in Brief):**
    > Melchior, C., De Marcellis-Warin, N., & Warin, T. (2025). *Dataset on Public Engagement with the World Health Organization on X (Twitter) from 2008 to 2021*. Data in Brief.

2.  **Research Article (JMIR):**
    > De Marcellis-Warin, N., Melchior, C., & Warin, T. (2025). *Social Media Metrics as Proxies for Popular Legitimacy: Analyzing Pre- and Post-COVID-19 Public Engagement with the World Health Organization on X*. Journal of Medical Internet Research.

## Authors and Affiliations

* **Cristiane Melchior** - LUT University, Finland
* **Nathalie De Marcellis-Warin** - Polytechnique Montréal, Canada
* **Thierry Warin** - HEC Montréal, Canada