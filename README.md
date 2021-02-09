# Choo Jun Jie's Portfolio

# Thesis: [Hamiltonian Monte Carlo and No-U-Turn Sampler](https://github.com/junjiechoo24/projects/tree/main/thesis)

Hamiltonian Monte Carlo (HMC) is a Markov chain Monte Carlo (MCMC) method that is able to effectively sample high dimensional target distributions by using Hamilton’s equations to design a proposal mechanism that exploits the target geometry. However, HMC’s performance is highly sensitive to tuning parameters. The No-U-Turn
Sampler (NUTS) eliminates the need to hand-tune parameters, whilst showing a competitive performance when compared with a well tuned vanilla HMC. This thesis will provide a background introduction to HMC and describe in detail the NUTS algorithm. Several numerical simulations will illustrate the flexibility of the NUTS algorithm and its practical advantage over vanilla HMC.

# Project 1: [Monte Carlo Convergence Diagnostics Project](https://github.com/junjiechoo24/projects)

Markov chain Monte Carlo (MCMC) is one of the most useful approaches to scientific computing because of its flexible construction, ease of use, and generality. Two critical questions that MCMC practitioners need to address are where to start and when to stop the simulation. Although a great amount of research has gone into establishing convergence criteria and stopping rules with sound theoretical foundation, in practice, MCMC users often decide convergence by applying empirical diagnostic tools. This review article discusses the most widely used MCMC convergence diagnostic tools.

# Project 2: [Vanilla and Generalised Elliptical Slice Sampling](https://github.com/junjiechoo24/projects)

Many probabilistic models introduce strong dependencies between variables using a latent multivariate Gaussian distribution or a Gaussian process. We present a new Markov chain Monte Carlo algorithm for performing inference in models with multivariate Gaussian priors. Its key properties are:

1. it has simple, generic code applicable to many models,
2. it has no free parameters,
3. it works well for a variety of Gaussian process based models.

These properties make our method ideal for use while model building, removing the need to spend time deriving and tuning updates for more complex algorithms.

# Project 3: [Regression and Permutation Test](https://github.com/junjiechoo24/bikeshare)

The data set is the Capital Bikeshare data set, from https://www.capitalbikeshare.com/system-data. This data comes from Washington D.C.’s bikeshare program, which records every individual ride taken. Each ride is tagged with its start and end time, start and end station (there are hundreds of locations where bikes can be rented across the city), as well as whether the rider has bought a one-time rental or is a member of the bikeshare program.

A script named getdata_bikeshare.R is used to download and clean the data so that it’s ready for R and organized in a simple format.

The following question was studied: Can any routes be detected (i.e., a particular combination of start & end station) where the average time it takes to travel the route, changes over the course of the time period? For example, if a bike lane is added to a major road, this may reduce the travel time for that particular route.

Methodology:

Cluster the data by route, and run a linear model on confounders only, i.e. Days since Jan1 2010 is not part of the model.
Within each cluster, use the residuals for permutation test, but group the residuals by day and permute the groups instead of the individual residuals, in order to account for the dependency of data belonging to the same day.

# Project 4: [Real Data Analysis Critique](https://github.com/junjiechoo24/projects)

The paper critiqued was “Lung cancer incidence decreases with elevation: evidence for oxygen as an inhaled carcinogen”, Simeonov & Himmelstein, PeerJ 2015 https://peerj.com/articles/705/

The statistical analyses performed in the paper was critiqued from the point of view of multiple testing and replicability. The validity of the conclusions was also assessed from a statistician’s point of view

Some ideas are: thinking about possible confounding variables, whether the data collected is representative of the claim being made, etc.

# Project 5: [Covid-19 Figures Report](https://github.com/junjiechoo24/projects/tree/main/covid)

Background: People are sharing Figure 1 on twitter where the figure comes from this report: https://medium.com/
@andreasbackhausab/coronavirus-why-its-so-deadly-in-italy-c4200a15a7bf

![Figure](https://imgur.com/a/UezBBsM)

This figure compares between Italy and South Korea. It catches people’s eyes because this may show that there can be a lot of infected young people in Italy that are missed as they show no or mild symptoms, and they may spread the virus to others unconsciously. As pointed out in the source report, Italy has predominantly been testing people with symptoms of a coronavirus infection, while South Korea has been testing basically everyone since the outbreak had become apparent. Consequently, South Korea has detected more asymptomatic, but positive cases of coronavirus than Italy, in particular among young people.

However, looking at Figure 1 alone is not enough to get the above conclusion as the age structure in the two countries are also different. Even if both two countries can diagnoses every effected case, you would see a higher fraction of elder people diagnosed in Italy than in South Korea since Italy has one of the oldest populations in the world.

If Italy has missed a lot of younger patients who have no or milder symptoms, we can give an estimate of how many people are actually infected in Italy at this moment using logistic regression.



# Report 1: [Data Analysis for Titansoft Technical Interview](https://github.com/junjiechoo24/reports/tree/titansoft)

This is my report to a technical interview for a data analyst role at Titansoft. Models used were Logistic regression and negative binomial model.


