# ESEC/FSE

[Back](../README.md#all-papers)

## FSE 2024

### Abstraction-Aware Inference of Metamorphic Relations

* <img src="../icons/pdf.png" width="24px">[Paper](https://mpapad.github.io/publications/pdfs/metamorphic_relation_inference.pdf)

**Abstract:** Metamorphic testing is a valuable technique that helps in dealing with the oracle problem. It involves testing software against specifications of its intended behavior given in terms of so called metamorphic relations, statements that express properties relating different software elements (e.g., different inputs, methods, etc). The effective application of metamorphic testing strongly depends on identifying suitable domain-specific metamorphic relations, a challenging task, that is typically manually performed.

This paper introduces MemoRIA, a novel approach that aims at automatically identifying metamorphic relations. The technique focuses on a particular kind of metamorphic relation, which asserts equivalences between methods and method sequences. MemoRIA works by first generating an object-protocol abstraction of the software being tested, then using fuzzing to produce candidate relations from the abstraction, and finally validating the candidate relations through run-time analysis. A SAT-based analysis is used to eliminate redundant relations, resulting in a concise set of metamorphic relations for the software under test. We evaluate our technique on a benchmark consisting of 22 Java subjects taken from the literature, and compare MemoRIA with the metamorphic relation inference technique SBES. Our results show that by incorporating the object protocol abstraction information, MemoRIA is able to more effectively infer meaningful metamorphic relations, that are also more precise, compared to SBES, measured in terms of mutation analysis. Also, the SAT-based reduction allows us to significantly reduce the number of reported metamorphic relations, while in general having a small impact in the bug finding ability of the corresponding obtained relations.

### A Miss Is as Good as A Mile: Metamorphic Testing for Deep Learning Operators

### Metamorphic Testing of Secure Multi-Party Computation (MPC) Compilers

## FSE 2021

### Generating Metamorphic Relations for Cyber-physical Systems with Genetic Programming: An Industrial Case Study

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3468264.3473920)

**Abstract:** One of the major challenges in the verification of complex industrial Cyber-Physical Systems is the difficulty of determining whether a particular system output or behaviour is correct or not, the so-called test oracle problem. Metamorphic testing alleviates the oracle problem by reasoning on the relations that are expected to hold among multiple executions of the system under test, which are known as Metamorphic Relations (MRs). However, the development of effective MRs is often challenging and requires the involvement of domain experts. In this paper, we present a case study aiming at automating this process. To this end, we implemented GAssertMRs, a tool to automatically generate MRs with genetic programming. We assess the cost-effectiveness of this tool in the context of an industrial case study from the elevation domain. Our experimental results show that in most cases GAssertMRs outperforms the other baselines, including manually generated MRs developed with the help of domain experts. We then describe the lessons learned from our experiments and we outline the future work for the adoption of this technique by industrial practitioners.

### New Visions on Metamorphic Testing after a Quarter of a Century of Inception

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3468264.3473136)

**Abstract:** Metamorphic testing (MT) was introduced about a quarter of a century ago. It is increasingly being accepted by researchers and the industry as a useful testing technique. The studies, research results, applications, and extensions of MT have given us many insights and visions for its future. Our visions include: MRs will be a practical means to top up test case generation techniques, beyond the alleviation of the test oracle problem; MT will not only be a standalone technique, but conveniently integrated with other methods; MT and MRs will evolve beyond software testing, or even beyond verification; MRs may be anything that you can imagine, beyond the necessary properties of algorithms; MT research will be beyond empirical studies and move toward a theoretical foundation; MT will not only bring new concepts to software testing but also new concepts to other disciplines; MRs will alleviate the reliable test set problem beyond traditional approaches. These visions may help researchers explore the challenges and opportunities for MT in the next decade.

### Metamorphic Testing of Datalog Engines

* <img src="../icons/pdf.png" width="24px">[Paper](https://dl.acm.org/doi/abs/10.1145/3468264.3468573)

**Abstract:** Datalog is a popular query language with applications in several domains. Like any complex piece of software, Datalog engines may contain bugs. The most critical ones manifest as incorrect results when evaluating queries—we refer to these as query bugs. Given the wide applicability of the language, query bugs may have detrimental consequences, for instance, by compromising the soundness of a program analysis that is implemented and formalized in Datalog. In this paper, we present the first metamorphic-testing approach for detecting query bugs in Datalog engines. We ran our tool on three mature engines and found 13 previously unknown query bugs, some of which are deep and revealed critical semantic issues.