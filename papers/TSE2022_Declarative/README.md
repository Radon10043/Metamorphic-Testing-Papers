# Feedback-directed Metamorphic Testing

* <img src="../../icons/pdf.png" width="24px">[Paper](./A_Declarative_Metamorphic_Testing_Framework_for_Autonomous_Driving.pdf)

**Abstract:** Autonomous driving has gained much attention from both industry and academia. Currently, Deep Neural Networks (DNNs) are widely used for perception and control in autonomous driving. However, several fatal accidents caused by autonomous vehicles have raised serious safety concerns about autonomous driving models. Some recent studies have successfully used the metamorphic testing technique to detect thousands of potential issues in some popularly used autonomous driving models. However, prior study is limited to a small set of metamorphic relations, which do not reflect rich, real-world traffic scenarios and are also not customizable. This paper presents a novel declarative rule-based metamorphic testing framework called RMT . RMT provides a rule template with natural language syntax, allowing users to flexibly specify an enriched set of testing scenarios based on real-world traffic rules and domain knowledge. RMT automatically parses human-written rules to metamorphic relations using an NLP-based rule parser referring to an ontology list and generates test cases with a variety of image transformation engines. We evaluated RMT on three autonomous driving models. With an enriched set of metamorphic relations, RMT detected a significant number of abnormal model predictions that were not detected by prior work. Through a large-scale human study on Amazon Mechanical Turk, we further confirmed the authenticity of test cases generated by RMT and the validity of detected abnormal model predictions.

[Back](../../README.md)