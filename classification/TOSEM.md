# TOSEM

[Back](../README.md#all-papers)

## TOSEM 2024

### MR-Scout: Automated Synthesis of Metamorphic Relations from Existing Test Cases

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3656340)

**Abstract:** Metamorphic Testing (MT) alleviates the oracle problem by defining oracles based on metamorphic relations (MRs) that govern multiple related inputs and their outputs. However, designing MRs is challenging, as it requires domain-specific knowledge. This hinders the widespread adoption of MT. We observe that developer-written test cases can embed domain knowledge that encodes MRs. Such encoded MRs could be synthesized for testing not only their original programs but also other programs that share similar functionalities.

In this article, we propose MR-Scout to automatically synthesize MRs from test cases in open-source software (OSS) projects. MR-Scout first discovers MR-encoded test cases (MTCs), and then synthesizes the encoded MRs into parameterized methods (called codified MRs), and filters out MRs that demonstrate poor quality for new test case generation. MR-Scout discovered over 11,000 MTCs from 701 OSS projects. Experimental results show that over 97% of codified MRs are of high quality for automated test case generation, demonstrating the practical applicability of MR-Scout. Furthermore, codified-MRs-based tests effectively enhance the test adequacy of programs with developer-written tests, leading to 13.52% and 9.42% increases in line coverage and mutation score, respectively. Our qualitative study shows that 55.76% to 76.92% of codified MRs are easily comprehensible for developers.

## TOSEM 2023

### Feedback-directed Metamorphic Testing

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3533314)

**Abstract:** Over the past decade, metamorphic testing has gained rapidly increasing attention from both academia and industry, particularly thanks to its high efficacy on revealing real-life software faults in a wide variety of application domains. On the basis of a set of metamorphic relations among multiple software inputs and their expected outputs, metamorphic testing not only provides a test case generation strategy by constructing new (or follow-up) test cases from some original (or source) test cases, but also a test result verification mechanism through checking the relationship between the outputs of source and follow-up test cases. Many efforts have been made to further improve the cost-effectiveness of metamorphic testing from different perspectives. Some studies attempted to identify “good” metamorphic relations, while other studies were focused on applying effective test case generation strategies especially for source test cases. In this article, we propose improving the cost-effectiveness of metamorphic testing by leveraging the feedback information obtained in the test execution process. Consequently, we develop a new approach, namely feedback-directed metamorphic testing, which makes use of test execution information to dynamically adjust the selection of metamorphic relations and selection of source test cases. We conduct an empirical study to evaluate the proposed approach based on four laboratory programs, one GNU program, and one industry program. The empirical results show that feedback-directed metamorphic testing can use fewer test cases and take less time than the traditional metamorphic testing for detecting the same number of faults. It is clearly demonstrated that the use of feedback information about test execution does help enhance the cost-effectiveness of metamorphic testing. Our work provides a new perspective to improve the efficacy and applicability of metamorphic testing as well as many other software testing techniques.