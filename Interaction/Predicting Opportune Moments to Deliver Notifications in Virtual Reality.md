# Paper Link
---

TIME: 2022/4 CHI

[Predicting Opportune Moments to Deliver Notifications in Virtual Reality](https://doi.org/10.1145/3491102.3517529)


# Problem
---

## purpose

Current commercial VR devices provide visual, audio, and even haptic feedback, providing an immersive experience for users.

1. The feeling of presence and immersion in VR might also lead to disconnection from the real world.
2. Presenting notifications in VR allows users to stay informed about real-world events without removing their headsets, preserving the continuity and immersion of the VR experience.
3. Only a few attempts to investigate the sending of real-life notifications in VR have been made



## Main Contribution

- present the first research attempt aimed at exploring the **feasibility** of predicting **opportune moments** for sending notifications in VRs.
- focus on sensor features available on VR devices, including head-mounted displays (**HMD**), **controllers** and **eye-trackers**, for prediction, reasons:
  - they offer easily accessible information open to developers;
  - provide rich information about users


The primary objective of this paper is to examine the performance of prediction using only sensor data for prediction, as well as performance after including the additional features (e.g., engagement levels and activity categories).


research questions are as follows:

- RQ1: ***How well can sensors alone predict opportune moments for sending notifications in VR?***, sub-question: ***Which sensor type contributes the most to the prediction?***
- RQ2: ***How much improvement can information about activity condition and user engagement make, respectively, in prediction performance?***
- RQ3: ***Does a personalized model outperform a general model for predicting opportune moments in VR?***



# Core Ideas
---

1. recruited 20 participants to participate in data collection;
2. The participants underwent a total of **six VR sessions** composed of **three different VR applications**, during which we collected **sensor information**;
3. used a **cued retrospective method** to collect **engagement labels** on VR sessions they had just experienced. Using these data, we built **deep learning models** for the prediction tasks.

## Experiment

- **Each session** was designed to be **five minutes** long, during which the participants saw four visual notifications. Notification delivery was designed to create stimuli to elicit participants’ feelings when seeing notifications in these VR applications.
- Only use the modality of **visual notifications** in data collection, as this is **most common** in today’s consumer VR platforms.
- Each of the four notifications was randomly sent **within a 25-second time window**, and **a 40-second interval** was placed between any two such time windows.

![fig](../Pictures%20and%20Graphs/Visual_notification.jpg "Visual notification")


They deemed it important to **collect diverse VR experiences** to make our prediction model **more generalizable** to different VR applications. This paper focuses on two dimensions of interruptibility: (1) body movement: high cognitive load; (2) visual attention: high degree of visual attention. Three scenarios are as follows:

- 360 videos: different video content might attract different levels of visual attention;
- VR Fitness: to collect data that featured **diverse amounts of body movement** with relatively **low levels of visual attention**;
- Rhythm game: to collect data that were diverse in **both visual attention and body movement**.

![fig](../Pictures%20and%20Graphs/Three_types_VR_activities.jpg "VR activities")




## Data Collection

- Participants were asked to **annotate opportune and inopportune moments** with the assistance of video replays that reminded them of their reactions during VR interaction.
- HTC Vive Pro Eye, which consists of two controllers and an HMD equipped with an eye tracker,
- During formal data collection, the participants experienced the **three VR activities in a random order**, and **each activity was split into two sessions**, with each session lasting approximately **five minutes** long.
- They recorded the sensor data from the VR device at **60 Hz** and **made note of the predefined current activity category** in the programs during each session.
- As sensor data were obtained in real-time, to predict opportune moments in real-time, we used the sensor data **five seconds** prior to predicting a perceived opportune moment.


![fig](../Pictures%20and%20Graphs/Features_of_data_collected.jpg "Features of data")


![fig](../Pictures%20and%20Graphs/Features_of_data_collected.jpg "slide windows")

For example, sensor data from the 600th frame to the 900th frame were used to predict whether the moment at the 901st frame was opportune for receiving notification.


This sampling method produced a dataset containing **33,219 total samples**, consisting of **13,236 positive samples** (suitable) and **19,983 negative samples** (not suitable).




## Method

sensor data (time-series data) were first fed into a time-series NN-based model to output a 64-dimensional feature vector. Additional contextual information (activity category and engagement) were categorical data, and they thus encoded them as a one-hot vector and fed them into a fully connected layer to output another 64-dimensional feature vector.

![fig](../Pictures%20and%20Graphs/NN_model_structure.jpg "Model Structure")



***Personalized models*** for each participant:

- split the data into a training and a test dataset according to time intervals to avoid overlapping between the two sets. 
- For example, for **300 seconds of VR activity recording data**, we took **0 to 30 seconds as test data** and the remaining data as training data.
- This method provides a metric for ***how personalized models performed on similar but unseen data***.


***general model***, leave-one-participant-out cross-validation:

- one participant’s data were used as test data, and the data from the remaining 19 participants were used as the training data.
- to gather **further insights** on **the generalizability of the features** across individual participants




# Result
---

1. **Personalized models outperformed general models for all combinations of sensor types**. Individual variances in sensor data patterns among the participants might be so large that the information learned from a group of individual participants was not sufficient to be predictive for a new user. **Combining more types of sensor data achieved better AUROC for both the personalized model and the general mode**.
   - ![fig](../Pictures%20and%20Graphs/Comparison_bwt_Personalize_general.jpg "Two models")
   - ![fig](../Pictures%20and%20Graphs/Personalize_general_model_performance.jpg "Two models")
2. The figure clearly shows that removing each of them resulted in differing performance drops in each activity, suggesting that each sensor contributed differently to prediction in the different types of VR activity.
   - ![fig](../Pictures%20and%20Graphs/Feature_importance.jpg "Feature importance")

3. Most participants supported these observations in the end-of-study interviews, mentioning that whether or not notifications were timed well depended on the content of the activity they were engaged in at the time.
   - ![fig](../Pictures%20and%20Graphs/Activity_engagement_and_opportuneness.jpg "Activity, engagement, and opportuneness")



# Conclusion

- **No single sensor in the VR devices was superior to the others, and each sensor was important in different types of VR activities**.
- **By including the activity conditions and summarized engagement information, the prediction achieved an AUROC of up to 0.93 for the personalized model and 0.81 for the general model**.
- **These results not only demonstrate the feasibility of identifying opportune moments for notifications in VR but also indicates that such predictions could achieve great performance**.


# Comment
---

- 这篇文章，在设计实验的时候，每一个细节都考虑得很清楚，都能在之前研究中找到依据。研究问题的设计也很符合文章的主题，并且讨论很全面，比如：在讨论genral model和personalized model的时候，分别进行实验，不仅验证了模型能力的强弱，而且讨论了两种思路的优缺点和未来能够应用的落脚点。

- 这篇文章的label方式很合理，在 labeling interruptibility 的时候，文章中是让试验者进行范围labeling， 将一段连续的时间，都进行标签化，有利于时间序列模型训练和进行结果修正。



# What can be used
---

- general model 和 personalized model的研究问题可以迁移到我们的项目中
- 关于feature importance的讨论也可以一定程度迁移到我们的项目中
- 关于如何设计实验或者如何选定实验过程的类型也可以参考这篇文章提供的思维方式进行思考
