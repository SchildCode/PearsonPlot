# PearsonPlot
A tool to investigate statistical distribution of univariate observations. It plots the skewness-vs-kurtosis of your data (together with bootsrapped samples) on a Pearson-type diagram for comparison with common statsitical distributions. Use it do investigate the possible statistical model describing your data. For example, it helped me discover that thermal conductivity of thermal insulation (which I initially assumed to be log-normal) is actually log-logistic, as it is not a homogeneous material, but is a mixture of two components (air and fibres).

This workbook contains a Visual Basic for Applications (VBA) macro to analyze the statistical distribution of your data, and to generate plots.

The workbook is a further development of [Karl Pearson](https://en.wikipedia.org/wiki/Karl_Pearson)'s diagram (www.wikipedia.org/wiki/Pearson_distribution) which was made popular again by the simpler "[Cullen & Frey](https://www.springer.com/gp/book/9780306459566) plot" in [R](https://cran.r-project.org/web/packages/fitdistrplus/vignettes/paper2JSS.pdf). This workbook vastly improves upon the "Cullen and Frey plot" by comparing the observations with many more common distibutions. Moreover, 3 variants of the plot can be generated, depending on the range of skewness and kurtosis in your data.

## User-instructions
- <b>STEP1</b>: Paste your observations into column A of sheet "InputData". There is no limit to the number of values.
- <b>STEP2</b>: The data is analyzed automatically and plotted when you click on the tab for one of the plots (Chart1, Chart2 or Chart3). The sample skewness and kurtosis of your data is plotted as a black circle, and [bootstrapped](https://en.wikipedia.org/wiki/Bootstrapping_(statistics)) values are plotted with small red dots, to show the range of possible values of the polulation skewness and kurtosis.

## Output options
<p align="center"><img src="images/Chart1.png" alt="Chart 1"/><br/>
<b>Chart 1</b>: Distributions with positive skew in the range 0 to +2 (plotted squared), and excess kurtosis up to +6.</p>
<br/>
<p align="center"><img src="images/Chart2.png" alt="Chart 2"/><br/>
<b>Chart 2</b>: Distributions with skewness in the range +3 to +3, and excess kurtosis up to +8.</p>
<br/>
<p align="center"><img src="images/Chart3.png" alt="Chart 3"/><br/>
<b>Chart 3</b>: Distributions with any value of skewness and kurtosis. Both parameters are squashed into the range -1 to +1. Skewness squared is subtracted from kurtosis before squashing, thus reducing the "impossible region" to a small rectangle, and making  distributions with kurtosis &Proportional; skewness² into horizontal lines.</p>

## Licence
GPL3

## Author and copyright
peter.schild@oslomet.no 
