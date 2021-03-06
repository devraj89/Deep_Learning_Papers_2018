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
-------------------------------------------------------------------

https://www.ijcai.org/proceedings/2018/0153.pdf

-- While attributes have been widely used for person re-identification (Re-ID) which aims at matching  the same person images across disjoint camera views, they are used either as extra features or for performing multi-task learning to assist the image-image matching task. However, how to find a set of person images according to a given attribute description, which is very practical in many surveillance applications, remains a rarely investigated cross-modality matching problem in person Re-ID. In this work, we present this challenge and leverage adversarial learning to formulate the attribute-image cross-modality person Re-ID model. By imposing a semantic consistency constraint across modalities as a regularization, the adversarial learning enables to generate imageanalogous concepts of query attributes for matching the corresponding images at both global level and semantic ID level. We conducted extensive experiments on three attribute datasets and demonstrated that the regularized adversarial modelling is so far the most effective method for the attributeimage cross-modality person Re-ID problem. 

-- much like the feature generating paper in CVPR 2018 

-- uses attributes to generate images 

[4] Extracting Privileged Information from Untagged Corpora for Classifier Learning
-------------------------------------------------------------------

https://www.ijcai.org/proceedings/2018/0151.pdf

-- The performance of data-driven learning approaches is often unsatisfactory when the training data is inadequate either in quantity or quality. Manually labeled privileged information (PI), e.g., attributes, tags or properties, is usually incorporated to improve classifier learning. However, the process of manually labeling is time-consuming and labor-intensive. To address this issue, we propose to enhance classifier learning by extracting PI from untagged corpora, which can effectively eliminate the dependency on manually labeled data. In detail, we treat each selected PI as a subcategory and learn one classifier for per subcategory independently. The classifiers for all subcategories are then integrated together to form a more powerful category classifier. Particularly, we propose a new instance-level multi-instance learning (MIL) model to simultaneously select a subset of training images from each subcategory and learn the optimal classifiers based on the selected images. Extensive experiments demonstrate the superiority of our approach.

[5] Semantic Structure-based Unsupervised Deep Hashing
-------------------------------------------------------------------

https://www.ijcai.org/proceedings/2018/0148.pdf

-- Hashing is becoming increasingly popular for approximate nearest neighbor searching in massive databases due to its storage and search efficiency. Recent supervised hashing methods, which usually construct semantic similarity matrices to guide hash code learning using label information, have shown promising results. However, it is relativelydifficult to capture and utilize the semantic relationships between points in unsupervised settings. To address this problem, we propose a novel unsupervised deep framework called Semantic Structurebased unsupervised Deep Hashing (SSDH). We first empirically study the deep feature statistics, and find that the distribution of the cosine distance for point pairs can be estimated by two half Gaussian distributions. Based on this observation, we construct the semantic structure by considering points with distances obviously smaller than the others as semantically similar and points with distances obviously larger than the others as semantically dissimilar. We then design a deep architecture and a pair-wise loss function to preserve this semantic structure in Hamming space. Extensive experiments show that SSDH significantly outperforms current state-of-the-art methods.

-- uses the pre-trained network which are already trained in supervised fashion .. so kind of like cheating 

-- uses the statistics of the pre-trained network to determine semantic similarity and dis-similarity

[6] Tri-net for Semi-Supervised Deep Learning
----------------------------------------------

https://www.ijcai.org/proceedings/2018/0278.pdf

-- Deep neural networks have witnessed great successes in various real applications, but it requires a large number of labeled data for training. In this paper, we propose tri-net, a deep neural network which is able to use massive unlabeled data to help learning with limited labeled data. We consider model initialization, diversity augmentation and pseudo-label editing simultaneously. In our work, we utilize output smearing to initialize modules, use fine-tuning on labeled data to augment diversity and eliminate unstable pseudo-labels to alleviate the influence of suspicious pseudo-labeled data. Experiments show that our method achieves the best performance in comparison with state-ofthe-art semi-supervised deep learning methods. In particular, it achieves 8.30% error rate on CIFAR10 by using only 4000 labeled examples. 

[7] Unpaired Multi-Domain Image Generation via Regularized Conditional GANs
----------------------------------------------

https://www.ijcai.org/proceedings/2018/0354.pdf

-- In this paper, we study the problem of multidomain image generation, the goal of which is to generate pairs of corresponding images from different domains. With the recent development in generative  models, image generation has achieved great progress and has been applied to various computer vision tasks. However, multi-domain image generation may not achieve the desired performance due to the difficulty of learning the correspondence of different domain images, especially when the information of paired samples is not given. To tackle this problem, we propose Regularized Conditional GAN (RegCGAN) which is capable of learning to generate corresponding images in the absence of paired training data. RegCGAN is based on the conditional GAN, and we introduce two regularizers to guide the model to learn the corresponding semantics of different domains. We evaluate the proposed model on several tasks for which paired training data is not given, including the generation of edges and photos, the generation of faces with different attributes, etc. The experimental results show that our model can successfully generate corresponding images for all these tasks, while outperforms the baseline methods. We also introduce an approach of applying RegCGAN to unsupervised domain adaptation.

