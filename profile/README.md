# 🏃‍♀️ Attack on Tor: Website Fingerprinting

This project is a machine learning project that achieves predictive accuracy for website access through Internet website access fingerprinting.

Under the guidance of Professor Oh Se-eun, we carried out this project during the fall semester of the 23rd school year.

## 1️⃣ **Closed-world Scenario**

In this scenario, it is assumed that the user only visits websites that are marked as "monitored". 

The objective of this scenario is to correctly classify 95 monitored websites.

## 2️⃣ **Open-world Scenario**

In this scenario, it is assumed that the user can visit any website, including "unmonitored" ones that we are not interested in. In this case, we perform two types of classification: binary classification and multi-class classification.

### **Binary Classification**:

The goal of this scenario is to determine whether a given web traffic trace corresponds to a monitored website. To train the model, we assign a label of '-1' to all instances of unmonitored websites.

### **Multi-Class Classification**:

This involves classification among web traffic traces tagged with 95 unique labels corresponding to monitored websites, plus additional unmonitored websites.

This project seeks to explore and illustrate these different scenarios and classification types within the context of web traffic analysis.

### Prerequisites

What things you need to install the software and how to install them

## Built With
* <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"> - The programming language used
* <img src="https://img.shields.io/badge/googlecolab-F9AB00?style=for-the-badge&logo=GoogleColab&logoColor=white"> - The environment used

  
## Authors
* **We are Running Machine**

* **A Jeong Sung** - *The * - [YourGithubUsername](https://github.com/YourGithubUsername)
* **1970094 Hong Saeyeon**  - [GitHub](https://github.com/YourGithubUsername)
* **2071007 Kim Myeongji** - [GitHub](https://github.com/YourGithubUsername)
* **Seohyun Kim**  - [GitHub](https://github.com/YourGithubUsername)
* **Eunseong Park** *I'm very appreciate that we work together* - [GitHub](https://github.com/YourGithubUsername)

## License

This project is licensed under the MIT License 

