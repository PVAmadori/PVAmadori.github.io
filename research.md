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

Our results showed that visual attention prediction from a module trained on a task always performs better at predicting the visual attention of a driver when the driver is performing such a task. I have also evaluated and compared the proposed architecture against state-of-the-art visual attention modelling from the literature and proven that task-awareness is greatly beneficial for human attention prediction on numerous metrics (see figure above).


## Seq2Seq/DecNet - Cognitive Overload Detection via Decision Anticipation

In this work, I developed two end-to-end networks to detect cognitive overload events in human via decision anticipation. The main assumption in this framework is that decision mistakes on the cognitive secondary task of dual-tasking users correspond to cognitive overload events. Cognitive overload events are instances wherein the cognitive resources
required to perform the task exceed the ones available to the users.

The architectures build on two core concepts:

1. sequential models can model human decision-making processes with high accuracy;
2. sequence-to-sequence learning paradigm greatly improves training stability in the model, which directly translates to better inference performance.

![image-left]({{ site.url }}{{ site.baseurl }}/assets/images/Picture3.png){: width="400" .align-left}

I designed Seq2Seq and DecNet (see figure left), two novel end-to-end architectures based on Long Short-Term Memory (LSTM) and Recurrent Neural Networks (RNN) that use eye gaze and head pose information to infer the likelihood of an incoming mistake from a human. DecNet is designed as a two-stage end-to-end sequential model that jointly learns to extract the most relevant features via an RNN module and to exploit them via an LSTM network in order to infer cognitive overload events by anticipating the correctness likelihood of an imminent decision. In other words, the hidden states of the RNN are used as input to the LSTM module (see figure below).

![image-left]({{ site.url }}{{ site.baseurl }}/assets/images/Picture4.png){: width="400"  .align-left}

The main goal of DecNet is to answer a direct research question: can we design an architecture that can anticipate cognitive overload events in humans by predicting whether a their next decision will be correct or wrong?

Our results show that the DecNet can reliably anticipate the correctness of incoming decisions, up to 2 seconds in advance, and that its formulation allows for real-time inference and direct closed-loop implementation.


## 5G MIMO Communications - Techniques for Energy-Efficient Communications

During my PhD studies at UCL, I focused my research on developing algorithms to improve energy efficiency of future 5G communications systems. I addressed energy efficiency both with algorithms to *improve the power efficiency of the hardware* and with techniques to *reduce the complexity of the hardware* itself.

To improve hardware power efficiency, I designed two downlink precoding techniques based on cross-entropy optimization and a two-step convex optimization-based algorithm to exploit interference as a source of additional power for communications. These techniques exploit the concept of **constructive interference** to improve the received power on handheld devices without the need to increase the power at the transmitter side.

To reduce the hardware complexity of communication systems, I developed several antenna selection algorithms which allow to reduce the number of radiating elements at the transmitter side, while preserving desired performance in terms of data throughput. I applied the concepts of antenna selection to both LTE bands and extremely high frequency bands for 5G, also known as millimetre-wave bands. 

Finally, I also combined both approaches to improve communications systems efficiency by designing a novel algorithm that jointly optimizes precoding and antenna selection at the transmitter side. This joint-optimization problem is very complex, and I proposed both a mixed-integer programming approach and an alternate optimization-based approach. My results showed that a joint solution to the precoding and antenna selection problems provide great benefits in terms of energy efficiency, as it offers a best-of-both-worlds solution.