[8] Unsupervised Disentangled Representation Learning with Analogical Relations
---------------------------------------------------------------------------------

-- Learning the disentangled representation of interpretable generative factors of data is one of the foundations to allow artificial intelligence to think like people. In this paper, we propose the analogical training strategy for the unsupervised disentangled representation learning in generative models. The analogy is one of the typical cognitive processes, and our proposed strategy is based on the observationthat sample pairs in which one is different from the other in one specific generative factor show the same analogical relation. Thus, the generator is trained to generate sample pairs from which a designed classifier can identify the underlying analogical relation. In addition, we propose a disentanglement metric called the subspace score, which is inspired by subspace learning methods and does not require supervised information. Experiments show that our proposed training strategy allows the generative models to find the disentangled factors, and that our methods can give competitive performances as compared with the state-of-the-art methods.


[9] Adversarially Regularized Graph Autoencoder (ARGA)
------------------------------------------------------------

https://github.com/Ruiqi-Hu/ARGA

-- Graph embedding is an effective method to represent graph data in a low dimensional space for graph analytics. Most existing embedding algorithms typically focus on preserving the topological structure or minimizing the reconstruction errors of graph data, but they have mostly ignored the data distribution of the latent codes from the graphs, which often results in inferior embedding in realworld graph data. In this paper, we propose a novel adversarial graph embedding framework for graph data. The framework encodes the topological structure and node content in a graph to a compact representation, on which a decoder is trained to reconstruct the graph structure. Furthermore, the latent representation is enforced to match a prior distribution via an adversarial training scheme. To learn a robust embedding, two variants of adversarial approaches, adversarially regularized graph autoencoder (ARGA) and adversarially regularized variational graph autoencoder (ARVGA), are developed. Experimental studies on real-world graphs validate our design and demonstrate that our algorithms outperform baselines by a wide margin in link prediction, graph clustering, and graph visualization tasks. 


[10] Recommendation with Multi-Source Heterogeneous Information
------------------------------------------------------------------

https://www.ijcai.org/proceedings/2018/0469.pdf

-- Network embedding has been recently used in social network recommendations by embedding lowdimensional representations of network items for recommendation. However, existing item recommendation models in social networks suffer from two limitations. First, these models partially use item information and mostly ignore important contextual information in social networks such as textual content and social tag information. Second, network embedding and item recommendations are learned in two independent steps without any interaction. To this end, we in this paper consideritem recommendations based on heterogeneous information sources. Specifically, we combine item structure, textual content and tag information for recommendation. To model the multi-source heterogeneous information, we use two coupled neural networks to capture the deep network representations of items, based on which a new recommendation model Collaborative multi-source Deep Network Embedding (CDNE for short) is proposed to learn different latent representations. Experimental results on two real-world data sets demonstrate that CDNE can use network representation learning to boost the recommendation performance. 

[11] Aspect-Level Deep Collaborative Filtering via Heterogeneous Information Networks
------------------------------------------------------------------------------------------------------------------

https://www.ijcai.org/proceedings/2018/0471.pdf

-- Latent factor models have been widely used for recommendation. Most existing latent factor models  mainly utilize the rating information between users and items, although some recently extended modelsadd some auxiliary information to learn a unified latent factor between users and items. The unified latent factor only represents the latent features of users and items from the aspect of purchase history. However, the latent features of users and items may stem from different aspects, e.g., the brandaspect and category-aspect of items. In this paper, we propose a Neural network based Aspect-level Collaborative Filtering model (NeuACF) to exploit different aspect latent factors. Through modelling rich objects and relations in recommender system as a heterogeneous information network, NeuACF first extracts different aspect-level similarity matrices of users and items through different meta-paths and then feeds an elaborately designed deep neural network with these matrices to learn aspect-level latent factors. Finally, the aspect-level latent factors are effectively fused with an attention mechanism for the top-N recommendation. Extensive experiments on three real datasets show that NeuACF significantly outperforms both existing latent factor models and recent neural network models

[12] Tag-based Weakly-supervised Hashing for Image Retrieval
---------------------------------------------------------------

https://www.ijcai.org/proceedings/2018/0525.pdf

We are concerned with using user-tagged images to learn proper hashing functions for image retrieval.  The benefits are two-fold: (1) we could obtain abundant training data for deep hashing models; (2) tagging data possesses richer semantic information which could help better characterize similarity relationships between images. However, tagging data suffers from noises, vagueness and incompleteness. Different from previous unsupervised or supervised hashing learning, we propose a novel weakly-supervised deep hashing framework which consists of two stages: weakly-supervisedpre-training and supervised fine-tuning. The second stage is as usual. In the first stage, rather than performing supervision on tags, the framework introduces a semantic embedding vector (sem-vector) for each image and performs learning of hashing and sem-vectors jointly. By carefully designing the optimization problem, it can well leverage tagging information and image content for hashing learning. The framework is general and does not depend on specific deep hashing methods. Empirical resultson real world datasets show that when it is integrated with state-of-art deep hashing methods, the performance increases by 8-10%. 





