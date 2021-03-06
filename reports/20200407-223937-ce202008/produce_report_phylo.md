---
title: "Phylodynamic Analysis"
urlcolor: blue
linkcolor: blue
output:
  word_document:
    fig_width: 7
    fig_height: 5
    fig_caption: true
    highlight: "tango"
    reference_docx: word_style.docx
    df_print: "kable"
  html_document:
    fig_width: 7
    fig_height: 5
    fig_caption: true
    highlight: "tango"
---






# Location: Nsw
# Most recent sample: 2020-03-17


### Primary author: David Jorgensen

### Report prepared on 2020-04-07

#### On behalf of the MRC GIDA COVID-19 phylodynamics working group at Imperial College London: Lily Geidelberg, Olivia Boyd, Manon Ragonnet, David Jorgensen,  Igor Siveroni, Erik Volz




## Background information  




#### This is analysis is based on : 
  
* **43 whole genomes** sampled from **within Nsw**
* **62 whole genomes** sampled from outside of **Nsw**
* Samples within Nsw were collected between **2020-01-18** and **2020-03-17**


##### To add: [optional plot of sample distribution through time]



## How many are infected in Nsw?





![plot of chunk Cumulative estimated infections through time]({{ site.url }}/reports/20200407-223937-ce202008/SEIJR_plot_size.png)

*Figure 1: Cumulative estimated infections through time. Points represent reported cases in Nsw. The dashed line indicates the date of last sample in Nsw in this analysis.*


* Estimated cumulative infections at last sample (2020-03-17): **3604 [1374-12429]** median [95%CI]

* Cumulative confirmed infections reported at 2020-03-17: 
**210**  

* Cumulative number of active infections at 2020-03-17:  



![plot of chunk daily estimated infections through time]({{ site.url }}/reports/20200407-223937-ce202008/Daily.png)

*Figure 2: Daily estimated infections through time. Points represent reported cases in Nsw. The dashed line indicates the date of last sample in Nsw in this analysis.*





![plot of chunk Rt]({{ site.url }}/reports/20200407-223937-ce202008/Rt.png)

*Figure 3: Reproduction number through time. The dashed line indicates the date of last sample in Nsw in this analysis.*

Reproduction number at last sample (2020-03-17): **1.8 [1.56-2.17]** median [95% CrI]


## How quickly has the epidemic in Nsw grown?




```
## 
## 
## | Quantile | Reproduction number | Growth rate (per day) |
## |:--------:|:-------------------:|:---------------------:|
## |   50%    |        1.81         |        0.0875         |
## |   2.5%   |        1.56         |        0.0629         |
## |  97.5%   |         2.2         |         0.122         |
## 
## Table: Table 1: Reproduction number, growth rate and doubling times (continued below)
## 
##  
## 
## | Doubling time (days) |
## |:--------------------:|
## |         7.92         |
## |         5.69         |
## |          11          |
```





## How has SARS-CoV 2 evolved in Nsw?



![plot of chunk mcc_tree]({{ site.url }}/reports/20200407-223937-ce202008/mcc.png)

*Figure 4: Time scaled phylogeny co-estimated with epidemiological parameters. The colour of the tips corresponds to location sampling; red tips were sampled from within Nsw, blue tips from outside.*



##### Molecular clock rate of evolution: **0.00168 [0.00131-0.0021]** median [95% CrI]  

<!-- #### (optional) Number of introductions into Nsw (someone needs to write code to compute this) -->




## Predicted cumulative infections over next 14 days (assuming exponential growth):



![plot of chunk predicted infections through time]({{ site.url }}/reports/20200407-223937-ce202008/cumu_inf_exp_model.png)

*Figure 5: Cumulative estimated infections. The dashed line indicates the date of last sample in Nsw in this analysis. The points represent reported cases in Nsw.*

Based on an estimated growth rate of 0.0875 [0.0629 - 0.122] median [95% CrI]:  

We estimate cumulative number of infections at last sample (2020-03-17) as: 1063 [138 - 12582]

We estimate number of infections at 2020-03-31 (14 days after last sample) as:
3604 [395 - 68142]  




## Methods summary



Details on methods and priors can be [found here](http://whoinfectedwhom.org/seijr0.1.0_methods.pdf).


Model version: seijr0.1.0

Report version: 20200407-223937-ce202008


## Acknowledgements

This work was supported by the [MRC Centre for Global Infectious Disease Analysis at Imperial College London](https://www.imperial.ac.uk/mrc-global-infectious-disease-analysis).

Sequence data were provided by [GISAID](http://www.epicov.org) and [these laboratories](http://whoinfectedwhom.org/gisaid_cov2020_acknowledgement_table.xls).


