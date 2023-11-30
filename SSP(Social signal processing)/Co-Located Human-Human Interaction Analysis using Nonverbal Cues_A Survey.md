# Paper Link

---
TIME: 2023/11 ACM Computing Surveys

[Co-Located Human-Human Interaction Analysis using Nonverbal Cues: A Survey](https://doi.org/10.1145/3626516)

# A survey of SSP

## HAR (Human activity recoginition)

A **major limitation** is that HAR approaches do not consider the social context in which humans perform actions and therefore they do not understand what such actions mean. For example, a HAR approach canunderstand that a person touches his/her own face by reasoning on the spatial relation between hands, face, andbody parts.

## Concepts of SSP

SSP research integrates **social psychology** concepts into **Artificial Intelligence** (AI) and focuses on automatic detection, interpretation, and synthesis of social signals, nonverbal behavioral cues (e.g.,gestures, eye gaze, body posture, vocal characteristics, interpersonal distances, facial expressions) capable to conveysocially-relevant information.

![Inference of varios social and psychological phenomena](../Pictures%20and%20Graphs/the%20inference%20of%20various%20social%20and%20psychological%20phenomena.png)

## Non-verbal cues

### Vocal behavior

Such behavior corresponds to everything in speech except words, including the use of vocalizations (e.g., fillers, laughter, and sobbing), pauses, and turn-taking. **Speaking activity** and **prosody** are thetwo aspects of vocal behavior that are most commonly used in the literature.

### Speaking activity

The most common form of speaking activity detection is referred to as **speaker diarization**, which is the automatic segmentation of speech recordings intoturns(i.e., time intervals) in which only one of thepersons involved in an interaction is speaking.

### Prosody

Such cues account for the way people talk and in most cases correspond to how loud people speak (is captured through the energy of the speech signal) and their intonation (is captured through the fundamentalfrequency of the speech signal).

#### Body Activity (Openpose)

The expression body activity refers to postures, movements of the upper body, arms, hands,and gestures.

#### Eye gaze and Visual Focus of Attention(VFOA)

* The **Visual Focus of Attention** (VFOA) can be defined as the point in space a person is looking at and it can be detected by estimating either gaze direction or head pose (someworks, for example, use head and body pose as an indicator of attention);

* OpenFace

* Once the VFOA of all people participating in an interaction is known, it is possible to calculate several features that were shown to account for different social and psychological phenomena.

#### Facial Expressions

* Facial expressions were specifically included in the analysis of dyads (e.g., interviews)or meetings.

* Their usage was relatively **less than** speaking activity, prosody, eye gaze/VFOA, and body activity such that the number of studies covering them is 7 whereas the number of works analyzing the **speaking activity, prosody, eye gaze/VFOA, and body activity** is 53, 47, 32 and 49, respectively.

#### Proxemics

* This is the domain studying **the social meaning of interpersonal distances** especially when themovement of people is not constrained.

* ***Free-standing conversations*** (conv.) are the settings in which proxemics play the most important role and individual distances were shown to account forthe detection of multiple social phenomena including *social roles, leadership, engagement and personality traits*.

#### Physical Appearance

This includes height, body shape, skin/hair color, clothes, and make-up of a person.

### Sensors

For what concerns **vocal behavior**, the most frequent sensors are **microphones** of different types:

* close-talk (CTM)
* headset (HSM)
* tabletop (TTM)
* lapel (LAM)
* microphone arrays (ARM)
* omnidirectional (ODM)
* four-channel cardioid (FCM)
* other distantly placed microphones such as single-channel far-field (FFM)

In the case of ***body activity, eye gaze, VFOA, facial expressions, proximity, and the physical appearance of the participants***, the main sensors are **cameras**:

* close-up (CUC)
* Red Green Blue Depth (RGBD)
* web (WC)
* 360 degrees (C360)
* frame-synchronized (FSC)
* digital movie (DMC)
* top-view (TVC)
* wearable(WCM)
* narrative (NC)
* pan and tilt zoom (PTZ)
* far-field (FFC)
* a combination of them

Except microphones and cameras, other sensing technologies have also attracted researchers:

* Smartphone: comprehensive
* Accelerometers(ACC): the analysis of small group round-table meetings as well as the analysis of mingling scenarios
* Sociometer badges(SB)
* Head-mounted wearables: capture the speech, body movement and gaze
* Respiration sensors
* Biological sensors: nonverbal behaviors, EEG

### Computational Methods

***Machine learning, deep learning supervised and unsupervised approaches***

![SSP_papers1](<../Pictures and Graphs/Papers_with_SSP_1.png>)
![SSP_papers2](<../Pictures and Graphs/papers_with_SSP_2.png>)

## Reviews: Methodologies of SSP

### Social Traits

The social traits addressed by the computing studies include **competence**, **likeability**, **hirability**, **personality**, **dominance**, and **leadership**.

#### leadership and styles

A leader is a person who has authority and power over a group of peoplr and can exert his/her dominance, influence and control over them;  Emergent leaders, on the other hand, are the ones who naturally show these characteristics in a group.

1. Regarding ***Emergent leadership***,

* Overall, the most frequently used modalities were audio andvideo, which were captured by ARM/LAM and CUC, respectively.

* There exist only a few study performing detection of **the designated leaders** (also called **role-based leaders**) such that focusing on **crowds** and **targeting the interactions among dyads**.

* VFOA and speaking activity-based features can perform betterthan head and body activity-based cues.

2. Regarding ***leadership style detection***,

* it was <u>*limited*</u> due to not **presenting comparisons** with other **nonverbal signals**.

* there has been <u>*no attempt*</u> to perform **leadership style prediction** using **deep models**.

#### Dominance

* Following social psychology, dominance leaves traces in terms of <u>**speaking time, turn management,interruptions, pitch, body activity, facial expression, VFOA, and eye gaze**</u>.

* The **research efforts** in the dominance context mainly focused on **improving automatic detection performance**.

* The **speaking activity cues** are the most effective ones while **the body activity** cues follow them.
* **The visual information is complementary to audio** and multimodal fusion is needed to achieve better dominance estimation performance.

#### Personality Traits

Big-Five traits:

* **openness to experience** (the person who is curious, original and have wide imagination and interest)
* **conscientiousness** (the person who is efficient, organized, reliable, responsible, and thoughtful)
* **extraversion** (the person who is active, energetic, talkative, and assertive)
* **agreeableness** (the person who is trustworthy,straightforward, kind, forgiving, and generous)
* **neuroticism** (the person who is nervous, tense, sensitive, unstable and worrying)

The automatic recognition of these traits was repeatedly performed with <u>**speaking activity, VFOA, prosody, and body activity-based cues**</u>.

* **Extraversion** was <u>the best-recognized personality quality</u> which was detected by using **vocal behavioral cues** (such as pitch) and **VFOA**.

* **Openness** was <u>the second best-recognized quality</u>, and the corresponding result was obtained when the speech energy derivative was used.

* **Non-linguistic features** (<u>prosody, speech activity, overlaps, and interruptions</u>) could outperform **linguistic features** (<u>words n-gram and dialog acts</u>) for the prediction of high/low extraversion, consciousness, and neuroticism traits.

* **VFOA features** were <u>good at predicting extraversion and neuroticism</u> while the head pose errors had more impact on extraversion detection in cocktail partyscenarios.

There is no doubt that **multimodal (e.g., acoustic and vision) approaches** dominate this research line due to their remarkably better performance than **unimodal methods**.

#### Hirability

* **Multimodal nonverbal cues perform better** than unimodal audio cues (speaking activity, prosody) or unimodal video-basedfeatures (VFOA, head, and body activities).

* The most predictive ones are **the applicant's audio cues** and **the interviewer's visual cues**. This shows that the interviewer-produced responses could condition the behavior of the job applicant, i.e.,by displaying visual back-channels.

* **The higher speaking turn duration and head nods** are positively correlated to higher ratings for hirability, competence, sociability, persuasiveness, clearness, and positiveness while **verbal content is less important**.

### Social roles and relations

#### Roles

Socio-emotional roles:

1. **Protagonist**: a person who takes the floor, leads the conversation, and asserts his/her authority

2. **Supporter**: a person who is cooperative, shows attention and acceptance while providing support

3. **Neutral**:  a person who does not express his/her ideas and accepts others' ideas

4. **Gatekeeper**:  the moderator who encourages the communication between the group members

5. **Attacker**:  a person who does not agree with others' ideas, does not respect the status of others and attacks other speaker

#### Social Relations

* **Automated detection of social relations** was majorly addressed based on **computer vision** techniques.

* The **used sensors** are different types of cameras and some of them **recorded the audio** too.

* The datasets composed of **movies** or **YouTube videos** were used for the validation of the proposed methods.

![SSP_papers3](<../Pictures and Graphs/Social_role_and_relations.png>)

### Interaction Dynamics

![SSP_papers4](<../Pictures and Graphs/Interaction_analysis.png>)

#### Group Conversational Context

The types of context are:

* brainstorming vs. decision-making
* formal vs. informal
* focused vs. unfocused
* scenario vs. non-scenario

it is **noticeable** that:

* Every study utilized the **speaking activity** as a cue
* Three of four works applied **SVM** for prediction
* Three of four works used **wearable sensors**

The **speaking activity** was quantified in terms of:

* participant’s **involvement**
* the cycles of high/low activity
* **interruptions** to discriminate scenario and non-scenario meetings with **parallel episodes**

#### Engagement, Involvement and Interest Level

* Overall, **visual cues** performed better than acoustic features

* acoustic features in some cases were preferable to **lexical features**

* **gaze activity and body motion** were among the **most effective cues** to detect the phenomena of **interest**

#### Group Performance

**Automatic detection of group performance** is a task investigated mostly in small groups (3–4 people) in which **people make a decision regarding a (pre-defined) task**. That topic is important since <u>**an intelligent detection system can provide information aimed at enhancing the performance and efficiency of a group and its members**</u>.


#### Group Satisfaction



#### Quality of Interactions



#### Group Cohesion



#### Vocal Entrainment



#### Rapport and Empathy



