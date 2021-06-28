---
layout: single
classes: wide
title: Research
permalink: /research/ 
author_profile: true
author: Pierluigi Vito Amadori
---

## HammerDrive - Task-Aware Visual Attention Prediction

The proposed framework for human visual attention prediction, namely HammerDrive, leverages on two core concepts: 
1. decision recognition;
2. attention prediction. 

The HammerDrive architecture (see figure below) combines and jointly exploits these concepts as a network a) dynamically recognizes driving sub-tasks (manoeuvres), while another network b) uses maneuver recognition information to predict the focus of human visual attention.

![image-left]({{ site.url }}{{ site.baseurl }}/assets/images/Picture1.png){: .align-left}

The proposed architecture is a novel implementation of task-aware visual attention modelling as it uses easy-to-access scene and telemetry data (red) to dynamically predict action-dependent visual attention of drivers. Telemetry data is used by HAMMER (blue) to track the current driving maneuver in real-time, and a front camera provides scene information to a convolutional 3D (C3D) network, a feature extraction module. These features are processed by ParRMDN (green), an ensemble of neural networks, whose outputs are scaled according to the HAMMER task feedback signal.


![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/Picture2.png){: .align-center}

Our results showed that visual attention prediction from a module trained on a task always performs better at predicting the visual attention of a driver when the driver is performing such a task. We have also evaluated and compared the proposed architecture against state-of-the-art visual attention modelling from the literature and proven that task-awareness is greatly beneficial for human attention prediction on numerous metrics (see figure above).


## Seq2Seq - Task-Aware Visual Attention Prediction

In this work, we investigated the underlying cognitive processes that characterise human decision-making. 

![image-left]({{ site.url }}{{ site.baseurl }}/assets/images/Picture4.png){: .align-left}

To achieve this, we designed Seq2Seq (see figure left), a novel end-to-end architecture based on Long Short-Term Memory (LSTM) that uses eye gaze and head pose information to infer the likelihood of an incoming mistake from a human.

The main goal of Seq2Seq is to answer a direct research question: can we design an architecture that can anticipate whether a human's next decision will be correct or wrong?

The architecture leverages on two core concepts:
1. sequential models can model human decision-making processes with high accuracy;
2. sequence-to-sequence learning paradigm greatly improves training stability in the model, which directly translates to better inference performance.

Our results show that the Seq2Seq can reliably anticipate the correctness of incoming decisions, up to 2 seconds in advance, and that its formulation allows for real-time inference and direct closed-loop implementation.


## 5G MIMO Communications - Techniques for Energy-Efficient COmmunications

To be added. Check soon!
