# sampling-code-in-R
THE CODE USED FOR DIFFERENT TYPES OF SAMPLING TECHNIQUES USED IN R ,USING DIFFERENT PACKAGES




#########TYPES OF SAMLINGS###########

###########STRATIFIED SAMPLING#####
Stratified sampling is a probability sampling technique wherein the researcher divides the entire population into different subgroups or strata, then randomly selects the final subjects proportionally from the different strata.

1)Stratified sampling is a probability sampling technique wherein the entire dataset is divided into different subgroups or strata, then randomly selects the final subjects proportionally from the different strata.
However while using this technique it is important that the strata must be non-overlapping. Because, an overlapping subgroups may lead to higher chances of some datapoints being selected over others. And this would completely negate the concept of stratified sampling as a type of probability sampling.

After dividing dataset in different stratums -
Proportionate Stratified Random Sampling - All stratum have same sampling fraction
Disproportionate Stratified Random Sampling - Different stratums have different sampling fractions

Stratified Sampling is normally used when the trainig dataset is huge and its difficult to use entire dataset for model training purpose.

2)Stratified sampling is a sampling method that takes into account the existence of disjoint groups within a population and produces samples where the proportion of these groups is maintained and in our case these groups are labels for digits from 0 to 9 each.

The command sample.split ensures that the labels of the samples created after splitting are in same ratio.

Example - Say you have data with 70% Y values and 305 N Values. Sample.split will ensure that the data in the sample will be of the same ratio as in the original dataset.

You can also try createDataPartition from caret package. Its document states: By default, createDataPartition does a stratified random split of the data.

ref

https://link.springer.com/chapter/10.1007/978-3-642-23808-6_10

https://stackoverflow.com/questions/20776887/stratified-splitting-the-data
