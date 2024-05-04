# Chapter 1. Overview of Machine Learning Systems

When to Use Machine Learning

Machine learning is an approach to (1) learn (2) complex patterns from (3) existing data and use these patterns to make (4) predictions on (5) unseen data.

 1. Learn: the system has the capacity to learn
 2. Complex patterns: there are patterns to learn, and they are complex
 3. Existing data: data is available, or it’s possible to collect data
 4. Predictions: it’s a predictive problem
 5. Unseen data: unseen data shares patterns with the training data

ML solutions will especially shine if your problem has these additional following characteristics:

 6. It’s repetitive
 7. The cost of wrong predictions is cheap
 8. It’s at scale
 9. The patterns are constantly changing

Machine Learning Use Cases

- Enterprise ML applications tend to have vastly different requirements and considerations from consumer applications
- Fraud detection
- Price optimization
- Churn prediction
- brand monitoring.

Understanding Machine Learning Systems

- Machine Learning in Research Versus in Production

|              | Research                                                | Production                                            |
|--------------|---------------------------------------------------------|-------------------------------------------------------|
| Requirements | State-of-the-art model performance on benchmark datasets | Different stakeholders have different requirements   |
| Computational priority | Fast training, high throughput                  | Fast inference, low latency                           |
| Data         | Static                                                  | Constantly shifting                                    |
| Fairness     | Often not a focus                                      | Must be considered                                    |
| Interpretability | Often not a focus                                  | Must be considered                                    |

- Different stakeholders and requirements

  - ML engineers
  - Sales team
  - Product team
  - ML platform team
  - Manager

- Computational priorities

  - latency
  - throughput

- Data

  - Dataset
  - Models and algorithms

- Fairness
    ML algorithms don’t predict the future, but encode the past

- Interpretability

- Machine Learning Systems Versus Traditional Software

| Challenge                                          | ML Perspective                                                                                                                                                                                                                                                                                              | SWE Perspective                                                                                                                                                                                                                                                             |
|----------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Code and Data Separation                          | ML systems integrate code, data, and artifacts, blurring the lines between them.                                                                                                                                                                                                                         | SWE emphasizes modularization and separation of concerns, keeping code and data distinct.                                                                                                                                                                                  |
| Importance of Data                                 | Data quality and quantity are paramount; applications are often driven by the quality and diversity of data.                                                                                                                                                                                            | SWE focuses on code quality and robustness; data is considered static and secondary.                                                                                                                                                                                        |
| Testing and Versioning                            | Testing and versioning encompass both code and data, with a focus on understanding data quality and relevance.                                                                                                                                                                                            | Testing and versioning primarily concern code, with less emphasis on data versioning and testing.                                                                                                                                                                          |
| Model Size                                         | ML models can be massive, with billions of parameters requiring significant memory for loading into RAM.                                                                                                                                                                                                   | SWE typically deals with smaller codebases and less memory-intensive operations.                                                                                                                                                                                            |
| Deployment Challenges                              | Deploying large models, especially on edge devices, poses engineering challenges due to resource constraints.                                                                                                                                                                                             | SWE deployment focuses on efficient software delivery and installation, often on standardized hardware.                                                                                                                                                                   |
| Performance Optimization                          | ML models need to be optimized for speed to be practical; performance is critical for real-time applications.                                                                                                                                                                                            | SWE optimization focuses on code efficiency and algorithmic performance, often less critical for real-time responsiveness.                                                                                                                                              |
| Monitoring and Debugging                          | Monitoring and debugging ML models in production is complex due to model complexity and lack of visibility into their decision-making process.                                                                                                                                                           | SWE emphasizes robust logging, error handling, and debugging tools for code-based issues.                                                                                                                                                                                 |
| Evolution of Technology and Engineering Solutions | Engineering challenges in ML are rapidly evolving, with solutions emerging to address scalability, efficiency, and deployment issues.                                                                                                                                                                    | SWE solutions evolve more gradually, building on established best practices and methodologies.                                                                                                                                                                             |
| Example: BERT Evolution                          | BERT, initially criticized for size and complexity, quickly became a standard in ML applications, showcasing the rapid pace of technological advancement and adoption.                                                                                                                                 | Example technologies like BERT demonstrate the iterative improvement and adoption cycles in software development, albeit at a slower pace than in the ML domain.                                                                                                        |
