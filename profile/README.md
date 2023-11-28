# 🏃‍♀️ Attack on Tor: Website Fingerprinting

This project is a machine learning project that achieves predictive accuracy for website access through Internet website access fingerprinting.

Under the guidance of Professor Se-eun Oh, we carried out this project during the fall semester of the 23rd school year.

## 1️⃣  **Closed-world Scenario**

In this scenario, it is assumed that the user only visits websites that are marked as "monitored". 

The objective of this scenario is to correctly classify 95 monitored websites.

### Problem ➊ **Multi-Class Classification with Monitored Data**

We developed a model that can predict 95 labels above a certain level by learning the monitored data provided by the professor from Google Colab to a machine learning algorithm.

## 2️⃣  **Open-world Scenario**

In this scenario, it is assumed that the user can visit any website, including "unmonitored" ones that we are not interested in. 

In this case, we perform two types of classification: binary classification and multi-class classification.

### Problem ➋  **Binary Classification**

The goal of this scenario is to determine whether a given web traffic trace corresponds to a monitored website. 

To train the model, we assign a label of '-1' to all instances of unmonitored websites.

### Problem ➌  **Multi-Class Classification including Unmonitored Data**

This involves classification among web traffic traces tagged with 95 unique labels corresponding to monitored websites, plus additional unmonitored websites.

This project seeks to explore and illustrate these different scenarios and classification types within the context of web traffic analysis.

# 🏃‍♀️ **Feature Extraction**

Several method to achieve the above include the following methods.

* **Continuous Feature**

Continuous features are provided with timestamps and packet size information in an array. 

We could use this itself as a feature, and obtain a new feature by separately extracting the cumulative Summated value of the packet and the Burst data information.

On the trend, it appears to be a feature that performs better in the experiment than the category feature we experienced a priori.

We find that the front part of one array of packet size information has a significant influence. 

In addition, the effect of improving performance and reducing learning time could be obtained through appropriate cuts of feature information.

Also, data with different lengths were padded to a certain value (0) to build data that is easy to learn.

* **Categorical Feature**

Categorical features are features that we can obtain by fetching data. We were able to extract a total of five types of features.

First of all, we completed features to obtain the number of incoming and outgoing packets and its standard deviation, respectively, and referred to the information on the number of packets.

As experimentally proven features of the above, it is generally known to be effective in network fingerprinting.

# 🏃‍♀️ Built With
* <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"> - The programming language used
* <img src="https://img.shields.io/badge/googlecolab-F9AB00?style=for-the-badge&logo=GoogleColab&logoColor=white"> - The environment used

  
# 🏃‍♀️ Authors
* **We are Running Machine**

* **A Jeong Sung** - *The * - [YourGithubUsername](https://github.com/YourGithubUsername)
* **1970094 Hong Saeyeon**  - [GitHub](https://github.com/YourGithubUsername)
* **2071007 Kim Myeongji** - [GitHub](https://github.com/YourGithubUsername)
* **Seohyun Kim**  - [GitHub](https://github.com/YourGithubUsername)
* **Eunseong Park** *I'm very appreciate that we work together* - [GitHub](https://github.com/YourGithubUsername)

## License

This project is licensed under the MIT License 

