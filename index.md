---
title       : A/B Test App
subtitle    : An Explaination
author      : YQ
job         : student
framework   : io2012      # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     :     # 
widgets     : mathjax          # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction to A/B Test

### What is A/B test?
A/B testing is jargon for a randomized experiment with two variants, A and B, which are the control and treatment in the controlled experiment. A/B test is frequently used in online marketing to identify changes to web pages that increase or maximize an outcome of interest.

### Statistical Analysis of This App

The statistical analysis has been done with a Pearson's Chi-square test. Yates's correction for continuity is used to reduce the error in the observed binomial frequency's approximation to continuous Chi-square distribution The input data is used to contruct a contingency table and that contingency table is used as an input for performing the Chi-square test.


--- .class #id 

## Guideline for Usage

### Input

To use this App, users are supposed to input the number of objects converted both in the control and treatment group. They also need to input the total number of objects in control and treatment group.

### Output

Once the "Submit" button is pressed, the App will calculate the conversion rates of both __control__ and __treatment__ group and show a graphical representation of the converted objects in both groups. It will also tell if the treatment significantly changes the conversion rate.

---


## Demo

An online retailer recently developed a new landing page and they want to know this new landing page's influence upon people's purchase behavior. The company conducted a test by randomly assigning visitors  to the old (control) and new (treatment) landing pages within certain period of time and collected the ordering data by visitors. 353 of 9985 old landing page visitors clicked their mouses to place an order while 401 of 10008 new landing page visitors clicked their mouses to place an order in this test. The manager wants to know if people are more/less likely or not to place an order when they land at this new landing page when they visit the website.

Group |Control  | Treatment
------------- |------------- | -------------
Converted |353  | 401
Nonconverted  | 9985 | 10008


---

## Demo (Cont')

A graphical representation is firstly obtained




The statistical test is performed at $\alpha$ = 0.05 level


```
## 
## 	Pearson's Chi-squared test with Yates' continuity correction
## 
## data:  contTable
## X-squared = 2.9332, df = 1, p-value = 0.08678
```

### Conclusion
Treatment group is not significantly ( $\alpha$    = 0.05 ) different from control group.

