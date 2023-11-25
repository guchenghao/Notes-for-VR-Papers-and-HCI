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

* ***Free-standing conversations*** (conv.) are the settings in which proxemics play the most important role and individual distances were shown to account forthe detection of multiple social phenomena including _social roles, leadership, engagement and personality traits_.

#### Physical Appearance

This includes height, body shape, skin/hair color, clothes, and make-up of a person.

### Sensors

For what concerns **vocal behavior**, the most frequent sensors are **microphones** of different types:

- close-talk (CTM)
- headset (HSM)
- tabletop (TTM)
- lapel (LAM)
- microphone arrays (ARM)
- omnidirectional (ODM)
- four-channel cardioid (FCM)
- other distantly placed microphones such as single-channel far-field (FFM)

In the case of **_body activity, eye gaze, VFOA, facial expressions, proximity, and the physical appearance of the participants_**, the main sensors are **cameras**:

- close-up (CUC)
- Red Green Blue Depth (RGBD)
- web (WC)
- 360 degrees (C360)
- frame-synchronized (FSC)
- digital movie (DMC)
- top-view (TVC)
- wearable(WCM)
- narrative (NC)
- pan and tilt zoom (PTZ)
- far-field (FFC)
- a combination of them

Except microphones and cameras, other sensing technologies have also attracted researchers:

- Smartphone: comprehensive
- Accelerometers(ACC): the analysis of small group round-table meetings as well as the analysis of mingling scenarios
- Sociometer badges(SB)
- Head-mounted wearables: capture the speech, body movement and gaze
- Respiration sensors
- Biological sensors: nonverbal behaviors, EEG

### Computational Methods

***Machine learning, deep learning supervised and unsupervised approaches***

![SSP_papers1](<../Pictures and Graphs/Papers_with_SSP_1.png>)
![SSP_papers2](<../Pictures and Graphs/papers_with_SSP_2.png>)

## Reviews: Methodologies of SSP


### Social Traits

### Social roles or relations

### Interaction Dynamics

