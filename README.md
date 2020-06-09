# PearsonPlot
A tool to investigate statistical distribution of univariate observations. Plots skewness-vs-kurtosis of your data (together with bootsrapped observations) on a Pearson diagram, and compares to common statsitical distributions.

This workbook contains one Visual Basic for Applications (VBA) macro do analyze the statistical distribution of observations.

The workbook is a further development of Karl Pearson's diagram (www.wikipedia.org/wiki/Pearson_distribution) which was made popular again by the simplifed Cullen & Frey plot in R. This workbook vastly improves upon the Cullen and Frey plot by comparing the observations with many common distibutions. Moreover, 3 variants of the plot can be generated, depending on the range of skewness and kurtosis in your data.

## User-instructions
STEP1: Paste your observations into column A of sheet "InputData". There is no limit to the number of values.
STEP2: The data is analyzed automatically and plotted when you click on the tab for one of the plots (Chart1, Chart2 or Chart3).

## Output options
<p align="center"><img src="images/chart1.png" alt="Chart 1"/><br/>
  <sub>Chart 1: Distributions with positive skew in the range 0 to +2 (plotted squared), and excess kurtosis up to +6.</sub></p>
  
<p align="center"><img src="images/chart2.png" alt="Chart 2"/><br/>
  <sub>Chart 2: Distributions with skewness in the range +3 to +3, and excess kurtosis up to +8.</sub></p>

<p align="center"><img src="images/chart2.png" alt="Chart 2"/><br/>
  <sub>Chart 3: Distributions with any value of skewness and kurtosis. Both parameters are squashed into the range -1 to +1. Skewness squared is subtracted from kurtosis before squashing, thus reducing the "impossible region" to a small rectangle, and making  distributions with kurtosis &Proportional; skewness² into horizontal lines.</sub></p>

## Licence
GPL3

## Author and copyright
peter.schild@oslomet.no 