## Table of contents

The contents of this project are:

1. [Introduction](https://github.com/poojarao76/Supervised-Machine-Learning/tree/main/Regression/CPU_performance#introduction)

2. [The problem statement](https://github.com/poojarao76/Supervised-Machine-Learning/tree/main/Regression/CPU_performance#the-problem-statement)

3. [Dataset description](https://github.com/poojarao76/Supervised-Machine-Learning/tree/main/Regression/CPU_performance#dataset-description)

4. [The problem statement](https://github.com/poojarao76/Supervised-Machine-Learning/tree/main/Regression/CPU_performance#libraries-required)

5. Libraries required

6. [Conclusion](https://github.com/poojarao76/Supervised-Machine-Learning/tree/main/Regression/CPU_performance#conclusion)

## Introduction

In this project, I develop a multiple linear regression model to estimate the relative CPU performance of computer hardware using a dataset that includes machine cycle time, main memory, cache memory, and minimum and maximum channels. 

## The problem statement

The problem is to estimate the relative CPU performance of computer hardware dataset. Relative CPU performance of the computer hardware is described in terms of machine cycle time, main memory, cache memory and minimum and maximum channels as given in the dataset.

## Dataset description

Now, we should get to know more about the dataset. It is a computer hardware dataset. The dataset consists of information about the computer vendors selling computers, model name of computers and various attributes to estimate the relative performance of CPU.

*The dataset can be found at the following url –*

https://archive.ics.uci.edu/ml/datasets/Computer+Hardware

The dataset description will help us to know more about the data.

Dataset description is given as follows:-

vendor name: 30

(adviser, amdahl,apollo, basf, bti, burroughs, c.r.d, cambex, cdc, dec, dg, formation, four-phase, gould, honeywell, hp, ibm, ipl, magnuson, microdata, nas, ncr, nixdorf, perkin-elmer, prime, siemens, sperry, sratus, wang)

*Model Name:* many unique symbols

*MYCT:* machine cycle time in nanoseconds (integer)

*MMIN:* minimum main memory in kilobytes (integer)

*MMAX:* maximum main memory in kilobytes (integer)

*CACH:* cache memory in kilobytes (integer)

*CHMIN:* minimum channels in units (integer)

*CHMAX:* maximum channels in units (integer)

*PRP:* published relative performance (integer)

*ERP:* estimated relative performance from the original article (integer)

## Libraries required

* Numpy 
* Pandas
* Matplotlib
* Seaborn
* sklearn

## Conclusion

The R-squared or the coefficient of determination is 0.4691 on an average for 5-fold cross validation. It means that the predictor is only able to explain 46.91% of the variance in the target variable. This indicates that the model is not a good fit to the data. We can see that the variables do not follow the normal distribution. The Q-Q plots confirm the same.

So, we can conclude that the linear regression model is unable to model the data to generate decent results. It should be noted that the model is performing equally on both training and testing datasets. 