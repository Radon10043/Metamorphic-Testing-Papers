# TSE

[Back](../README.md#all-papers)

## TSE 2023

### Feedback-directed Metamorphic Testing

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3533314)

**Abstract:** Over the past decade, metamorphic testing has gained rapidly increasing attention from both academia and industry, particularly thanks to its high efficacy on revealing real-life software faults in a wide variety of application domains. On the basis of a set of metamorphic relations among multiple software inputs and their expected outputs, metamorphic testing not only provides a test case generation strategy by constructing new (or follow-up) test cases from some original (or source) test cases, but also a test result verification mechanism through checking the relationship between the outputs of source and follow-up test cases. Many efforts have been made to further improve the cost-effectiveness of metamorphic testing from different perspectives. Some studies attempted to identify “good” metamorphic relations, while other studies were focused on applying effective test case generation strategies especially for source test cases. In this article, we propose improving the cost-effectiveness of metamorphic testing by leveraging the feedback information obtained in the test execution process. Consequently, we develop a new approach, namely feedback-directed metamorphic testing, which makes use of test execution information to dynamically adjust the selection of metamorphic relations and selection of source test cases. We conduct an empirical study to evaluate the proposed approach based on four laboratory programs, one GNU program, and one industry program. The empirical results show that feedback-directed metamorphic testing can use fewer test cases and take less time than the traditional metamorphic testing for detecting the same number of faults. It is clearly demonstrated that the use of feedback information about test execution does help enhance the cost-effectiveness of metamorphic testing. Our work provides a new perspective to improve the efficacy and applicability of metamorphic testing as well as many other software testing techniques.

### Metamorphic Testing for Web System Security

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/10089522/)

**Abstract:** Security testing aims at verifying that the software meets its security properties. In modern Web systems, however, this often entails the verification of the outputs generated when exercising the system with a very large set of inputs. Full automation is thus required to lower costs and increase the effectiveness of security testing. Unfortunately, to achieve such automation, in addition to strategies for automatically deriving test inputs, we need to address the oracle problem, which refers to the challenge, given an input for a system, of distinguishing correct from incorrect behavior (e.g., the response to be received after a specific HTTP GET request). In this paper, we propose Metamorphic Security Testing for Web-interactions ( MST-wi ), a metamorphic testing approach that integrates test input generation strategies inspired by mutational fuzzing and alleviates the oracle problem in security testing. It enables engineers to specify metamorphic relations (MRs) that capture many security properties of Web systems. To facilitate the specification of such MRs, we provide a domain-specific language accompanied by an Eclipse editor. MST-wi automatically collects the input data and transforms the MRs into executable Java code to automatically perform security testing. It automatically tests Web systems to detect vulnerabilities based on the relations and collected data. We provide a catalog of 76 system-agnostic MRs to automate security testing in Web systems. It covers 39% of the OWASP security testing activities not automated by state-of-the-art techniques; further, our MRs can automatically discover 102 different types of vulnerabilities, which correspond to 45% of the vulnerabilities due to violations of security design principles according to the MITRE CWE database. We also define guidelines that enable test engineers to improve the testability of the system under test with respect to our approach. We evaluated MST-wi effectiveness and scalability with two well-known Web systems (i.e., Jenkins and Joomla). It automatically detected 85% of their vulnerabilities and showed a high specificity (99.81% of the generated inputs do not lead to a false positive); our findings include a new security vulnerability detected in Jenkins. Finally, our results demonstrate that the approach scale, thus enabling automated security testing overnight.

## TSE 2022

### Using Metamorphic Testing to Improve the Quality of Tags in OpenStreetMap

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/9729566)

