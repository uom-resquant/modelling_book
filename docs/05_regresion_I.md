# Regression I: Mean differences
## Hypotheses: The logic of hypothesis testing

In the last unit, we learned how to think about and build confidence intervals. We explained how we could use confidence intervals to deal with uncertainty when estimating population parameters. Confidence intervals as we will see are very commonly used in statistics. The other key inferential tool in data analysis is the hypothesis test. Today, we will focus on this second tool. 

Last week, we saw how we could use confidence intervals as well to form a view about whether there are differences across groups in the population. We also saw how we could do "inference by eye" by virtue of visually comparing the confidence interval for the estimated mean value of fear for men and the estimated mean value of fear for women. Now, we are going to use a different approach to make inferences about the existence of these differences in the population: hypothesis testing.

Wikipedia defines a statistical hypothesis test as "a method of making decisions using data from a scientific study". The logic of hypothesis testing is based on the work of a number of pioneers in the field of statistics, the British Ronald Fisher and Egon Pearson and the Polish Jerzy Neyman. This work is so important that [some people argue](https://simplystatistics.tumblr.com/post/18903448428/ra-fisher-is-the-most-influential-scientist-ever) that Sir Ronald Fisher is one of the most influential academics in the history of science; not a small feat! 

Hypothesis testing, or null hypothesis testing (NHST) as it is often referred to, proceeds in a number of steps. 

1.**We always start with a research question** 

Our research questions in criminology can vary: Are ethnic minorities more likely to be stopped and searched? Does punishing offenders reduce crime? Is crime going down? Is self-control associated with offending? Here we are asking, are women more afraid of violent crime than men?

2.**To answer a research question, we have to formulate at least one and sometimes several research hypotheses related to it** 

A research hypothesis is simply a proposed answer to our research question that we can test by carrying out some research. Research hypothesis can be directional and non-directional:

>"When the research hypothesis does not indicate a specific type of outcome, stating only that there is a relationship or a difference, we say that it is a **non-directional hypothesis**. However, in those cases where a researcher has a very clear idea of what to expect -based on prior research evidence and/or theory -the research hypothesis may be more precise. In this case, the researcher may specify the nature of the relationship that is expected. Such a research hypothesis is called a **directional hypothesis**. When a directional hypothesis is used, the researcher states at the outset that he or she is interested in a specific type of outcome -for example, that one group has more arrests than another. Suppose we are interested in comparing the arrest records of drug-involved offenders with those of offenders who do not use drugs. Our research hypothesis might be simply that the arrest records of drug-involved offenders and offenders who do not use drugs are different (a nondirectional hypothesis). But based on prior knowledge of criminal behaviour among drug-involved offenders, we might want to state a directional hypothesis -that drug-involved offenders have more serious arrest records than non-drug-involved offenders do. One problem with choosing the latter option is that if we state our research hypothesis as a directional hypothesis, we are stating that we are not interested in outcomes that fall in the opposite direction. In criminal justice research, we can often be surprised by what we learn in a study. Accordingly, researchers generally are cautious in defining a directional research hypothesis" (Weisburd and Britt, 2010: 120)

In our example, the research hypothesis will be non-directional and simply state that there are differences in the fear of violent crime among men and women.

3. **The following step is to formulate what is called a null hypothesis**

In frequentist statistical inference we test hypothesis not in reference to the research hypothesis but in reference to the **null hypothesis**. The null hypothesis gains its name from the fact that it usually states that there is no relationship or no difference. "We make decisions about the hypothesis in relation to the null hypothesis rather than the research hypothesis. This is because the null hypothesis states that the parameter in which we are interested is a particular value" (Weisburd and Britt. 2010: 122). 

In the example that we are using, the null hypothesis would be that there is no difference in the mean level of fear for males and females. This is the same than saying that the difference on fear for these two groups is zero. So, using the null hypothesis gives us a specific value. Typically, this value is zero, whereas the research hypothesis would be consistent with any of many values other than zero.  We will see in a second why working with a precise value such as zero is helpful.

De Veaux et al. (2012) explain the logic of hypothesis testing as being similar to the logic of jury trials. In jury trials within the Common Law tradition, somebody is innocent until proven guilty:

>"the null hypothesis is that the defendant is innocent... The evidence takes the form of facts that seem to contradict the presumption of innocence. For us" (researchers) "this means collecting data... The next step is to judge the evidence. Evaluating the evidence is the responsibility of the jury in a trial, but it falls on your shoulders in hypothesis testing. The jury considers the evidence in light of the presumption of innocence and judges whether the evidence against the defendant would be plausible if the defendant were in fact innocent. Like the jury, you ask, **'Could these data plausibly have happened by chance if the null hypothesis were true?'** If they are unlikely to have occurred, then the evidence raises a reasonable doubt about the null hypothesis. Ultimately, you must make a decision. The standard of beyond a reasonable doubt is wonderfully ambiguous... But when you ask the same question of your null hypothesis, you have the advantage of being able to quantify exactly how surprising the evidence would be were the null hypothesis true" (De Veaux et al. 2012: 479)

So, in hypothesis testing, we look at our observed sample data. In our case, we look at the difference in fear of violent crime for males and females, and we ask ourselves the question: is the observed difference likely to have come from a population where the real difference is zero (as our null hypothesis specifies)? As you can see, testing against the null gives us the advantage of testing against a specific value. We can compare the value that we observe with zero, the precise value hypothesised by the null hypothesis. *The downside of it is that few things are exactly the same in nature*. So, to say that the level of fear of crime in men and women is probably not exactly the same (e.g., a difference of zero) is arguably not always going to give us the answer that we want.

4. **The fundamental step in hypothesis testing, therefore, is the question: are the observed data surprising, given the null hypothesis? The key question is to determine exactly how likely the data we observed would be were the null hypothesis a true model of the world**

So in essence we are after a probability, specifically a conditional probability (i.e, *the probability of our data if the null hypothesis were true*). We are trying to quantify the probability of seeing data like the one we have observed (a difference of 0.79 in our example) if we take as given that the null hypothesis is true (and the value "should be" zero). We call this probability the **p value**. You may have heard this term before. All it means, it bears repeating, is **the probability of observing our data if the null hypothesis were true**.

>"**When the p value is high**, then we can conclude that we have not seeing anything unusual. Events that have a high probability of happening happen often. The data are thus consistent with the model from the null hypothesis, and we have no reason to reject the null hypothesis. But we realize many other similar hypotheses could also account for the data we've seen, so we haven't proven that the null hypothesis is true. The most we can say is that it doesn't appear to be false. Formally, we fail to reject the null hypothesis. That's a pretty weak conclusion, but it's all we're entitled to. **When the p value is low enough**, it says that it's very unlikely we'd observed data like these if our null hypothesis were true. We started with a model. Now, the model tells us that the data are unlikely to have happened. The model and the data are at odds with each other, so we have to make a choice. Either the null hypothesis is correct, and we've just seen something remarkable, or the null hypothesis is wrong..." (De Veaux et al. 2012: 480)

When is a p value high and when is low? Typically, we use criteria similar to those we use when constructing confidence intervals: we would consider a p value low enough if 95% of the time the observed data was considered to be inconsistent with the model proposed by our null hypothesis. So, we look for p-values that are smaller or bigger than 0.05.

That is, we look for differences that happen less than 5% of the time before we tentatively reject the null hypothesis. However, there is nothing sacrosanct about 95% and you could have good reasons to depart from this criterion (read page 123 to 128 of Weisburd and Britt, 2010 for further details). In fact, only last year, a number of researchers argued we should use a more stringent p value to address the crisis of reproducibility in science.

You will see that statistics books refer to the threshold we use to define a p-value as high or low as our **level of statistical significance** (also often referred to as the **alpha level**). In our example here (and all the others we will use this semester), we will use an alpha level of 0.05. That is, we will reject the null hypothesis *only if our p level is below that threshold*.

5. **After defining our research and null hypothesis and having taken a decision of how low our p value ought to be in order to reject the null hypothesis, we need to specify a model for testing this null hypothesis. All models make assumptions, so an important part of specifying a model is stating your assumptions and checking that they are not being violated. **

Throughout the semester, we will cover a number of statistical tests, all with their own assumptions. These tests are appropriate in different circumstances (defined by their assumptions). Basically, what we will be doing in the remaining thematic units this semester is to explain what those circumstances are for each test so that you can choose the right one on each occasion. We will see later the assumptions made by the sort of hypothesis tests you use to compare means across groups.

6. **Once we've gone through all those steps comes the calculation of the test statistics and, based on the results, our decision**

Different tests that we will encounter this semester have different formulas. Sometimes I will give you a basic description of what those formulas are doing, because it is good to know what is being computed for conceptual understanding. But the mechanics are handled by the computer. You won't need to memorise those formulas nor calculate anything yourself.

The ultimate goal of these statistical tests for hypothesis testing is to obtain a p-value: the probability that the observed statistic (or a more extreme value) occurs if the null model is correct. If the p value is small enough (smaller than our alpha level: such as 0.05) then we will **"reject the null hypothesis"**. If it is not, we will **"fail to reject the null hypothesis"**. The language is important.

Whatever you decide, the *American Psychological Association Statistical Committee* recommends that it is always a good idea to report the p-value as an indication of the strength of the evidence. That is, not only report the finding to be significant or not, also report your actual p value.

One final word. P values have attracted a lot of debate over the years. They are often misunderstood, and people often read too much into them. They have also been used in a too simplistic way as a yardstick to decide what research findings are "worthy". It is important to know what they are and how they work. It is particularly important not to overinterpret them either. The term statistical **significance** is particularly misleading because in common usage we think of something significant as important. But in our context is basically equivalent to say that we have observed in our sample/study may not be noise. That's it. You will find all sorts of reactions to p values. Some people think we should ban them and use alternative approaches to data analysis (like Bayesian statistics). Others think that we should use more stringent thresholds (like p-values below .01 or .001). Yet most scientists still rely on them, so it is important that you learn what they are, their limitations, and how to interpret them in a correct manner.

## Power analysis

In this section, we introduce the `pwr` package for power analysis. In the video lectures you had to watch as preparation for today we introduced the notion of power analysis. In order for a statistical test to be able to be effective, to be able to detect an effect, you need to have sufficient power. Power is related to the magnitude of the effect (it will be easier to detect stronger rather than weaker effects) and sample size (it will be easier to detect effects with large samples than with small samples). A problem with many scientific studies is that they are *underpowered*, the fail to reject the null hypothesis simply because they do not have sufficient power (often because the sample size is not large enough). Power analysis is generally done during the planning of an analysis so that you know what kind of sample you are going to need if you want to be able to run meaningfull hypothesis tests. That is you do your power analysis before you collect your data. 

But we can also check how much power we have after the fact, just to ensure we are not failing to reject the null hypothesis as a consequence of insufficient power. For this purposes we can use the `pwr` package. For computing the power when comparing two sample means we use the `pwr.t2n.test` function. This function expects we provide the sample size of each group (if we are doing the power calculation after we have collated our data) and the effect size we may want to be able to detect. Let's see how many people we have in each of our two groups (male and female) when assessing differences in fear of violent crime.



```r
library(psych)
BCS0708<-read.csv("https://raw.githubusercontent.com/eonk/dar_book/main/datasets/BCS0708.csv")
describeBy(BCS0708$tcviolent, BCS0708$sex)
```

```
## 
##  Descriptive statistics by group 
## group: female
##    vars    n mean   sd median trimmed  mad   min  max range skew kurtosis   se
## X1    1 4475 0.33 1.04   0.23    0.25 0.96 -2.35 3.56  5.91 0.61     0.02 0.02
## ------------------------------------------------------------ 
## group: male
##    vars    n  mean   sd median trimmed  mad   min  max range skew kurtosis   se
## X1    1 3959 -0.27 0.86  -0.44   -0.36 0.69 -2.35 3.81  6.16  1.1     1.91 0.01
```

Ok, so that is 4475 and 3959. Let's say we want to detect even very small effect sizes. The functions in this package assume a default .05 level of statistical significance, although this is something we could change. So if we go with the default, we would write as follows:


```r
library(pwr)
```

```
## Warning: package 'pwr' was built under R version 4.3.2
```

```r
pwr.t2n.test(n1 = 4475, n2 = 3959, d= 0.2)
```

```
## 
##      t test power calculation 
## 
##              n1 = 4475
##              n2 = 3959
##               d = 0.2
##       sig.level = 0.05
##           power = 1
##     alternative = two.sided
```

The function is telling us that we have a power of 1. The statistical power ranges from 0 to 1, and as statistical power increases, the probability of making a type II error (wrongly failing to reject the null) decreases. So with a power of 1 we are very unlikely indeed to failing to reject the null hypothesis when we should.

With sample sizes this large, you are unlikely to run into problems with power. But these things do matter in particular applications. Think for example of cases when you are trying to evaluate if a particular criminal justice intervention works. If you work with small samples you may wrongly conclude that your intervention didn't make a difference (you fail to reject the null hypothesis) because you did not have sufficient statistical power. This was a common problem in older studies (see [here](https://www.sciencedirect.com/science/article/pii/0047235289900044) for a review) and it is a problem that still persist to some extent (read [this](https://www.tandfonline.com/doi/abs/10.1080/07418825.2018.1495252) more recent review).

