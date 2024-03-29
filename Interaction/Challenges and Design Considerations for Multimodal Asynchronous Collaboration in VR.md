# Paper link

TIME: 2019/11 Proceedings of the ACM on Human-Computer Interaction

[Challenges and Design Considerations for Multimodal Asynchronous Collaboration in VR](https://dl.acm.org/doi/10.1145/3359142)

## Introduction

* With the advancement of virtual reality technology, asynchronous collaboration in immersive 3D environments has become an active research area.

* **Multimodal recording**-the capture and later playback of multiple, dynamic interaction modes, such as speech, locomotion, body language, and object manipulations-is at the foundation of **asynchronous collaboration** in these VR systems.

* There is a **significant gap** of knowledge regarding the challenges and design considerations of authoring or consuming multimodal recording in VR

* Our participants were tasked to **perform asynchronously collaborative 3D design tasks** by **viewing and recording multimodal interactions**

### Research questions

* Research questions for **multimodal asynchronous VR collaboration** (MAVRC):
  * RQ1: How are social behaviors transferred from face-to-face to MAVRC?
  * RQ2: What are the challenges of maintaining workspace awareness and coordination in MAVRC?
  * RQ3: What are the challenges of navigating and creating multimodal recordings in MAVRC?

* As for RQ1:
  * MAVRC is **fundamentally different** from those of the previous studies in that asynchronous communication is one-way-the message sender cannot respond to the viewer's inquiry in real-time.
  * It is an **open question** to what extent, or if at all, users feel the **social presence** of an **embodied 3D representation** of their asynchronous collaborator and **display social behaviors** towards it

* As for RQ2:
  * **Workspace awareness** is the knowledge of ***what is going on and what others are doing***
  * **Asynchronous change awareness** is the knowledge of how **shared artefacts** (e.g., 3D models, source code, documents) have **evolved** via the contributions of time-distributed collaborators
  * Dynamic activities of one's asynchronous collaborator can occur **out of the user's view**, and the collaborator would not know how to **draw one's attention to it**

### Key findings

* Participants felt the **social presence** of asynchronous collaborators when viewing recordings, <u>leading to proxemic behaviors and empathy</u>

* Immersion in VR can cause challenges in viewing multimodal recordings, such as **viewpoint disorientation** or **confusion** from different versions of 3D scenes

* **Recording (and viewing) co-expressive speech and body language** enabled participants to **express (and understand) nuanced ideas effectively** but **highlighted needs for editing (and browsing) tools**


![multimodal asynchronous VR collaboration](../Pictures%20and%20Graphs/../Pictures%20and%20Graphs/Multimodal_collaboration_in_VR.png)

### Contributions

* A **conceptualization** of multimodal recording based asynchronous collaboration in VR

* **Empirical findings** on the user challenges of respecting proxemics, maintaining awareness, and consuming/producing multimodal recordings in MAVRC

* **Design implications** for multimodal recording for asynchronous collaboration: proactive proxemics management, animating changes in 3D, viewpoint display for awareness, and 3D navigational cues

## Related Work

* **Asynchronous collaboration** refers to cooperative scenarios where participants interact at different times.

* Since these frameworks and tools are developed for applications in a 2D environment, it is still **unclear** how the **challenges and design considerations** for asynchronous collaboration reveal themselves differently in VR.

### Multimodal recoding and annotation

* Central to asynchronous collaboration is the exchange of messages across time.
  
* The benefit of **expressive richness** comes at a cost in **browsing and editing**.

* In contrast to these previous studies on **2D media**, our empirical setting is in **3D** where the **recording of body movement** and **scene manipulation** is a <u>multidimensional data stream</u>.

### Proxemic interactions in VR and HCI

* **Proxemics** describes the way interpersonal distance manifest social context.

* Due to the **embodied nature** of VR, many researchers studied the **social implication** of **interpersonal distance** in CVEs.
* Bailenson et al. 's study on **proxemics** in immersive VR:
  * **Human proxemic behaviors**, such as moving away from an **embodied agent** who invades one's **Personal space**, can be transferred or even **amplified** in collaborative VR environments (CVEs).
  * VR users also exhibit such behaviors to an interactive avatar with high behavioral realism

## Method

![Illustration experimental task](../Pictures%20and%20Graphs/../Pictures%20and%20Graphs/Illustration_experimental_task.png)

* This paper collected **interview** and **observation data** where subjects experienced a representative spatial task in an **asynchronously collaborative setting**.

### Experimental system: CVE for creating and viewing 3D multimodal recordings

* **Core interaction modalities** in their experimental system:
  * speech
  * **body gestures** (e.g., head and hand movements, locomotion, and pointing)
  * manipulations on scene objects

* These modalities were chosen as:
  * they enabled rich expression for **spatial tasks** in a CVE
  * were **easy to capture** using most off-the-shelf VR systems

* Integrating a **highly realistic avatar design** showing the full range of emotions and gestural interactions can <u>pose complex challenges</u> (e.g., **tracking instrumentation**, **computational complexity**) that is beyond our scope.

* In <u>asynchronous collaboration</u>, **multimodal recording** is a **medium** for **time-distributed collaborators** to exchange immersive and expressive messages.

* Our system uses a simple and familiar interface for creating and viewing recordings, modeled after **typical screen recording** or **video player** apps.
  * **Create recording**: users can click on the **"REC" button** on the **world-stabilized** VR menu
  * **View recording**: users browse through saved recordings in the menu and select one

## Comments

* 这篇文章和我目前研究关系不大。但是这篇文章对在VR或者CVEs的情况下，协作者之间进行异步协作这种情况进行了调查。

* VR下的异步协作和现实世界中的异步协作非常不同，不同VR场景下的异步协作的具体形式也不同

* 这篇文章利用representative spatial task来进行实验，然后通过参加者的交互数据和问卷数据来进行分析