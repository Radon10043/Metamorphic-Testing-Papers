# SANER

[Back](../README.md#all-papers)

## SANER 2025

### Can Large Language Models Discover Metamorphic Relations? A Large-Scale Empirical Study

* <img src="../icons/pdf.png" width="24px">Paper
* <img src="../icons/github.png" width="24px">[Code](https://github.com/Radon10043/Empirical-Study-LLM-MR)

**Abstract:** Software testing is a mainstream approach for software quality assurance. One fundamental challenge for testing is that in many practical situations, it is very difficult to verify the correctness of test results given inputs for Software Under Test (SUT), which is known as the oracle problem. Metamorphic Testing (MT) is a software testing technique that can effectively alleviate the oracle problem. The core component of MT is a set of Metamorphic Relations (MRs), which are basically the necessary properties of SUT, represented in the form of relationship among multiple inputs and their corresponding expected outputs. Different methods have been proposed to support the systematic MR identification. However, most of them still rely heavily on test engineers' understanding of the SUT and involve massive manual work.

Although a few preliminary studies have shown LLMs' viability in generating MRs, there does not exist a thorough and in-depth investigation on their capability in MR identification. We are thus motivated to conduct a comprehensive and large-scale empirical study to systematically evaluate the performance of LLMs in identifying appropriate MRs for a wide variety of software systems. This study makes use of 37 SUTs collected from previous MT studies. Prompts are constructed for two LLMs, gpt-3.5-turbo-1106 and gpt-4-1106-preview, to perform the MR identification for each SUT. The empirical results demonstrate that both LLMs can generate a large amount of MR candidates (MRCs). Among them, 29.86% and 43.79% of all MRCs are identified as the MRs valid for the corresponding SUT, respectively. In addition, 24.59% and 38.63% of all MRCs are MRs that had never been identified in previous studies. Our study not only reinforces LLM-based MR identification as a promising research direction for MT, but also provides some practical guidelines for how to further improve LLMs' performance in generating good MRs.