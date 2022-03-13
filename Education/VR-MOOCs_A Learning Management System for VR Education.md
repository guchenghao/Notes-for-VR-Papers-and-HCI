# Paper Link
---

TIME: 2019/09 IEEEXR
[VR-MOOCs: A Learning Management System for VR Education](https://ieeexplore.ieee.org/document/8798106)


# Problem
---

## purpose

- Our LMS system for the VR MOOC system is expected to shed light on how the **interactive VR learning content can be affiliated to the proper instructional design** in the near future
---

## propose
- a first of its kind-VR MOOC LMS. The chemistry experiment VR content is running for the students, and **a supervisor can monitor their learning performance and interaction behaviors**
---

# Method or Solution
---

## Device and Development tools
- HMD
---

## Steps and models
---

1. Client System

   - students can at any time ask helps from the teacher, and instant feedback from the teacher through the LMS makes them to perceive the teacher’s presence
   - he teacher can**talk through the student’s HMD**, or **intentionally manipulate the VR objects** or put them into new learning contexts through the LMS system.

2. Server System

   - Three viewpoint modes: *Student’s FP (first-person)local view*; *the world view of the student performance*; *the multi-view of all the students participated in the VR-MOOC*.

   - With regard to the teacher’s interventions, the server firstly **judges if the clients need any help**. If necessary, **the sever automatically alerts to the teacher** in order to selectively provide either direct assistance (verbal comments via the HMD speaker),or indirect assistance (direct object manipulations in the virtual environment).

   - Every behavioral and assistance data of the students are recorded in the database.
---

# Comment
---

1. 虽然这篇文章很短，也只是个demo，而且还有很多后续分析和其他工作没有做，但是这篇文章的idea point很有意思，从教育的coaching（**教育干预 educational intervention**）角度入手，分析teacher在VR Education Environment中的作用和社交定位，以此来证明VR-Mooc LMS的必要性和创新性。
   
2. 本文的核心痛点就在于在VR的环境下，teacher直接去指导或干预学生学习的表现效果不好，而且不方便（**lack of locus of control 缺乏心理控制源**），这样反而会减少学生在VR下engagement，此时本文的LMS就发挥了作用。

3. 关于这篇文章具体系统的设计方案和逻辑，本篇文章的LMS系统主要利用monitoring的思想来解读VR环境下teacher和students中间的关系和定位，以此来设计系统架构以及师生之间的interaction，具有一定的启发意义。
---

# What can be used
---

- 如果multi-user VR social platform在将来研究中被应用于education领域的话，这篇文章探讨的VR下师生关系和Moitoring的设计方案，可以借鉴或参考

- 本文在Introduction部分的分析，在今后的研究中可以被引用