**Abstract:** We present a metamorphic testing approach to validate the information included in OpenStreetMap, a collaborative effort to produce a free map of the world. We focus on the quality of the tags storing the information about the elements of the map. We identified metamorphic relations with the potential to detect different types of tagging errors. In particular, we carefully designed mechanisms to automatically generate follow-up inputs , a fundamental component in the successful application of a metamorphic testing approach. The intrinsic nature of automatically analysing tags implies that we will detect real errors but some false positives as well. In order to obtain a good trade-off between real errors and false positives, we introduce thresholds . Our MRs will raise an error associated with a certain value if, depending on the nature of the MR, we have a certain number of elements (not) fulfilling a given condition. In order to evaluate the goodness and versatility of our framework, we chose four cities in different continents with the goal of analysing very heterogeneous contributors adding information in different languages. The application of this framework to the analysis of the chosen cities revealed errors in all of them and in all the considered categories. In addition, around 66% of the errors found by our MRs in the analysed areas have not been previously reported by Osmose , the de facto standard OSM error checker.

### A Declarative Metamorphic Testing Framework for Autonomous Driving

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/9906558)

**Abstract:** Autonomous driving has gained much attention from both industry and academia. Currently, Deep Neural Networks (DNNs) are widely used for perception and control in autonomous driving. However, several fatal accidents caused by autonomous vehicles have raised serious safety concerns about autonomous driving models. Some recent studies have successfully used the metamorphic testing technique to detect thousands of potential issues in some popularly used autonomous driving models. However, prior study is limited to a small set of metamorphic relations, which do not reflect rich, real-world traffic scenarios and are also not customizable. This paper presents a novel declarative rule-based metamorphic testing framework called RMT . RMT provides a rule template with natural language syntax, allowing users to flexibly specify an enriched set of testing scenarios based on real-world traffic rules and domain knowledge. RMT automatically parses human-written rules to metamorphic relations using an NLP-based rule parser referring to an ontology list and generates test cases with a variety of image transformation engines. We evaluated RMT on three autonomous driving models. With an enriched set of metamorphic relations, RMT detected a significant number of abnormal model predictions that were not detected by prior work. Through a large-scale human study on Amazon Mechanical Turk, we further confirmed the authenticity of test cases generated by RMT and the validity of detected abnormal model predictions.

## TSE 2021

### Enhance Combinatorial Testing With Metamorphic Relations

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/9629275)

**Abstract:** Due to the effectiveness and efficiency in detecting defects caused by interactions of multiple factors, Combinatorial Testing (CT) has received considerable scholarly attention in the last decades. Despite numerous practical test case generation techniques being developed, there remains a paucity of studies addressing the automated oracle generation problem, which holds back the overall automation of CT. As a consequence, much human intervention is inevitable, which is time-consuming and error-prone. This costly manual task also restricts the application of higher testing strength, inhibiting the full exploitation of CT in industrial practice. To bridge the gap between test designs and fully automated test flows, and to extend the applicability of CT, this paper presents a novel CT methodology, named COMER, to enhance the traditional CT by accounting for Metamorphic Relations (MRs). COMER puts a high priority on generating pairs of test cases which match the input rules of MRs, i.e., the Metamorphic Group (MG) , such that the correctness can be automatically determined by verifying whether the outputs of these test cases violate their MRs. As a result, COMER can not only satisfy the t-way coverage as what CT does, but also automatically check as many test oracle violations as possible. Several empirical studies conducted on 31 real-world software projects have shown that COMER increased the number of metamorphic groups by an average factor of 75.9 and also increased the failure detection rate by an average factor of 11.3, when compared with CT, while the overall number of test cases generated by COMER barely increased.

### Metamorphic Robustness Testing: Exposing Hidden Defects in Citation Statistics and Journal Impact Factors

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/8708940)

