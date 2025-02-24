---
title: "Towards flexible data stream collaboration: Federated Learning in Kafka-ML"
authors:
- A. J. Chaves
- C. Martín
- M. Díaz

date: "2024-01-01T00:00:00Z"
doi: "10.1016/j.iot.2023.101036"

# Schedule page publish date (NOT publication's date).
publishDate: "2024-02-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

journal: "Internet of Things"
volume: "25"
pages: "101036"
issn: "2542-6605"

abstract: Federated learning is applied in scenarios where organisations lack sufficient data volume for modelling their business logic and cannot share their data with external parties. Moreover, Industry 4.0 and IoT scenarios generate massive data streams, which normally are fed to ML/AI solutions for model training and prediction. However, in most cases, ML/AI frameworks are not prepared to work with these streaming pipelines. In this paper, we present an asynchronous federated learning solution based on the Kafka-ML data stream framework, which is able to combine federated learning and data stream capabilities within ML/AI applications. While most federated learning approaches are tailored to a specific ML model or a use case, the solution provided adapts itself to the availability of both data and ML models, achieving a flexible and dynamic federated learning solution. To validate its performance, an evaluation of the federated learning solution is carried out on different scenarios in a multi-node state-of-the-art infrastructure. Results show that this framework can work with multiple federated clients, being the resulting accuracy dependent on the amount of data and the behaviour of clients during training.

# Summary. An optional shortened abstract.
summary: This paper presents an asynchronous federated learning solution within Kafka-ML, integrating federated learning with data streams for ML/AI applications.

tags:
- Kafka-ML
- Data Streams
- Deep Learning
- Internet of Things
- Federated Learning

featured: true

links:
- name: PDF File
  url_pdf: https://www.sciencedirect.com/science/article/pii/S2542660523003591

---