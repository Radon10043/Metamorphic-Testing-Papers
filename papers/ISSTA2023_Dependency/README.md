# Dependency-Aware Metamorphic Testing of Datalog Engines

* <img src="../../icons/pdf.png" width="24px">[Paper](./Dependency-Aware_Metamorphic_Testing_of_Datalog_Engines.pdf)

**Abstract:** Datalog is a declarative query language with wide applicability, especially in program analysis. Queries are evaluated by Datalog engines, which are complex and thus prone to returning incorrect results. Such bugs, called query bugs, may compromise the soundness of upstream program analyzers, having potentially detrimental consequences in safety-critical settings.

To address this issue, we develop a metamorphic testing ap- proach for detecting query bugs in Datalog engines. In comparison to existing work, our approach is based on rich precedence information capturing dependencies among relations in the program. This enables much more general and effective metamorphic transformations. We implement our approach in DLSmith, which detected 16 previously unknown query bugs in four Datalog engines.

[Back](../../README.md)