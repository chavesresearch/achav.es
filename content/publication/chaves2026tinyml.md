---
title: "Orchestrating TinyML Soft Sensors With Data Streams: A Hybrid Cloud-Edge Architecture for IoT Scenarios"
authors:
- A. J. Chaves
- C. Martín
- A. Shahid
- M. Díaz

date: "2026-10-19T00:00:00Z"
doi: "10.1002/spe.70119"

journal: "Software: Practice and Experience"

# Schedule page publish date (NOT publication's date).
publishDate: "2026-10-27T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

abstract: "The deployment of soft sensors, data-based models that estimate unobservable or costly variables from available sensor data, remains limited in IoT infrastructures by the resource constraints of IoT devices and the complexity of managing model lifecycles at scale. This work presents a novel architecture that enables the end-to-end transformation, distribution and execution of soft sensors on IoT embedded devices. The proposed approach leverages Kafka-ML, a framework for managing ML models and data streams, which has been extended to orchestrate the end-to-end lifecycle of soft sensors in real time via IoT data streams. By enabling local inference on IoT devices, the system reduces reliance on cloud connectivity during operation: while initial deployment, model updates, and lifecycle orchestration via Kafka-ML require network access, local inference allows the estimation of complex variables even when subsequent connectivity is unreliable or intermittent. The approach has been evaluated in two representative scenarios, non-intrusive load monitoring (NILM) and water quality monitoring, each with different demands regarding communications overhead and accuracy. The automated quantization pipeline yields negligible accuracy degradation for the NILM scenario (MAE shifted from 2.836 to 2.837) and an acceptable performance trade-off for water quality monitoring (MAE rose from 0.53 to 0.82 mg/L), while reducing inference latency by up to 4.6× compared to remote inference. These results demonstrate the framework's capability to automate the deployment of distributed, autonomous, and privacy-preserving soft sensors across heterogeneous monitoring scenarios."

# Summary. An optional shortened abstract.
summary: This paper extends Kafka-ML with a hybrid cloud-edge architecture that automatically quantizes, deploys over-the-air and orchestrates TinyML soft sensors on IoT devices fed by data streams.

tags:
- TinyML
- Soft Sensors
- Edge Computing
- Kafka-ML
- Model Orchestration
- Internet of Things

featured: true

links:
- name: PDF File
  url: files/chaves2026tinyml.pdf
---
