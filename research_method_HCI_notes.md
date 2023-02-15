# Notes for Research Method in Human Computer Interaction



## 1. Experimental Research

----

### 1.1 Relationships between three types of research

---

Typical research projects include a combination of two or even three kinds of investigation.

>![table](./Pictures%20and%20Graphs/Relatationship_between_different_researchs.jpg "Relationship")

>
* __Descriptive__: Descriptive investigations are often the first step of a research program, enabling researchers to identify interesting phenomena or events that establish the cornerstone of the research and identify future research directions.
  
* __Relational__: Relational investigations enable researchers or practitioners to discover connections between multiple events or variables.
  
* __Experimental__: Experimental research provides the opportunity to explore the fundamental causal relations

>


### 1.2 TYPICAL DEPENDENT VARIABLES IN HCI RESEARCH

---

Dependent variables frequently measured can be categorized into five groups: __*efficiency, accuracy, subjective satisfaction, ease of learning and retention rate, and physical or cognitive demand*__.


>
* __Efficiency__: Efficiency describes how fast a task can be completed.
  
* __Accuracy__: Accuracy describes the states in which the system or the user makes errors.
  
* __Subjective satisfaction__: Subjective satisfaction describes the user's perceived satisfaction with the interaction experience. The data is normally collected using __*Likert scale ratings*__ (e.g., numeric scales from 1 to 5) through questionnaires.
  
* __Ease of Learning__: Ease of learning and retention rate describe how quickly and how easily an individual can learn to use a new application or complete a new task and how long they retain the learned skills

* __Physical or cognitive demand__: an application or a task exerts on an individual or how long an individual can interact with an application without significant fatigue.
>


## 2. Experiment Design

----
### 2.1 Wizard-of-Oz approach

---

The Wizard-of-Oz approach allows us to test *ideal applications* that do not exist in the real world. This approach is not without its limitations. Humans also make errors. It is very likely that the human “wizard” would make errors when listening to the dictation or when typing the words.


### 2.2 Between-group design and within-group design

---

> 
__Between-group design__ is also called “between-subject design.” between-group design has __notable disadvantages__. In a between-group experiment, we are comparing the performance of one group of participants against the performance of another group of participants. The results are subject to substantial impacts from __individual differences__. Recruiting __the number of participants__ needed for a between-group experiment can be a very challenging task. 

>![fig](./Pictures%20and%20Graphs/between-group_design.jpg "between-group design")


A __within-group design__ (also called “within-subject design”) requires each participant to be exposed to multiple experimental conditions. The biggest problem with a within-group design is __*the possible impact of learning effects*__. For instance, suppose we are conducting a within-group experiment that evaluates two types of ATM: one with a button interface and one with a touch-screen interface. The task is to withdraw money from an existing account. If the participant first completes the task using the ATM with the button interface, the participant gains some experience with the ATM interface and its functions. Therefore, the participant may perform better when subsequently completing the same tasks using the ATM with the touch-screen interface. Another potential problem with within-group designs is __*fatigue*__

>![fig](./Pictures%20and%20Graphs/within-group_design.jpg "between-group design")


>![fig](./Pictures%20and%20Graphs/Comparison_between_two_design.jpg "Comparison")

### 2.3 How to choose appropriate design

---

Many times the decision is **quite hard** to make since the advantages and disadvantages of the between-group design and within-group design are exactly opposite to each other.

The size of the individual differences is very hard to estimate. However, it is empirically confirmed that individual differences are smaller when the tasks are *__simple__* and involve *__limited cognitive process__*. In contrast, individual differences are larger when the task is complicated or involves significant cognitive functions.

Difficulty in finding and recruiting qualified participants is a problem frequently faced by many HCI researchers.


Having decided to adopt a **within-group design**, you need to consider how to control the negative impact of learning effects, fatigue, and other potential problems associated with a within-group design.


providing sufficient training time for users to get acquainted with the system or the task greatly reduces the learning effect during the actual task sessions. Of course, __training cannot completely eliminate the learning effect__. It only reduces its impact. This approach, combined with the counterbalancing of task conditions, is widely adopted in HCI studies to control the impact of learning.


To address the problem of *fatigue* caused by multiple experimental tasks, we need to design experiment tasks frugally, **reducing the required number of tasks** and **shortening the experiment time whenever possible**.



### 2.4 Investigate more than one independent variable

---

#### 2.4.1 Factorial design

***Factorial designs*** are widely adopted when an experiment investigates **more than one** independent variable or factor. It allows us to simultaneously investigate the impact of **all independent variables** as well as the ***interaction effects*** between multiple variables

>![fig](./Pictures%20and%20Graphs/factorial_design.jpg "Factorial design")


#### 2.4.2 Split-plot design

In a factorial study, we can also choose a split-plot design. A ***split-plot design*** has **<u>both between-group components and within-group components</u>**. That is, one or more independent variables are investigated through a between-group approach and the other variables are investigated through a within-group approach.


