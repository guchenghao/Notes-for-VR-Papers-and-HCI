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

