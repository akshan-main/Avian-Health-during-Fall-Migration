# Avian-Health-during-Fall-Migration

The dataset consists of data pertaining to birds in the August to October time period collected from 2010 until 2020. The data includes birds from two different locations within north central New Mexico. These locations occur near the overlap of the Pacific and Central migratory bird flyways and the migratory birds most likely come into the study area from both flyways. The birds were banded as per the The North American Bird Banding Manual. The identification and sexing criteria was based on Identification Guide to North American Passerines. Birds were grouped into either one of insectivore, granivore or omnivore on basis of their dieting habits as per life history information available from Cornell’s The Birds of North America Online.

The birds were categorized as either breeding in the area or migrants. Our dataset consists of 15,244 individuals from 71 species, of which 44 species were considered to be migrants. The Palmer Drought Severity Index (PDSI) is a standardized index that spans from −10 (dry) to +10 (wet), and has been quite successful at quantifying long-term drought. PDSI value of 0.0 to −0.5 means the conditions are normal; −0.5 to −1.0 alludes to incipient drought; −1.0 to −2.0 corresponds to mild drought; −2.0 to −3.0 means moderate drought; −3.0 to −4.0 is severe drought and anything below -4.0 is classified as
extreme drought as per The Climate Data Guide: Palmer Drought Severity Index (PDSI).Fat score is an estimate of the total tissue depth (fat + muscle). The categories within fat scores comprises of “none”, “trace”, “light”, “half”, “filled”, “bulging”, “greatly bulging”, and “very excessive". Fuel stores fluctuates seasonally and that’s why fat score is a better metric of usage here than body mass. The 
categories of fat scores here are set forth by the Institute for Bird Populations. Data from birds captured during the same year were excluded because we wanted to compare fat scores between the years. The “rare” species caught ≤ 3 times were removed from the 10-year dataset. The data is standardized for further analyses by grouping the subspecies into species category. Multiple logistic regression models were employed to formulate the influence of age, residency, feeding guild coupled with a drought index. We grouped response variable of fat score into two values. One is “none”, which is equal to 0 and all the other categories are 1. The grouping is done in this manner to tackle zero inflation problems since nearly half of fat scores were categorized as “none”. If a migrant bird has a fat score greater than zero during fall migration, its in a better psychological condition. We use the R statistical software here and the libraries used are dplyr, tidyverse, ggplot2.

The Akaike information criterion (AIC) is an estimator of predictor error and thereby relative quality of statistical models for a given set of data. Given a collection of models for the data, AIC estimates the quality of each model, relative to each of the other models. Thus, AIC provides a means for model selection. AIC is founded on information theory. When a statistical model is used to represent the process that generated the data, the representation will almost never be exact; so some information will be lost by using the model to represent the process. AIC estimates the relative amount of information lost by a given model: the less information a model loses, the higher the quality of that model. Also , more the number of predictor variables , it constitutes to a better model. In estimating the amount of information lost by a model, AIC deals with the trade-off between the goodness of fit of the model and the simplicity of the model. In other words, AIC deals with both the risk of overfitting and the risk of underfitting.
Model selection results of logistic regression models for estimating fat score in relation to Palmer Drought Severity Index (PDSI) from New Mexico region 2 climate division, diet classification (insectivore, granivore and omnivore), residency (migratory versus year-round resident) and age (hatch year versus after hatch year)with respect to the data collected from 2010 to 2020. Model selection based on Akaike’s Information Criterion (AIC), and difference in AIC between each model compared to the model with the lowest AIC (ΔAIC) is evaluated .The candidate model set was based on combinations of variables contributing to avian health. correlated variables with a variance inflation factor >5 were not included in the same model or candidate set of models as per Regression Diagnostics: Identifying Influential Data and Sources of Collinearity.