>![fig](./Pictures%20and%20Graphs/split_plot_design.jpg "split-plot design")


This gives us a typical split-plot design that involves both a between-group component (age analysis is based on the columns) and a within-group component (GPS use is analyzed by comparing condition 1 with condition 4, condition 2 with condition 5, and condition 3 with condition 6).


#### 2.4.3 Interaction effects


One advantage of a factorial design is that it allows us to study the interaction effects between two or more independent variables. It is critical to **study interaction effects** in HCI studies since performance may be affected by multiple factors jointly. **Interaction effects may have important implications for design.**


>![fig](./Pictures%20and%20Graphs/Interaction_effect.jpg "Interaction effect")


### 2.5 Reliability of experiment results

---

**Random errors** are also called “chance errors” or “noise”. There is no way to eliminate or control random errors but we can reduce the impact of random errors by enlarging the observed sample size.

**Systematic errors**, also called “**biases**”. While random errors cause variations in observed values in both d tions around the actual value, systematic errors always push the observed values in the same direction.

A **pilot study** is not a luxury that we conduct only when we have plenty of time or money to spend. On the contrary, years of experience tells us that pilot studies are critical for all HCI experiments to identify potential biases. A pilot study is the only chance you have to **fix your mistakes** before you run the main study.


**Environmental factors** can be categorized into two groups: <u>**physical environmental factors**</u> and <u>**social environmental factors**</u>. Examples of physical environmental factors include noise, temperature, lighting, vibration, and humidity. Examples of social environmental factors include the number of people in the surrounding environment and the relationship between those people and the participant.


>![fig](./Pictures%20and%20Graphs/Lifecycle_of_HCI_research.jpg "life cycle of HCI research")


We should try to avoid or control biases through:
1. **accurate and appropriate measurement devices** and scales; 
2. clearly defined and d**etailed experimental procedures**; 
3. **carefully recruited participants**; 
4. well-trained, professional, and unbiased **experimenters**; 
5. well-controlled **environments**.


## 3. Statistical analysis

### 3.1 Preparing data

---

* Cleaning up data
* Coding data
* Organizing  data


### 3.2 Descriptive  statistical

---

#### 3.2.1 Central tendency


Various measures can be used to describe the central tendency of a data set, including **the mean**, **the median**, and **the mode**


#### 3.2.2 Spread

Measures in this group include **range**, **variances**, and **standard deviations**.


#### 3.2.3 Comparing Means

Due to variances in the data, you **should not directly** compare the means of the multiple conditions and claim that a difference exists as long as the means are different.

Various significance tests are available to compare the means of multiple groups. Commonly used tests include **<u>t tests</u>** and the **<u>ANOVA</u>**.

* ***T-test***: A t test is a simplified ANOVA involving **only two groups or conditions**. 
* ***ANOVA***: When a study involves **more than two conditions**, an ANOVA test has to be used.

>![fig](./Pictures%20and%20Graphs/T_test_and_ANOVA.jpg "significance tests")


### 3.3 T-test
---

T-test has several types:

- **Independent-samples T-test**
- **Paried-samples T-test**

When the two groups being compared are **presumably unrelated**, an **<u>independent-samples t test</u>** can be used. When the two means are contributed by the **same group**, a **<u>paired-samples t test</u>** can be considered.

The t tests return a value, ***t***, with larger t values suggesting higher probability of the null hypothesis being false. In other words, <u>the higher the t value, the more likely the two means are different</u>.

The returned t value is **2.169**, which is **higher than the t value** for <u>the specific degree of freedom (df = 15) at the 95% confidence interval (t = 2.131)</u>. For instance: An independent-samples t test suggests that there is significant difference in the task completion time between the group who used the standard word-processing software and the group who used word-processing software with word prediction functions **(t(15) = 2.169, p < 0.05)**.


>![fig](./Pictures%20and%20Graphs/Independent_t_test.jpg "significance tests")



### 3.4 ANOVA
---

ANOVA has several types:

- **One-way ANOVA**
  - **One-way between-group ANOVA**
  - **One-way within-group ANOVA**, also **Repeated measures ANOVA**
- **Two-way ANOVA**, also **Factorial ANOVA**

>![fig](./Pictures%20and%20Graphs/Repeated_measures_ANOVA.jpg "repeated measures")

>![fig](./Pictures%20and%20Graphs/results_of_Repeated_ANOVA.jpg "result 1")

    The returned F value with degree of freedom (2, 14) is 2.925. It is below the 95% confidence interval, suggesting that there is no significant difference between the three text entry methods.



>![fig](./Pictures%20and%20Graphs/Two-way_repeated_measures.jpg "two-way repeated measures")


