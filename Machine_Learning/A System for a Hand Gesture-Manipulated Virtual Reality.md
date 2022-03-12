# Paper Link
---
[A System for a Hand Gesture-Manipulated Virtual Reality Environment](https://dl.acm.org/doi/10.1145/2987491.2987511)

# Problem
---
## purpose

- **limited research** has investigated machine learning techniques for HGR in virtual reality applications (VR).
  
- A review of current literature has revealed that many researchers have used the LMC to classify Sign Language gestures, but very few have applied it to VR.
---
## propose
- This paper reports on the design, implementation, and evaluation of **a static HGR system for VR applications using the LMC**. 
  
- The gesture recognition system incorporated **a lightweight feature vector of five normalized tip-to-palm distances and a k-nearest neighbour (kNN) classifier**.
  
- The system was evaluated in terms of **response time, accuracy and usability using a case-study** VR stellar data visualization application created in the Unreal Engine 4.
  
- This system was created to explore the efficacy of machine learning techniques for HGR in VR applications

---
# Method or Solution
---
## Device and Development tools
- Leap Motion Controller(LMC)
- Unreal Engine4
- Oculus Rift DK2
---
## Steps and modles
1. *Data Input*: Collect and read frame data from the LMC
   
2. *Static Gesture Recognition System*: According to step(1), Normalized the LMC input TPP distances data and dataset TPP distances data(Already exist).Then, use **KNN classification algorithm** to classify the static gesture.
   
3. *VR Gesture Handler*: The gesture handler is a component embedded in the application that receives a classified gesture and performs the appropriate action on the VR environment.(**use a finite state machine to divide each hand gesuture into a state**)
   
4. *VR Stellar Data Visualization Application*
---
# Experiment
---
- *preliminary User Study*: Three new users, two men and a woman of varying hand
sizes, were included in the study to **measure the ease of use and comfort of the system**.
---
# Result or Conclusion
---
- the system is **lightweight enough** to allow the program to run at a **high framerate**, which is an important consideration to take when developing for VR.
  
- Static gestures used in the application had an 82.5% accuracy rate, with a minimum of 60% accuracy with the point gesture and a maximum of 100% accuracy with the fist gesture.
  
- Gestures with low accuracy ratings primarily suffered from **occlusion issues**
---
# Comment
---
1. 这篇文章完整地介绍了整个系统的设计方案和使用工具，这点思路很清晰。
   
2. 这篇文章**没有立足于某个特定的应用场景，也没有针对没有领域的特定问题**，而是基于HGR技术很少被应用于VR中这个点以及与传统手势数据收集方式进行对比(本文章利用LMc以及VR的前沿技术)，来**填补HGR技术和VR结合这个空白(相对来说)**，因此设计了这个系统。
   
3. 这篇文章的user study过于单薄和简单，实验流程和思路倒还是清晰的，但是实验样本太少，缺少说服力，文章作者自己也点出这个问题。
   
4. 这篇文章在classification算法部分的设计过于简单，并没有考虑很周全。
   
5. 这个系统的亮点除了之前说的填补了一个所谓的**应用空白**，作者还还强调该系统的lightweight(轻量级)，可以以高帧率在VR环境下运行，从侧面说明了KNN算法在这方面的应用优势。
---
# What can be used
---
- lightweight这个点可以在未来的应用设计或者系统设计中被关注，成为一个考虑方向
  
- 这边文章的系统结合ML算法和VR应用的设计思路，在未来研究中可供参考