**Abstract:** We propose a robustness testing approach for software systems that process large amounts of data. Our method uses metamorphic relations to check software output for erroneous input in the absence of a tangible test oracle. We use this technique to test two major citation database systems: Scopus and the Web of Science. We report a surprising finding that the inclusion of hyphens in paper titles impedes citation counts, and that this is a result of the lack of robustness of the citation database systems in handling hyphenated paper titles. Our results are valid for the entire literature as well as for individual fields such as chemistry. We further find a strong and significant negative correlation between the journal impact factor (JIF) of IEEE Transactions on Software Engineering (TSE) and the percentage of hyphenated paper titles published in TSE. Similar results are found for ACM Transactions on Software Engineering and Methodology. A software engineering field-wide study reveals that the higher JIF-ranked journals are publishing a lower percentage of papers with hyphenated titles. Our results challenge the common belief that citation counts and JIFs are reliable measures of the impact of papers and journals, as they can be distorted simply by the presence of hyphens in paper titles.

### BiasFinder: Metamorphic Test Generation to Uncover Bias for Sentiment Analysis Systems

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/9653830)

**Abstract:** Artificial intelligence systems, such as Sentiment Analysis (SA) systems, typically learn from large amounts of data that may reflect human bias. Consequently, such systems may exhibit unintended demographic bias against specific characteristics (e.g., gender, occupation, country-of-origin, etc.). Such bias manifests in an SA system when it predicts different sentiments for similar texts that differ only in the characteristic of individuals described. To automatically uncover bias in SA systems, this paper presents BiasFinder, an approach that can discover biased predictions in SA systems via metamorphic testing. A key feature of BiasFinder is the automatic curation of suitable templates from any given text inputs, using various Natural Language Processing (NLP) techniques to identify words that describe demographic characteristics. Next, BiasFinder generates new texts from these templates by mutating words associated with a class of a characteristic (e.g., gender-specific words such as female names, “she”, “her”). These texts are then used to tease out bias in an SA system. BiasFinder identifies a bias-uncovering test case (BTC) when an SA system predicts different sentiments for texts that differ only in words associated with a different class (e.g., male vs. female) of a target characteristic (e.g., gender). We evaluate BiasFinder on 10 SA systems and 2 large scale datasets, and the results show that BiasFinder can create more BTCs than two popular baselines. We also conduct an annotation study and find that human annotators consistently think that test cases generated by BiasFinder are more fluent than the two baselines.

## TSE 2020

### Theoretical and Empirical Analyses of the Effectiveness of Metamorphic Relation Composition

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/9144441)

**Abstract:** Metamorphic Relations (MRs) play a key role in determining the fault detection capability of Metamorphic Testing (MT). As human judgement is required for MR identification, systematic MR generation has long been an important research area in MT. Additionally, due to the extra program executions required for follow-up test cases, some concerns have been raised about MT cost-effectiveness. Consequently, the reduction in testing costs associated with MT has become another important issue to be addressed. MR composition can address both of these problems. This technique can automatically generate new MRs by composing existing ones, thereby reducing the number of follow-up test cases. Despite this advantage, previous studies on MR composition have empirically shown that some composite MRs have lower fault detection capability than their corresponding component MRs. To investigate this issue, we performed theoretical and empirical analyses to identify what characteristics component MRs should possess so that their corresponding composite MR has at least the same fault detection capability as the component MRs do. We have also derived a convenient, but effective guideline so that the fault detection capability of MT will most likely not be reduced after composition.

## TSE 2019

### METRIC+: A Metamorphic Relation Identification Technique Based on Input Plus Output Domains

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/8807231)

**Abstract:** Metamorphic testing is well known for its ability to alleviate the oracle problem in software testing. The main idea ofmetamorphic testing is to test a software system by checking whether each identified metamorphic relation (MR) holds among severalexecutions. In this regard, identifying MRs is an essential task in metamorphic testing. In view of the importance of this identificationtask, METRIC (METamorphic Relation Identification based on Category-choice framework) was developed to help software testersidentify MRs from a given set of complete test frames. However, during MR identification, METRIC primarily focuses on the inputdomain without sufficient attention given to the output domain, thereby hindering the effectiveness of METRIC. Inspired by this problem,we have extended METRIC into METRIC + by incorporating the information derived from the output domain for MR identification. A toolimplementing METRIC + has also been developed. Two rounds of experiments, involving four real-life specifications, have beenconducted to evaluate the effectiveness and efficiency of METRIC + . The results have confirmed that METRIC + is highly effective andefficient in MR identification. Additional experiments have been performed to compare the fault detection capability of the MRsgenerated by METRIC + and those bymMT (another MR identification technique). The comparison results have confirmed that the MRsgenerated by METRIC + are highly effective in fault detection.

