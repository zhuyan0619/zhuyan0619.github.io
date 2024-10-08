---
title: "A Scalable Architecture for Reprioritizing Ordered Parallelism"
collection: publications
category: conferences
permalink: /publication/HIVE
excerpt: 'Keywords: Computer Architecture \| Execution Model & Multicore Architecture \| Speculative Execution'
date: 2022-06-19
venue: '49th IEEE/ACM International Symposium on Computer Architecture (ISCA)'
slidesurl: 'http://zhuyan0619.github.io/files/HIVE_presentation.pdf'
paperurl: 'http://zhuyan0619.github.io/files/HIVE_paper.pdf'
citation: 'Gilead Posluns, <u>Yan Zhu</u>, Guowei Zhang, Mark C. Jeffrey'
---

Abstract: Many algorithms schedule their work, or tasks, according to a priority order for correctness or faster convergence. While priority schedulers commonly implement task enqueue and dequeueMin operations, some algorithms need a priority update operation that alters the scheduling metadata for a task. Prior software and hardware systems that support scheduling with priority updates compromise on either parallelism, work-efficiency, or both, leading to missed performance opportunities. Moreover, incorrectly navigating these compromises violates correctness in those algorithms that are not resilient to relaxing priority order.

We present Hive, a task-based execution model and multicore architecture that extracts abundant fine-grain parallelism from algorithms with priority updates, while retaining their strict priority schedules. Like prior hardware systems for ordered parallelism, Hive uses data- and control-dependence speculation and a large speculative window to execute tasks in parallel and out of order. Hive improves on prior work by (i) directly supporting updates in the interface, (ii) identifying the novel scheduler-carried dependence, and (iii) speculating on such dependences with task versioning, distinct from data versioning. Hive enables safe speculative updates to the schedule and avoids spurious conflicts among tasks to better utilize speculation tracking resources and efficiently uncover more parallelism. Across a suite of nine benchmarks, Hive improves performance at 256 cores by up to 2.8× over the next best hardware solution, and even more over software-only parallel schedulers.