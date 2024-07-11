# ASE

[Back](../README.md#all-papers)

## ASE 2022

### ElecDaug: Electromagnetic Data Augmentation for Model Repair based on Metamorphic Relation

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3551349.3559536)
* <img src="../icons/github.png" width="24px">[Code](https://github.com/ehhhhjw/tool_ElecDaug)

**Abstract:** With the application of deep learning (DL) in signal detection, improving the robustness of classification models has received much attention, especially in automatic modulation classification (AMC) of electromagnetic signals. A large amount of electromagnetic signal data is required to obtain robust models in the training and testing process. However, the high cost of manual collection and the issue of low quality of automatically generated data contribute to the AMC model’s defects. Therefore, it is essential to generate electromagnetic data by data augmentation. In this paper, we propose a novel electromagnetic data augmentation tool, namely ElecDaug, which directs the metamorphic process by electromagnetic signal characteristics to achieve automatic data augmentation. Based on electromagnetic data pre-processing, transmission or time-frequency domains characteristic metamorphic, ElecDaug can augment the data samples to build robust AMC models. Preliminary experiments show that ElecDaug can effectively augment available data samples for model repair. The video is at https://youtu.be/x5g6IVX_Q3s. Documentation and source code can be found here: https://github.com/ehhhhjw/tool_ElecDaug.git.

### Unveiling Hidden DNN Defects with Decision-Based Metamorphic Testing

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3551349.3561157)

**Abstract:** Contemporary DNN testing works are frequently conducted using metamorphic testing (MT). In general, de facto MT frameworks mutate DNN input images using semantics-preserving mutations and determine if DNNs can yield consistent predictions. Nevertheless, we find that DNNs may rely on erroneous decisions (certain components on the DNN inputs) to make predictions, which may still retain the outputs by chance. Such DNN defects would be neglected by existing MT frameworks. Erroneous decisions, however, would likely result in successive mis-predictions over diverse images that may exist in real-life scenarios.

This research aims to unveil the pervasiveness of hidden DNN defects caused by incorrect DNN decisions (but retaining consistent DNN predictions). To do so, we tailor and optimize modern eXplainable AI (XAI) techniques to identify visual concepts that represent regions in an input image upon which the DNN makes predictions. Then, we extend existing MT-based DNN testing frameworks to check the consistency of DNN decisions made over a test input and its mutated inputs. Our evaluation shows that existing MT frameworks are oblivious to a considerable number of DNN defects caused by erroneous decisions. We conduct human evaluations to justify the validity of our findings and to elucidate their characteristics. Through the lens of DNN decision-based metamorphic relations, we re-examine the effectiveness of metamorphic transformations proposed by existing MT frameworks. We summarize lessons from this study, which can provide insights and guidelines for future DNN testing.

## ASE 2021

### Assessing Robustness of ML-Based Program Analysis Tools using Metamorphic Program Transformations

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/9678706)

**Abstract:** Metamorphic testing is a well-established testing technique that has been successfully applied in various domains, including testing deep learning models to assess their robustness against data noise or malicious input. Currently, metamorphic testing approaches for machine learning (ML) models focused on image processing and object recognition tasks. Hence, these approaches cannot be applied to ML targeting program analysis tasks. In this paper, we extend metamorphic testing approaches for ML models targeting software programs. We present LAMPION, a novel testing framework that applies (semantics preserving) metamorphic transformations on the test datasets. LAMPION produces new code snippets equivalent to the original test set but different in their identifiers or syntactic structure. We evaluate LAMPION against CodeBERT, a state-of-the-art ML model for Code-To-Text tasks that creates Javadoc summaries for given Java methods. Our results show that simple transformations significantly impact the target model behavior, providing additional information on the models reasoning apart from the classic performance metric.

### Metamorphic Testing on Multi-module UAV Systems

* <img src="../icons/pdf.png" width="24px">[Paper](https://ieeexplore.ieee.org/abstract/document/9678841/)

**Abstract:** Recent years have seen a rapid development of machine learning based multi-module unmanned aerial vehicle (UAV) systems. To address the oracle problem in autonomous systems, numerous studies have been conducted to use metamorphic testing to automatically generate test scenes for various modules, e.g., those in self-driving cars. However, as most of the studies are based on unit testing including end-to-end model-based testing, a similar testing approach may not be equally effective for UAV systems where multiple modules are working closely together. Therefore, in this paper, instead of unit testing, we propose a novel metamorphic system testing framework for UAV, named MSTU, to detect the defects in multi-module UAV systems. A preliminary evaluation plan to apply MSTU on an emerging autonomous multi-module UAV system is also presented to demonstrate the feasibility of the proposed testing framework.

## ASE 2020

### TestMC: Testing Model Counters using Differential and Metamorphic Testing

* <img src="../icons/pdf.png" width="24px">[Paper](TestMC: Testing Model Counters using Differential and Metamorphic Testing)

**Abstract:** Model counting is the problem for finding the number of solutions to a formula over a bounded universe. This is a classic problem in computer science that has seen many recent advances in techniques and tools that tackle it. These advances have led to applications of model counting in many domains, e.g., quantitative program analysis, reliability, and security. Given the sheer complexity of the underlying problem, today's model counters employ sophisticated algorithms and heuristics, which result in complex tools that must be heavily optimized. Therefore, establishing the correctness of implementations of model counters necessitates rigorous testing. This experience paper presents an empirical study on testing industrial strength model counters by applying the principles of differential and metamorphic testing together with bounded exhaustive input generation and input minimization. We embody these principles in the TestMC framework, and apply it to test four model counters, including three state-of-the-art model counters from three different classes. Specifically, we test the exact model counters projMC and dSharp, the probabilistic exact model counter Ganak, and the probabilistic approximate model counter ApproxMC. As subjects, we use three complementary test suites of input formulas. One suite consists of larger formulas that are derived from a wide range of real-world software design problems. The second suite consists of a bounded exhaustive set of small formulas that TestMC generated. The third suite consists of formulas generated using an off-the-shelf CNF fuzzer. TestMC found bugs in three of the four subject model counters. The bugs led to crashes, segmentation faults, incorrect model counts, and resource exhaustion by the solvers. Two of the tools were corrected subsequent to the bug reports we submitted based on our study, whereas the bugs we reported in the third tool were deemed by the tool authors to not require a fix.

### Metamorphic Object Insertion for Testing Object Detection Systems

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3324884.3416584)