## TSE 2018

### Metamorphic Relations for Enhancing System Understanding and Use

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/8493260)

Modern information technology paradigms, such as online services and off-the-shelf products, often involve a wide variety of users with different or even conflicting objectives. Every software output may satisfy some users, but may also fail to satisfy others. Furthermore, users often do not know the internal working mechanisms of the systems. This situation is quite different from bespoke software, where developers and users typically know each other. This paper proposes an approach to help users to better understand the software that they use, and thereby more easily achieve their objectives—even when they do not fully understand how the system is implemented. Our approach borrows the concept of metamorphic relations from the field of metamorphic testing (MT), using it in an innovative way that extends beyond MT. We also propose a “symmetry” metamorphic relation pattern and a “change direction” metamorphic relation input pattern that can be used to derive multiple concrete metamorphic relations. Empirical studies reveal previously unknown failures in some of the most popular applications in the world, and show how our approach can help users to better understand and better use the systems. The empirical results provide strong evidence of the simplicity, applicability, and effectiveness of our methodology.

**Abstract:**

## TSE 2016

### A Survey on Metamorphic Testing

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/7422146)

**Abstract:** A test oracle determines whether a test execution reveals a fault, often by comparing the observed program output to the expected output. This is not always practical, for example when a program's input-output relation is complex and difficult to capture formally. Metamorphic testing provides an alternative, where correctness is not determined by checking an individual concrete output, but by applying a transformation to a test input and observing how the program output “morphs” into a different one as a result. Since the introduction of such metamorphic relations in 1998, many contributions on metamorphic testing have been made, and the technique has seen successful applications in a variety of domains, ranging from web services to computer graphics. This article provides a comprehensive survey on metamorphic testing: It summarises the research results and application areas, and analyses common practice in empirical studies of metamorphic testing as well as the main open challenges.

### Metamorphic Testing for Software Quality Assessment: A Study of Search Engines

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/7254235)

**Abstract:** Metamorphic testing is a testing technique that can be used to verify the functional correctness of software in the absence of an ideal oracle. This paper extends metamorphic testing into a user-oriented approach to software verification, validation, and quality assessment, and conducts large scale empirical studies with four major web search engines: Google, Bing, Chinese Bing, and Baidu. These search engines are very difficult to test and assess using conventional approaches owing to the lack of an objective and generally recognized oracle. The results are useful for both search engine developers and users, and demonstrate that our approach can effectively alleviate the oracle problem and challenges surrounding a lack of specifications when verifying, validating, and evaluating large and complex software systems.

## TSE 2013

### How Effectively Does Metamorphic Testing Alleviate the Oracle Problem?

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/6613484)

**Abstract:** In software testing, something which can verify the correctness of test case execution results is called an oracle. The oracle problem occurs when either an oracle does not exist, or exists but is too expensive to be used. Metamorphic testing is a testing approach which uses metamorphic relations, properties of the software under test represented in the form of relations among inputs and outputs of multiple executions, to help verify the correctness of a program. This paper presents new empirical evidence to support this approach, which has been used to alleviate the oracle problem in various applications and to enhance several software analysis and testing techniques. It has been observed that identification of a sufficient number of appropriate metamorphic relations for testing, even by inexperienced testers, was possible with a very small amount of training. Furthermore, the cost-effectiveness of the approach could be enhanced through the use of more diverse metamorphic relations. The empirical studies presented in this paper clearly show that a small number of diverse metamorphic relations, even those identified in an ad hoc manner, had a similar fault-detection capability to a test oracle, and could thus effectively help alleviate the oracle problem.