>![fig](./Pictures%20and%20Graphs/results_of_two-way_repeated_measures.jpg "result 2")

    The task type has a significant impact on the time spent to c plete the task (F(1, 7) = 14.217, p < 0.01). There is no significant difference among the three text entry methods (F(2, 14) = 2.923, n.s.). The interaction effect between the two independent variables is not significant either (F(2, 14) = 0.759, n.s.).


#### 3.4.1 One-way(one-factor) test Explaination

>![fig](./Pictures%20and%20Graphs/one-way_explaination.jpg "Explaination")


#### 3.4.2 Two-way(Factorial tet) test Explaination

>![fig](./Pictures%20and%20Graphs/Two-way_explaination.jpg "Explaination")



#### 3.4.3 One-way repeated measures test Explaination

>![fig](./Pictures%20and%20Graphs/One-way_repeated_measures.jpg "Explaination")



#### 3.4.4 Python and ANOVA

ANOVA: <https://www.reneshbedre.com/blog/anova.html>

Repeated-measure-anova: <https://www.reneshbedre.com/blog/repeated-measure-anova.html>



### 3.5 Assumption of T-test and ANOVA
---

Before running a t test or an F test, it is important to examine whether your data meet the assumptions of the two tests.

* First, the errors of all data points should be independent of each other. If they are not independent of each other, the result of the test can be misleading.
* Second, the errors in the data need to be identically distributed.
* Third, the errors in the data should be normally distributed.



### 3.6 Identifying relationships
---

#### 3.6.1 Pearson correlation coeffcient test 

One of the most common objectives for HCI-related studies is to **identify relationships** between various factors. The most widely used statistical method for testing correlation is **<u>the Pearson's product moment correlation coefficient test</u>**.

The value of Pearson's r ranges from **−1.00 to 1.00**. When the Pearson's r value between two variables is −1.00, it suggests a perfect negative linear relationship between the two variables. When the Pearson's r value between two variables is 1.00, it suggests a perfect positive linear relationship between the two variables. When the Pearson's r value is 0, it means that there is no linear relationship between the two variables.

In practice, the Pearson's r.pow(2) is reported more often than the Pearson's r. The r.pow(2) represents the proportion of the variance shared by the two variables. Suppose we have two variables X and Y, the **<u>r.pow(2) represents the percentage of variance in variable X that can be explained by variable Y</u>**. 

***The most important thing to keep in mind about correlation is that it does not imply a causal relationship.***



#### 3.6.2 Regression

Unlike correlation analysis, which allows the study of **only two variables**, ***regression analysis*** allows you to **investigate the relationship among one dependent variable and a number of independent variables**.

In HCI-related studies, ***regression analysis*** is used for two main purposes: **<u>model construction and prediction</u>**. In cases of model construction, we are interested in identifying the quantitative relationship between one dependent variable and a number of independent variables. In cases of prediction, we are interested in using a number of known factors, also called “predictor variables,” to **predict the value of the dependent variable**, also called the “criterion variable”

>![fig](./Pictures%20and%20Graphs/Regression_analysis.jpg "Regression analysis")


    In this regression analysis, the dependent variable is the task completion time. The independent variables are age, computer experience (as represented by the number of years using computers), target size, and the distance between the current cursor location and the target.


***If you are interested in the impact that each independent variable has on task completion time, the hierarchical regression procedure can be adopted.*** Suppose **<u>target size and navigation distance are the most important factors that you want to examine</u>**; you can enter target size in the first block for independent variables and navigation distance, age, and computer experience into the subsequent blocks.


### 3.7 Nonparametric statistical tests
---

Although nonparametric tests are also called <u>"assumption-free" tests</u>, it should be noted that they are not actually free of assumptions. Nonparametric analysis sacrifices the power to use all available i tion to reject a false null hypothesis in exchange for less strict assumptions about the data.


#### 3.7.1 Chi-Ssquared test

***The Chi-squared test is probably the most popular significance test used to analyze frequency counts***

The degree of freedom of a Chi-squared test is calculated by the following equation:

Degree of freedom = (Number of rows - 1) - 1 (Number of columns)


>![fig](./Pictures%20and%20Graphs/Chi-squared_frequency_counts.jpg "Chi-squared test")



## 4. Surveys


***Surveys*** are one of the **most commonly used** research methods, across all fields of research, not just human-computer interaction (HCI). Surveys are also one of the **<u>most maligned</u>** methods. Surveys can be s tured, well-tested, robust, and result in data with a high level of validity. **However, surveys can be poorly done, resulting in data of questionable validity**.

The **<u>strength</u>** of the survey is the ability to get a large number of responses quickly from a population of users that is geographically dispersed. 

One of the reasons why surveys may <u>be maligned</u> is that they are often used **not because they are the most appropriate method but because they are the easiest method**.

Survey research may be the **most appropriate** methodology for <u>**measuring attitudes, awareness, intent, feedback about user experiences, characteristics of users, and over-time comparisons**</u>.

A combination of <u>computer-collected data</u> and <u>a user survey</u> might **make the most sense**.