**Abstract:** Recent advances in deep neural networks (DNNs) have led to object detectors (ODs) that can rapidly process pictures or videos, and recognize the objects that they contain. Despite the promising progress by industrial manufacturers such as Amazon and Google in commercializing deep learning-based ODs as a standard computer vision service, ODs --- similar to traditional software --- may still produce incorrect results. These errors, in turn, can lead to severe negative outcomes for the users. For instance, an autonomous driving system that fails to detect pedestrians can cause accidents or even fatalities. However, despite their importance, principled, systematic methods for testing ODs do not yet exist.

To fill this critical gap, we introduce the design and realization of MetaOD, a metamorphic testing system specifically designed for ODs to effectively uncover erroneous detection results. To this end, we (1) synthesize natural-looking images by inserting extra object instances into background images, and (2) design metamorphic conditions asserting the equivalence of OD results between the original and synthetic images after excluding the prediction results on the inserted objects. MetaOD is designed as a streamlined workflow that performs object extraction, selection, and insertion. We develop a set of practical techniques to realize an effective workflow, and generate diverse, natural-looking images for testing. Evaluated on four commercial OD services and four pretrained models provided by the TensorFlow API, MetaOD found tens of thousands of detection failures. To further demonstrate the practical usage of MetaOD, we use the synthetic images that cause erroneous detection results to retrain the model. Our results show that the model performance is significantly increased, from an mAP score of 9.3 to an mAP score of 10.5.

## ASE 2018

### DeepRoad: GAN-based Metamorphic Testing and Input Validation Framework for Autonomous Driving Systems

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3238147.3238187)

**Abstract:** While Deep Neural Networks (DNNs) have established the fundamentals of image-based autonomous driving systems, they may exhibit erroneous behaviors and cause fatal accidents. To address the safety issues in autonomous driving systems, a recent set of testing techniques have been designed to automatically generate artificial driving scenes to enrich test suite, e.g., generating new input images transformed from the original ones. However, these techniques are insufficient due to two limitations: first, many such synthetic images often lack diversity of driving scenes, and hence compromise the resulting efficacy and reliability. Second, for machine-learning-based systems, a mismatch between training and application domain can dramatically degrade system accuracy, such that it is necessary to validate inputs for improving system robustness.

In this paper, we propose DeepRoad, an unsupervised DNN-based framework for automatically testing the consistency of DNN-based autonomous driving systems and online validation. First, DeepRoad automatically synthesizes large amounts of diverse driving scenes without using image transformation rules (e.g. scale, shear and rotation). In particular, DeepRoad is able to produce driving scenes with various weather conditions (including those with rather extreme conditions) by applying Generative Adversarial Networks (GANs) along with the corresponding real-world weather scenes. Second, DeepRoad utilizes metamorphic testing techniques to check the consistency of such systems using synthetic images. Third, DeepRoad validates input images for DNN-based systems by measuring the distance of the input and training images using their VGGNet features. We implement DeepRoad to test three well-recognized DNN-based autonomous driving systems in Udacity self-driving car challenge. The experimental results demonstrate that DeepRoad can detect thousands of inconsistent behaviors for these systems, and effectively validate input images to potentially enhance the system robustness as well.

## ASE 2014

### Search-based Inference of Polynomial Metamorphic Relations

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/2642937.2642994)

**Abstract:** Metamorphic testing (MT) is an effective methodology for testing those so-called ``non-testable'' programs (e.g., scientific programs), where it is sometimes very difficult for testers to know whether the outputs are correct. In metamorphic testing, metamorphic relations (MRs) (which specify how particular changes to the input of the program under test would change the output) play an essential role. However, testers may typically have to obtain MRs manually.

In this paper, we propose a search-based approach to automatic inference of polynomial MRs for a program under test. In particular, we use a set of parameters to represent a particular class of MRs, which we refer to as polynomial MRs, and turn the problem of inferring MRs into a problem of searching for suitable values of the parameters. We then dynamically analyze multiple executions of the program, and use particle swarm optimization to solve the search problem. To improve the quality of inferred MRs, we further use MR filtering to remove some inferred MRs.

We also conducted three empirical studies to evaluate our approach using four scientific libraries (including 189 scientific functions). From our empirical results, our approach is able to infer many high-quality MRs in acceptable time (i.e., from 9.87 seconds to 1231.16 seconds), which are effective in detecting faults with no false detection.