# Unveiling Hidden DNN Defects with Decision-Based Metamorphic Testing

* <img src="../../icons/pdf.png" width="24px">[Paper](./Unveiling_Hidden_DNN_Defects_with_Decision-Based_Metamorphic_Testing.pdf)

**Abstract:** Contemporary DNN testing works are frequently conducted using metamorphic testing (MT). In general, de facto MT frameworks mutate DNN input images using semantics-preserving mutations and determine if DNNs can yield consistent predictions. Nevertheless, we find that DNNs may rely on erroneous decisions (certain components on the DNN inputs) to make predictions, which may still retain the outputs by chance. Such DNN defects would be neglected by existing MT frameworks. Erroneous decisions, however, would likely result in successive mis-predictions over diverse images that may exist in real-life scenarios.

This research aims to unveil the pervasiveness of hidden DNN defects caused by incorrect DNN decisions (but retaining consistent DNN predictions). To do so, we tailor and optimize modern eXplainable AI (XAI) techniques to identify visual concepts that represent regions in an input image upon which the DNN makes predictions. Then, we extend existing MT-based DNN testing frameworks to check the consistency of DNN decisions made over a test input and its mutated inputs. Our evaluation shows that existing MT frameworks are oblivious to a considerable number of DNN defects caused by erroneous decisions. We conduct human evaluations to justify the validity of our findings and to elucidate their characteristics. Through the lens of DNN decision-based metamorphic relations, we re-examine the effectiveness of metamorphic transformations proposed by existing MT frameworks. We summarize lessons from this study, which can provide insights and guidelines for future DNN testing.

[Back](../../README.md)