# ISSTA

[Back](../README.md#all-papers)

## ISSTA 2023

### Dependency-Aware Metamorphic Testing of Datalog Engines

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3597926.3598052)

**Abstract:** Datalog is a declarative query language with wide applicability, especially in program analysis. Queries are evaluated by Datalog engines, which are complex and thus prone to returning incorrect results. Such bugs, called query bugs, may compromise the soundness of upstream program analyzers, having potentially detrimental consequences in safety-critical settings.

To address this issue, we develop a metamorphic testing approach for detecting query bugs in Datalog engines. In comparison to existing work, our approach is based on rich precedence information capturing dependencies among relations in the program. This enables much more general and effective metamorphic transformations. We implement our approach in DLSmith, which detected 16 previously unknown query bugs in four Datalog engines.

### ECSTATIC: Automatic Configuration-Aware Testing and Debugging of Static Analysis Tools

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3597926.3604918)

**Abstract:** Static analyses are powerful tools that can serve as a complement to dynamic approaches such as testing. In order to ensure generality, many static analysis tools are configurable. However, these configurations can make testing and debugging more difficult. To address this issue, we introduce a new tool, ECSTATIC, which leverages partial order relations between analysis configuration options to automatically test and debug static analyzers, even without ground truths. ECSTATIC’s results are reproducible by virtue of running within Docker containers, and ECSTATIC provides clear extension interfaces for users to add their own tools and input programs. We evaluated ECSTATIC on four popular dataflow analysis tools, and found 74 bugs in all four tools. We also found that ECSTATIC’s novel two-staged delta debugging was able to reduce real-world programs by 50%, compared to a baseline of 6%.

## ISSTA 2022

### One Step Further: Evaluating Interpreters using Metamorphic Testing

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3533767.3534225)

**Abstract:** The black-box nature of the Deep Neural Network (DNN) makes it difficult for people to understand why it makes a specific decision, which restricts its applications in critical tasks. Recently, many interpreters (interpretation methods) are proposed to improve the transparency of DNNs by providing relevant features in the form of a saliency map. However, different interpreters might provide different interpretation results for the same classification case, which motivates us to conduct the robustness evaluation of interpreters.

However, the biggest challenge of evaluating interpreters is the testing oracle problem, i.e., hard to label ground-truth interpretation results. To fill this critical gap, we first use the images with bounding boxes in the object detection system and the images inserted with backdoor triggers as our original ground-truth dataset. Then, we apply metamorphic testing to extend the dataset by three operators, including inserting an object, deleting an object, and feature squeezing the image background. Our key intuition is that after the three operations which do not modify the primary detected objects, the interpretation results should not change for good interpreters. Finally, we measure the qualities of interpretation results quantitatively with the Intersection-over-Minimum (IoMin) score and evaluate interpreters based on the statistics of metamorphic relation's failures.

We evaluate seven popular interpreters on 877,324 metamorphic images in diverse scenes. The results show that our approach can quantitatively evaluate interpreters' robustness, where Grad-CAM provides the most reliable interpretation results among the seven interpreters.

### Metamorphic Relations via Relaxations: An Approach to Obtain Oracles for Action-Policy Testing

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3533767.3534392)
* <img src="../icons/Github.png" width="24px">[Code](https://github.com/Practical-Formal-Methods/pi-fuzz)

**Abstract:** Testing is a promising way to gain trust in a learned action policy π, in particular if π is a neural network. A “bug” in this context constitutes undesirable or fatal policy behavior, e.g., satisfying a failure condition. But how do we distinguish whether such behavior is due to bad policy decisions, or whether it is actually unavoidable under the given circumstances? This requires knowledge about optimal solutions, which defeats the scalability of testing. Related problems occur in software testing when the correct program output is not known.

Metamorphic testing addresses this issue through metamorphic relations, specifying how a given change to the input should affect the output, thus providing an oracle for the correct output. Yet, how do we obtain such metamorphic relations for action policies? Here, we show that the well explored concept of relaxations in the Artificial Intelligence community can serve this purpose. In particular, if state s′ is a relaxation of state s, i.e., s′ is easier to solve than s, and π fails on easier s′ but does not fail on harder s, then we know that π contains a bug manifested on s′.

We contribute the first exploration of this idea in the context of failure testing of neural network policies π learned by reinforcement learning in simulated environments. We design fuzzing strategies for test-case generation as well as metamorphic oracles leveraging simple, manually designed relaxations. In experiments on three single-agent games, our technology is able to effectively identify true bugs, i.e., avoidable failures of π, which has not been possible until now.

## ISSTA 2018

### Identifying Implementation Bugs in Machine Learning Based Image Classifiers using Metamorphic Testing

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3213846.3213858)

We have recently witnessed tremendous success of Machine Learning (ML) in practical applications. Computer vision, speech recognition and language translation have all seen a near human level performance. We expect, in the near future, most business applications will have some form of ML. However, testing such applications is extremely challenging and would be very expensive if we follow today's methodologies. In this work, we present an articulation of the challenges in testing ML based applications. We then present our solution approach, based on the concept of Metamorphic Testing, which aims to identify implementation bugs in ML based image classifiers. We have developed metamorphic relations for an application based on Support Vector Machine and a Deep Learning based application. Empirical validation showed that our approach was able to catch 71% of the implementation bugs in the ML applications.