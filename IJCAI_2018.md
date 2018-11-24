Interesting Papers
------------------

[1] Dual Adversarial Networks for Zero-shot Cross-media Retrieval
-------------------------------------------------------------------

https://www.ijcai.org/proceedings/2018/0092.pdf

-- Existing cross-media retrieval methods usually require that testing categories remain the same with training categories, which cannot support the retrieval  of increasing new categories. Inspired by zero-shot learning, this paper proposes zeroshot cross-media retrieval for addressing the above problem, which aims to retrieve data of new categories across different media types. It is challenging that zero-shot cross-media retrieval has to handle not only the inconsistent semantics across new and known categories, but also the heterogeneous distributions across different media types. To address the above challenges, this paper proposes Dual Adversarial Networks for Zero-shot Crossmedia Retrieval (DANZCR), which is the first approach to address zero-shot cross-media retrieval to the best of our knowledge. Our DANZCR approach consists of two GANs in a dual structure for common representation generation and original representation reconstruction respectively, which capture the underlying data structures as well as strengthen relations between input data and semantic space to generalize across seen and unseen categories. Our DANZCR approach exploits word embeddings to learn common representations in semantic space via an adversarial learning method, which preserves the inherent cross-media correlation and enhances the knowledge transfer to new categories. Experiments on three widely-used cross-media retrieval datasets show the effectiveness of our approach.

[2] Visual Data Synthesis via GAN for Zero-Shot Video Classification
---------------------------------------------------------------------

https://www.ijcai.org/proceedings/2018/0157.pdf

-- using GANs for ZSL in zero shot

-- no analysis on GZSL protocol

[3] Adversarial Attribute-Image Person Re-identification

https://www.ijcai.org/proceedings/2018/0153.pdf

-- While attributes have been widely used for person re-identification (Re-ID) which aims at matching  the same person images across disjoint camera views, they are used either as extra features or for performing multi-task learning to assist the image-image matching task. However, how to find a set of person images according to a given attribute description, which is very practical in many surveillance applications, remains a rarely investigated cross-modality matching problem in person Re-ID. In this work, we present this challenge and leverage adversarial learning to formulate the attribute-image cross-modality person Re-ID model. By imposing a semantic consistency constraint across modalities as a regularization, the adversarial learning enables to generate imageanalogous concepts of query attributes for matching the corresponding images at both global level and semantic ID level. We conducted extensive experiments on three attribute datasets and demonstrated that the regularized adversarial modelling is so far the most effective method for the attributeimage cross-modality person Re-ID problem. 

-- much like the feature generating paper in CVPR 2018 

-- uses attributes to generate images 





