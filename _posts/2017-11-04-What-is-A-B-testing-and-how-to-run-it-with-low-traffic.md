---
layout: post
title: What is A/B testing and how to run it with low traffic 
image: /img/ab-testing.jpg
tags: [A/B testing, Growth Analytics, Marketing Analytics, Web Analytics, Conversion, Optimisation]
---

Many websites don’t have a huge amount of traffic. This makes it difficult to run **A/B tests** (experiments) for changes to websites. I’ll try to explain what an experiment is and what the requirements are to successfully run an experiment.
 
**What is A/B testing:** A/B testing (also known as *split testing* or *bucket testing*) is a statistical experiment to compare two versions of a webpage (or an app, or email campaigns) against each other to determine which one performs better. During A/B testing, two variants of a page are shown to different group of users, and statistical techniques are used to determine which variation performs better for a given conversion goal. In case of A/B, we test two variants (control and test). If we want to test more than two variants at the same time, it’s called *multivariate testing* (A/B/C/… testing).
 
**The statistical foundation of A/B testing:** It is [hypothesis testing](https://en.wikipedia.org/wiki/Statistical_hypothesis_testing). First, we come up with our hypothesis; ‘version B is not different than A’ (this is our null hypothesis (H0) and we want to reject that).

Let’s assume we are testing two versions of an email campaign, we want to see if we will have higher *click through rates* (CTR) when we change the email subject line. In bucket A, we have 2,000 randomly selected email subscribers from our database. In bucket B we have another 2,000 randomly selected email subscribers and we send two versions of the email campaign to those users.
 
Then we compute our *p-value*, which is the probability of observing an effect given that the null hypothesis is true. Usually, if the p-value < 5%, it is considered statistically significant. [This is how we calculate it](https://abtestguide.com/calc/).

Assuming that, during our test, 200 of the emails have been clicked through in bucket A (10% conversion), and 250 of the emails have been clicked through in bucket B (12.5% conversion). In this case, with 95% confidence, the calculated p-value is 0.0061, which is smaller than 0.05. So the test results are statistically significant. We can say that version B is performing better than version A. Our uplift is 2.5%.
 
**Sample size calculation:** In order to run a hypothesis test, we need enough number of visitors for each bucket (control and test). A choice of small sample sizes can result in wide confidence intervals or risks of errors in statistical hypothesis testing. [This is how we calculate our sample size](https://www.optimizely.com/sample-size-calculator/?conversion=2&effect=10&significance=95). *Minimum Detectable Effect* is the uplift we expect. Notice that the higher effect we expect, the lower sample size we will need. Play around with that calculator and see the changes. *Google recommends at least 100 conversions per page before deciding which version is best*.
 
**Test duration:** You may use [this](https://vwo.com/ab-split-test-duration/) calculator to see the duration of the test. Airbnb has published a great article about test duration. You may find it [here](https://medium.com/airbnb-engineering/experiments-at-airbnb-e2db3abf39e7).
 
### Your challenge: Not having a huge amount of website traffic (or email subscribers)

Unfortunately not all websites have enough traffic -or email subscribers- to run A/B tests. In this case we may take different approaches to our decision making process;

1. **A/B test with tweaks:**

 * **Test for dramatic changes**
 If you don’t have a high volume of traffic, you may need to test the pages for more dramatic changes (higher improvement rate=smaller sample size).
 
 * **Focus on micro-conversions:**
 Instead of focusing on main conversion rates such as purchased products on an ecommerce website or sign-ups in general, you may track the conversion to number of pageviews for particular pages.
 
 * **Boost the test traffic with marketing campaigns:**
 You may try to drive traffic via PPC or email campaigns.
 
2. **5 Second test:**
[This](https://fivesecondtest.com/) website allows you to run experiments by uploading screenshots (or dummy) of two versions of your webpage. I think it’s a great alternative to traditional A/B testing. 
 
3. **User testing:**
Having users testing the current product (and the versions as well maybe). You may find 5-10 people to test your product and give you feedback or try [Usertesting](http://www.usertesting.com/), [TryMyUI](http://www.trymyui.com/), or [YouEye](https://www.youeye.com/) for a wider scope.
 
4. **Mouse tracking heat maps:**
Tracking your users’ movements on your website will give you a great insight about the user journey. Try [Mouseflow](https://mouseflow.com/) (or Feng-GUI, EyeQuant, LookTracker) to see the blockers for conversion.
 
5. **Collect insight from users directly:**
Invest in a live chat solution such as [Intercom](https://www.intercom.com/live-chat). This will help you to understand the problems your users face when they use the website.
 
Hope this helps you to understand what A/B testing is and what the alternative approaches are. Please leave your comments below.

