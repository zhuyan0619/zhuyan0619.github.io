---
title: "Rawsamble: Overlapping and Assembling Raw Nanopore Signals using a Hash-based Seeding Mechanism"
collection: publications
category: "talks"
permalink: /publication/Rawsamble
excerpt: 'Keywords: Bioinformatics \| Genomic Analysis Algorithm \| AI for Healthcare'
date: 2024-07-14
venue: "32nd ISCB Conference on Intelligent Systems for Molecular Biology (ISMB)"
location: "Montreal, Quebec, Canada"
citation: "Can Firtina, Maximilian Mordig, Joël Lindegger, Harun Mustafa, Sayan Goswami, Stefano Mercogliano, <u>Yan Zhu</u>, Andre Kahles, Onur Mutlu"
---

Presentation Overview: Although raw nanopore signal mapping to a reference genome is widely studied to achieve highly accurate and fast mapping of raw signals, mapping to a reference genome is not possible when the corresponding reference genome of an organism is either unknown or does not exist. To circumvent such cases, all-vs-all overlapping is performed to construct de novo assembly from overlapping information. However, such an all-vs-all overlapping of raw nanopore signals remains unsolved due to its unique challenges such 1) generating multiple and accurate mapping pairs per read, 2) performing similarity search between a pair of noisy raw signals, and 3) performing space- and compute-efficient operations for portability and real-time analysis.

We introduce Rawsamble, the first mechanism that can quickly and accurately find overlaps between raw nanopore signals without translating them to bases. We find that Rawsamble can 1) find overlaps while meeting the real-time requirements with throughput on average around 200,000 bp/sec, 2) share a large portion of overlapping pairs with minimap2 (37.12% on average), and 3) lead to constructing long assemblies from these useful overlaps. Finding overlapping pairs from raw signals is critical for enabling new directions that have not been explored before for raw signal analysis, such as de novo assembly construction from overlaps that we explore in this work. We believe these overlaps can be useful for many other new directions coupled with real-time analysis.
