---
layout: post
categories: Papers-I-Read
title: Reconstruction and Simulation of Neocortical Microcircuitry
tags: [Papers-I-Read, Neuroscience, Cell]
---

[Link to Paper](https://www.cell.com/fulltext/S0092-8674%2815%2901191-5)

The paper reports on Neuralink’s approach to scalable and extensible brain machine interfaces. They successfully develop flexible polymer probes and a robot to insert them, achieving a BMI with a high channel count and great single-spike resolution.

Existing electrodes are incapable of long term neural recording as they are either metal or semiconductor based. To combat this, a thin and flexible electrode made primarily from polyimide encapsulating a gold film is developed. It is both better in terms of longevity and biocompatibility. These ultra-fine polymer probes are patterned on a wafer, with 3,072 electrodes per array distributed across 96 threads. Each thread has 32 independent probes. Different treatments for surface modification are used to lower the impedance of these probes.

For precise and automated insertion of these probes, a neurosurgical robot is built. The robot consists of a needle (for holding threads and penetrating brain tissue) and an imaging stack (for live viewing, guiding, insertion and verification of threads). A custom software is used to pre select insertion sites and define robot insertion paths. The robot is capable of inserting 192 electrodes per minute, each one at a time! The flexibility to insert these flexible probes at target specific regions, without any vasculature at such speed, is commendable.

The arrays of electrodes are packaged into tiny implantable devices capable of recording from 3072 channels simultaneously. A custom application specific integrated circuit (ASIC) is used for
on-board amplification and digitization of signals. The system was tested on freely moving rats.

I believe that BMIs hold the potential for treatment of several neurological disorders. Due to the restrain on reading from a large number of neurons, their clinical use has been limited. The system presented in the paper, is a significant step towards fully implantable human BMI systems.
