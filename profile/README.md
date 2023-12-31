<img src="https://capsule-render.vercel.app/api?type=waving&color=153C19&height=400&section=header&text=Running-Machine&fontSize=90" />

# 🏃‍♀️ Attack on Tor: Website Fingerprinting

This project is a machine learning project that achieves predictive accuracy for website access through Internet website access fingerprinting.

Under the guidance of Professor Se-eun Oh, we carried out this project during the fall semester of the 23rd school year.

## 1️⃣  **Closed-world Scenario**

In this scenario, it is assumed that the user only visits websites that are marked as "monitored". 

The objective of this scenario is to correctly classify 95 monitored websites.

### Problem ➊ **Multi-Class Classification with Monitored Data**

We developed a model that can predict 95 labels above a certain level by learning the monitored data provided by the professor from Google Colab to a machine learning algorithm.

The below bar graph shows the comparison of our final model and other models ([Click](https://github.com/Running-Machine-ML23-2/problem_1/)):

![image (1)](https://github.com/Running-Machine-ML23-2/.github/assets/96706954/e52c0d8d-f44a-4d63-9d97-0db54f268621)


## 2️⃣  **Open-world Scenario**

In this scenario, it is assumed that the user can visit any website, including "unmonitored" ones that we are not interested in. 

In this case, we perform two types of classification: binary classification and multi-class classification.

### Problem ➋  **Binary Classification**

The goal of this scenario is to determine whether a given web traffic trace corresponds to a monitored website. 

To train the model, we assign a label of '-1' to all instances of unmonitored websites.

Here is the Confusion Matrix of our final model([Click](https://github.com/Running-Machine-ML23-2/problem_2/blob/main/Adaboost.ipynb)):

![image](https://github.com/Running-Machine-ML23-2/.github/assets/96706954/f915c953-1de3-44da-aa9e-6c032dabe3b8)


### Problem ➌  **Multi-Class Classification including Unmonitored Data**

This involves classification among web traffic traces tagged with 95 unique labels corresponding to monitored websites, plus additional unmonitored websites.

This project seeks to explore and illustrate these different scenarios and classification types within the context of web traffic analysis.

The below bar graph shows the comparison of our final model and other models ([Click](https://github.com/Running-Machine-ML23-2/problem_3/)):

![image (2)](https://github.com/Running-Machine-ML23-2/.github/assets/96706954/1b40bdea-ad2c-4b32-be92-270b7ffca46a)


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

# 🏃‍♀️ How to run

It is possible to preprocess and import data using the provided ipynb code. 

Data was provided for the project, and individual contact and consultation from institutions, schools, etc. is required if data access rights are desired.
* Problem 1
```
├── Adaboost.ipynb
├── Final_Random_Forest.ipynb
├── KNN.ipynb
├── Matrix.ipynb
└── SVM.ipynb
```
* Problem 2
```
├── Adaboost.ipynb
├── Binary_Matrix.ipynb
└── SVM.ipynb
```
* Problem 3
```
├── Adaboost.ipynb
├── Final_Radom_Forest.ipynb
├── KNN.ipynb
├── Matrix.ipynb
└── SVM.ipynb
```
* Extra Credit
```
├── Extra_credit.ipynb
├── Extra_credit_split.ipynb
└── Extra_credit_split_4.ipynb
```

# 🏃‍♀️ Built With

* <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"> - The programming language used
* <img src="https://img.shields.io/badge/googlecolab-F9AB00?style=for-the-badge&logo=GoogleColab&logoColor=white"> - The environment used

  
# 🏃‍♀️ Authors

<img src="https://github.com/Running-Machine-ML23-2/.github/assets/96706954/ad9a1759-429e-4d43-84b3-faf977f6e2c9" width="400" height="100"/>


* **We are Running Machine**

* **Sung Ajeong** - [Gmail](azng1217@ewhain.net)
* **Hong Saeyeon**  - [Gmail](sugarsugar@ewhain.net)
* **Kim Myeongji** - [Gmail](kimmyeongji3@gmail.com)
* **Kim Seohyun**  - [Gmail](syrup91@ewhain.net)
* **Park Eunseong** *I'm very appreciate that we work together* - [Gmail](eunseong06070@gmail.com)

Our team name is "Running Machine." This name encapsulates our mission and vision as a group dedicated to the pursuit of advanced machine learning projects. 

The name "Running Machine" has a dual meaning. On one hand, it represents our commitment to machine learning - a rapidly evolving field that is akin to a machine that never stops 'running'. On the other hand, it also signifies our team's continuous drive to learn, grow, and 'run' towards our goal of achieving predictive accuracy for website access through internet website access fingerprinting.

Our vision is to innovate and push the boundaries of what is possible with machine learning, particularly in the realm of internet security. We aim to create systems that can accurately predict website access patterns, thereby enhancing the safety and efficiency of internet use. 

Our mission, in line with our name, is to keep 'running', to keep innovating. We are not just a machine that's running. We are a machine that's evolving, learning, and improving. We are the Running Machine. 

## License

This project is licensed under the MIT License 

