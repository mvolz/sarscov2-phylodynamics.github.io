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






# Location: Hongkong
# Most recent sample: 2020-03-14


### Primary author: Manon Ragonnet

### Report prepared on 2020-04-07

#### On behalf of the MRC GIDA COVID-19 phylodynamics working group at Imperial College London: Lily Geidelberg, Olivia Boyd, Manon Ragonnet, David Jorgensen,  Igor Siveroni, Erik Volz




## Background information  




#### This is analysis is based on : 
  
* **27 whole genomes** sampled from **within Hongkong**
* **43 whole genomes** sampled from outside of **Hongkong**
* Samples within Hongkong were collected between **2020-01-21** and **2020-03-14**


##### To add: [optional plot of sample distribution through time]



## How many are infected in Hongkong?





<img src="SEIJR_plot_size.png" width="1050" />

*Figure 1: Cumulative estimated infections through time. Points represent reported cases in Hongkong. The dashed line indicates the date of last sample in Hongkong in this analysis.*


* Estimated cumulative infections at last sample (2020-03-14): **432 [35-21603]** median [95%CI]

* Cumulative confirmed infections reported at 2020-03-14: 
**141**  

* Cumulative number of active infections at 2020-03-14:  



<img src="Daily.png" width="1050" />

*Figure 2: Daily estimated infections through time. Points represent reported cases in Hongkong. The dashed line indicates the date of last sample in Hongkong in this analysis.*





<img src="Rt.png" width="1050" />

*Figure 3: Reproduction number through time. The dashed line indicates the date of last sample in Hongkong in this analysis.*

Reproduction number at last sample (2020-03-14): **3.59 [2.6-4.71]** median [95% CrI]


## How quickly has the epidemic in Hongkong grown?



<table class="table" style="width: auto !important; ">
<caption>Table 1: Reproduction number, growth rate and doubling times</caption>
 <thead>
  <tr>
   <th style="text-align:center;"> Quantile </th>
   <th style="text-align:center;"> Reproduction number </th>
   <th style="text-align:center;"> Growth rate (per day) </th>
   <th style="text-align:center;"> Doubling time (days) </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> 50% </td>
   <td style="text-align:center;"> 3.65 </td>
   <td style="text-align:center;"> 0.231 </td>
   <td style="text-align:center;"> 3.00 </td>
  </tr>
  <tr>
   <td style="text-align:center;"> 2.5% </td>
   <td style="text-align:center;"> 2.78 </td>
   <td style="text-align:center;"> 0.169 </td>
   <td style="text-align:center;"> 2.17 </td>
  </tr>
  <tr>
   <td style="text-align:center;"> 97.5% </td>
   <td style="text-align:center;"> 5.09 </td>
   <td style="text-align:center;"> 0.320 </td>
   <td style="text-align:center;"> 4.10 </td>
  </tr>
</tbody>
</table>





## How has SARS-CoV 2 evolved in Hongkong?



<img src="mcc.png" width="600" />

*Figure 4: Time scaled phylogeny co-estimated with epidemiological parameters. The colour of the tips corresponds to location sampling; red tips were sampled from within Hongkong, blue tips from outside.*



##### Molecular clock rate of evolution: **0.000657 [0.000511-0.000932]** median [95% CrI]  

<!-- #### (optional) Number of introductions into Hongkong (someone needs to write code to compute this) -->




## Predicted cumulative infections over next 14 days (assuming exponential growth):



<img src="cumu_inf_exp_model.png" width="1050" />

*Figure 5: Cumulative estimated infections. The dashed line indicates the date of last sample in Hongkong in this analysis. The points represent reported cases in Hongkong.*

Based on an estimated growth rate of 0.231 [0.169 - 0.320] median [95% CrI]:  

We estimate cumulative number of infections at last sample (2020-03-14) as: 3700 [458 - 53686]

We estimate number of infections at 2020-03-14 (0 days after last sample) as:
3700 [458 - 53686]  




## Methods summary



Details on methods and priors can be [found here](http://whoinfectedwhom.org/seijr0.1.0_methods.pdf).


Model version: seijr0.0.0

Report version: 20200407-224313-c37a4344


## Acknowledgements

This work was supported by the [MRC Centre for Global Infectious Disease Analysis at Imperial College London](https://www.imperial.ac.uk/mrc-global-infectious-disease-analysis).

Sequence data were provided by [GISAID](http://www.epicov.org) and [these laboratories](http://whoinfectedwhom.org/gisaid_cov2020_acknowledgement_table.xls).


