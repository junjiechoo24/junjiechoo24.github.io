# Choo Jun Jie's Portfolio



# Training an AI Model to Sing!

In this project, I leveraged the So-VITS model to transform isolated voice samples of the character Noa from Blue Archive into musical performances. The process involved training the model on these voice samples, then using audio analysis techniques to separate target songs into instrumental and voice tracks for inferencing, before blending the song's instrumentals and newly inferenced voice tracks again for the full song!

You can watch the videos below on YouTube:

### [Even if it's your happiness](https://youtu.be/dAj5I4rhsZc)
[![Even if it's your happiness](https://img.youtube.com/vi/dAj5I4rhsZc/0.jpg)](https://youtu.be/dAj5I4rhsZc)

### [Yume to Hazakura](https://youtu.be/DQyZHKgjF34)
[![Yume to Hazakura](https://img.youtube.com/vi/DQyZHKgjF34/0.jpg)](https://youtu.be/DQyZHKgjF34)


### Skills: Python, Deep Learning


---
<br><br> <!-- Adding additional spacing -->


# [GCP Project to analyse PvP match results for Blue Archive](https://github.com/junjiechoo24/discord_bot_pvp/tree/master)

![Blue Archive PvP Analysis](https://drive.google.com/uc?id=11LgIJYlc79NX8gjipqzLADvb9pt6uNk2)

## Project Overview

The primary goal of this project is to gather win/lose results of PvP matches in the Blue Archive game that were posted onto Discord. The aim is to analyse winning and losing compositions to find the best PvP composition for every situation in the game.

The Discord bot will extract image data from specified Discord channels daily, process this data using Optical Character Recognition (OCR), and store the extracted text in Google BigQuery. Deployed on Google Cloud Platform (GCP) using Docker, the project also incorporates Google Cloud Scheduler to trigger the bot via Google Pub/Sub. This setup was used to experiment with these features despite their overkill for this use case. Google Cloud Functions could also have been used instead of Docker, but the project aimed to explore Docker's capabilities as well, despite it being overkill again.

The OCR process can often be improved with better preprocessing steps to enhance accuracy and reliability. The project details are as follows:

### Trigger Mechanism
- **Google Cloud Scheduler**: Used to schedule tasks and trigger a message to Google Pub/Sub at specified intervals.
- **Google Pub/Sub**: Acts as a messaging service to pass the trigger message to the Docker container.
- **Docker Container**: Deployed on GCP, the container is triggered by messages from Pub/Sub to execute the image processing and data extraction tasks.

### Daily Batch Processing
- The bot scans and processes image attachments from specified Discord channels on a daily basis, ensuring that recent data is always captured and ready for analysis.

### Image Processing
- **Preprocessing**: Images are resized, converted to grayscale, and thresholded to enhance OCR performance. This preprocessing step improves the clarity of the images and makes the text extraction more accurate.
- **OCR Extraction**: The preprocessed images are then analysed using an OCR API to extract text data, which is essential for tracking and analysing game-related metrics.

### Data Storage
- **Google Cloud Storage**: Processed images and their associated metadata are uploaded to Google Cloud Storage.
- **Google BigQuery**: The extracted text data is then integrated into Google BigQuery for structured analysis and reporting.

### Monitoring
- The bot logs and monitors processing jobs, tracking the success or failure of each job. Occasionally, image processing might fail, which is why it's important to track errors.

## Possible Future Experimentations

- **Real-Time Processing**: To enhance the system further, future experiments could involve using Google Pub/Sub to process and extract data from images in real-time as they are posted to Discord.


### Skills: Python, GCP (Google Pub/Sub, Cloud Scheduler, BigQuery), Docker, OCR




---
<br><br> <!-- Adding additional spacing -->


# Total Covid-19 Cases by Country (Updated: 24 March 2021)

I used a public Covid-19 dataset to create a bar chart visualisation of the top 20 countries in total Covid-19 cases at any given date from January 2020 to March 2021.

[![YouTube Video](https://img.youtube.com/vi/ylWDpoVeQwQ/0.jpg)](https://www.youtube.com/watch?v=ylWDpoVeQwQ)

---
<br><br> <!-- Adding additional spacing -->



# Thesis: [Hamiltonian Monte Carlo and No-U-Turn Sampler](https://github.com/junjiechoo24/projects/tree/main/thesis)

![Figure](https://i.imgur.com/TCeTApe.gif)

Hamiltonian Monte Carlo (HMC) is a Markov chain Monte Carlo (MCMC) method that is able to effectively sample high dimensional target distributions by using Hamilton’s equations to design a proposal mechanism that exploits the target geometry. However, HMC’s performance is highly sensitive to tuning parameters. The No-U-Turn
Sampler (NUTS) eliminates the need to hand-tune parameters, whilst showing a competitive performance when compared with a well tuned vanilla HMC. This thesis will provide a background introduction to HMC and describe in detail the NUTS algorithm. Several numerical simulations will illustrate the flexibility of the NUTS algorithm and its practical advantage over vanilla HMC.

### Skills: R, Julia, Monte Carlo

---
<br><br> <!-- Adding additional spacing -->


# [Comparing Neural Networks with K-Nearest Neighbours and Decision Tree Models](https://github.com/junjiechoo24/projects/tree/main/NN-KNN-DT)

![Figure](https://i.imgur.com/xoY10Zc.png)

In this project, we'll explore the effectiveness of deep, feedforward neural networks at classifying images, we'll gradually build a neural network by adding hidden layers and by testing with differents models. We will also compare neural networks with K-NearestNeighbours and Decision Tree models. The features in an image don't have an obvious linear or nonlinear relationship that can be learned with a model like linear or logistic regression. In grayscale, each pixel is just represented as a brightness value ranging from 0 to 256. Scikit-learn contains a number of datasets pre-loaded with the library, within the namespace of sklearn.datasets. The load_digits() function returns a copy of the hand-written digits dataset from UCI. 

Conclusion: Deep learning is effective in image classification because of the models' ability to learn hierarchical representations. At a high level, an effective deep learning model learns intermediate representations at each layer in the model and uses them in the prediction process.

### Skills: Python, Deep Learning, Machine Learning

---
<br><br> <!-- Adding additional spacing -->

# [Covid-19 Figures Report](https://github.com/junjiechoo24/projects/tree/main/covid)

Background: People are sharing Figure 1 on twitter where the figure comes from this report: https://medium.com/
@andreasbackhausab/coronavirus-why-its-so-deadly-in-italy-c4200a15a7bf

![Figure](https://i.imgur.com/JsbZFoK.png)

This figure compares between Italy and South Korea. It catches people’s eyes because this may show that there can be a lot of infected young people in Italy that are missed as they show no or mild symptoms, and they may spread the virus to others unconsciously. As pointed out in the source report, Italy has predominantly been testing people with symptoms of a coronavirus infection, while South Korea has been testing basically everyone since the outbreak had become apparent. Consequently, South Korea has detected more asymptomatic, but positive cases of coronavirus than Italy, in particular among young people.

However, looking at Figure 1 alone is not enough to get the above conclusion as the age structure in the two countries are also different. Even if both two countries can diagnoses every effected case, you would see a higher fraction of elder people diagnosed in Italy than in South Korea since Italy has one of the oldest populations in the world.

If Italy has missed a lot of younger patients who have no or milder symptoms, we can give an estimate of how many people are actually infected in Italy at this moment using logistic regression.

### Skills: R, Generalised Linear Models

---
<br><br> <!-- Adding additional spacing -->


# [Monte Carlo Convergence Diagnostics Project](https://github.com/junjiechoo24/projects)

Markov chain Monte Carlo (MCMC) is one of the most useful approaches to scientific computing because of its flexible construction, ease of use, and generality. Two critical questions that MCMC practitioners need to address are where to start and when to stop the simulation. Although a great amount of research has gone into establishing convergence criteria and stopping rules with sound theoretical foundation, in practice, MCMC users often decide convergence by applying empirical diagnostic tools. This review article discusses the most widely used MCMC convergence diagnostic tools.

### Skills: Monte Carlo algorithms

---
<br><br> <!-- Adding additional spacing -->

# [Vanilla and Generalised Elliptical Slice Sampling](https://github.com/junjiechoo24/projects)

Many probabilistic models introduce strong dependencies between variables using a latent multivariate Gaussian distribution or a Gaussian process. We present a new Markov chain Monte Carlo algorithm for performing inference in models with multivariate Gaussian priors. Its key properties are:

1. it has simple, generic code applicable to many models,
2. it has no free parameters,
3. it works well for a variety of Gaussian process based models.

These properties make our method ideal for use while model building, removing the need to spend time deriving and tuning updates for more complex algorithms.

### Skills: R, Statistical modelling algorithms

---
<br><br> <!-- Adding additional spacing -->

# [Regression and Permutation Test](https://github.com/junjiechoo24/bikeshare)

The data set is the Capital Bikeshare data set, from https://www.capitalbikeshare.com/system-data. This data comes from Washington D.C.’s bikeshare program, which records every individual ride taken. Each ride is tagged with its start and end time, start and end station (there are hundreds of locations where bikes can be rented across the city), as well as whether the rider has bought a one-time rental or is a member of the bikeshare program.

A script named getdata_bikeshare.R is used to download and clean the data so that it’s ready for R and organized in a simple format.

The following question was studied: Can any routes be detected (i.e., a particular combination of start & end station) where the average time it takes to travel the route, changes over the course of the time period? For example, if a bike lane is added to a major road, this may reduce the travel time for that particular route.

Methodology:

Cluster the data by route, and run a linear model on confounders only, i.e. Days since Jan1 2010 is not part of the model.
Within each cluster, use the residuals for permutation test, but group the residuals by day and permute the groups instead of the individual residuals, in order to account for the dependency of data belonging to the same day.

### Skills: R, Data analysis

---
<br><br> <!-- Adding additional spacing -->

# [Real Data Analysis Critique](https://github.com/junjiechoo24/projects)

The paper critiqued was “Lung cancer incidence decreases with elevation: evidence for oxygen as an inhaled carcinogen”, Simeonov & Himmelstein, PeerJ 2015 https://peerj.com/articles/705/

The statistical analyses performed in the paper was critiqued from the point of view of multiple testing and replicability. The validity of the conclusions was also assessed from a statistician’s point of view

Some ideas are: thinking about possible confounding variables, whether the data collected is representative of the claim being made, etc.

### Skills: Data analysis




