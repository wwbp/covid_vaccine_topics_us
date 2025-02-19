# Twitter discourse reveals geographical and temporal variation in concerns about COVID-19 Vaccines in the United States.

A set of 100 COVID-19 vaccine-related topics derived from Twitter between December 2020 and February 2021. 

Read the full publication [here](https://doi.org/10.1016/j.vaccine.2021.06.014). 

We also release the tweet_ids of vaccine related tweets from December 2020 to November 2021 (a subset of which was used in this paper) [here](https://drive.google.com/file/d/1SxzVkEvy24gxQl-SV_G9yGpB2spqvgPJ/view?usp=sharing). You could use several tools such as [hydrator](https://github.com/DocNow/hydrator) to download the tweet objects. 

## Topics

There are two files in this data:

### covidVax100US_cp
This file is used to extract topic prevalence.

* `id`: auto-incremented numeric row id
* `term`: unigram in topic
* `category`: Numeric topic id (from 0 to 99)
* `weight`: Conditional probability of the topic given the unigram, as derived through the LDA process. 

### covidVax100US_freq_t50ll
This file is used to visualize top words in each topic.

* `id`: auto-incremented numeric row id 
* `term`: unigram in topic
* `category`: Numeric topic id (from 0 to 100)
* `weight`: Posterior likelihood

The third file `acp_vaccination_rates_week.csv` indicates Percentage of people who received two doses of the COVID-19 vaccine in each ACP community as designated by the [American Communities Project](https://www.americancommunities.org/). Vaccination data was obtained from [CDC](https://www.cdc.gov/coronavirus/2019-ncov/vaccines/distributing/reporting-counties.html) between December 13, 2020 and June 3, 2021 for counties and aggregated to weeks across ACP communities.

## Tweet IDs
`tweetIDs_FIPS.csv.zip`: Vaccine related tweets and the corresponding County FIPS codes. We are unable to share the raw tweets in alignment with Twitter TOS. 


## Citation

Please cite the following paper if you use this data. 

Sharath Chandra Guntuku, Alison M. Buttenheim, Garrick Sherman, Raina M. Merchant, Twitter discourse reveals geographical and temporal variation in concerns about COVID-19 Vaccines in the United States, Vaccine, 2021,

```
@article{guntuku2021twittervaccine,
title = {Twitter discourse reveals geographical and temporal variation in concerns about COVID-19 Vaccines in the United States},
journal = {Vaccine},
year = {2021},
issn = {0264-410X},
doi = {https://doi.org/10.1016/j.vaccine.2021.06.014},
url = {https://www.sciencedirect.com/science/article/pii/S0264410X21007386},
author = {Sharath Chandra Guntuku and Alison M. Buttenheim and Garrick Sherman and Raina M. Merchant}
}
```

## Contact

Please contact sharathg [at] cis [dot] upenn [dot] edu or garricks [at] sas [dot] upenn [dot] edu with any questions.

## License

Licensed under a GNU General Public License v3 (GPLv3).
