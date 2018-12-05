
Paper list and downloadable links can be found here 
----------------------------------------------------------------------------

https://dblp.org/db/conf/mm/mm2018.html

https://dl.acm.org/citation.cfm?id=3240508&picked=prox


[1] Style Separation and Synthesis via Generative Adversarial Networks
----------------------------------------------------------------------------

Style synthesis attracts great interests recently, while few works focus on its dual problem “style separation”. In this paper, we propose the Style Separation and Synthesis Generative Adversarial Network (S3  -GAN) to simultaneously implement style separation and style synthesis on object photographs of specific categories. Based on the assumption that the object photographs lie on a manifold, and the contents and styles are independent, we employ S3 -GAN to build mappings between the manifold and a latent vector space for separating and synthesizing the contents and styles. The S3 -GAN consists of an encoder network, a generator network, and an adversarialnetwork. The encoder network performs style separation by mapping an object photograph to a latent vector. Two halves of the latent vector represent the content and style, respectively. The generator network performs style synthesis by taking a concatenated vector as input. The concatenated vector contains the style half vector of the style target image and the content half vectorof the content target image. Once obtaining the images from the generator network, an adversarial network is imposed to generate  more photo-realistic images. Experiments on CelebA and UT Zappos 50K datasets demonstrate that the S3 -GAN has the capacity of style separation and synthesis simultaneously, and could capture various styles in a single model.

[2] Learning to Transfer: Generalizable Attribute Learning with Multitask Neural Model Search
-------------------------------------------------------------------------------------------------

As attribute leaning brings mid-level semantic properties for objects, it can benefit many traditional learning problems in multimedia  and computer vision communities. When facing the huge  number of attributes, it is extremely challenging to automatically  design a generalizable neural network for other attribute learning tasks. Even for a specific attribute domain, the exploration of the  neural network architecture is always optimized by a combination of heuristics and grid search, from which there is a large space of possible choices to be searched. In this paper, Generalizable Attribute Learning Model (GALM) is proposed to automatically design the neural networks for generalizable attribute learning. The main novelty of GALM is that it fully exploits the Multi-Task Learning and Reinforcement Learning to speed up the search procedure. With the help of parameter sharing, GALM is able to transfer the pre-searched architecture to different attribute domains. In experiments, we comprehensively evaluate GALM on 251 attributes from three domains: animals, objects, and scenes. Extensive experimental results demonstrate that GALM significantly outperforms the state-of-the-art attribute learning approaches and previous neural architecture search methods on two generalizable attribute learning scenarios.

[3] Supervised Online Hashing via Hadamard Codebook Learning
-------------------------------------------------------------------------------------------------

-- "However, most existing hashing methods adopted oine batch learning, which is not suitable to handle incremental datasets with streaming data or new instances. In contrast, the robustness of the existing online hashing remains as an  open problem, while the embedding of supervised/semantic information hardly boosts the performance of the online hashing, mainly due to the defect of unknown category numbers in supervised learning."  

-- an online hashing scheme where an new incoming class training data can be used to learn the new class projections without adversably affecting the old class projections 

-- this is a non-deep method which uses the concept of codebook and updates the codebook to take care of the new classes (another interpretation will be like have a dictionary of atoms with group sparsity where each group denotes some classes, and then add another group to take care of the new classes)

[4] Pseudo Transfer with Marginalized Corrupted Attribute for Zero-shot Learning
-------------------------------------------------------------------------------------------------

-- Zero-shot learning (ZSL) aims to recognize unseen classes that are excluded from training classes. ZSL suffers from 1) Zero-shot bias  (Z-Bias) — model is biased towards seen classes because unseen data is inaccessible for training; 2) Zero-shot variance (Z-Variance)   — associating different images to same semantic embedding yields large associating error. To reduce Z-Bias, we propose a pseudo transfer mechanism, where we first synthesize the distribution of unseen data using semantic embeddings, then we minimize the mismatch between the seen distribution and the synthesized unseen distribution. To reduce Z-Variance, we implicitly corrupted  one semantic embedding multiple times to generate image-wise semantic vectors, with which our model learn robust classifers. Lastly, we integrate our Z-Bias and Z-variance reduction techniques with a linear ZSL model to show its usefulness. Our proposed model successfully overcomes the Z-bias and Z-variance problems. Extensive experiments on five benchmark datasets including ImageNet1Kdemonstrate that our model outperforms the state-of-the-art methods with fast training. 

-- read about Z bias and Z variance 

-- they are intentionally corrupting the attributes ? nice idea i think ... but how to corrupt it in such a way that it does not by mistake translate to another attribute of another class ... how can we guarantee that the corrupted attribute will not match with one of the unseen category attributes ?


[5] Webly Supervised Joint Embedding for Cross-Modal Image-Text Retrieval
-------------------------------------------------------------------------------------------------

-- a two stage process where initially the embeddings are learned using the clean data and in the next stage they use webly supervised data (basically data collected from Web Flickr ... the data might be noisy)

-- so they use a lower learning rate and also to pick suitable examples to learn from they use something called curriculum learning 
... what is that ? refer to this paper ... https://ronan.collobert.com/pub/matos/2009_curriculum_icml.pdf bengio

-- can the inverse of curriculum learning be used for novelty detection work ? basically the network will learn which examples to not look into because they look pretty similar to the ones already trained ones ? can that be used to define most similar and not-similar examples ?

[6] Dissimilarity Representation Learning for Generalized Zero-Shot Re cognition
-------------------------------------------------------------------------------------------------

-- Generalize d zero-shot learning (GZSL) aims to re cognize any test instance coming either from a known class or from a novel class  that has no training instance. To synthesize training instances for novel classes and thus resolving GZSL as a common classifiation problem, we prop ose a Dissimilarity Representation Learning (DSS) metho d. Dissimilarity representation is to represent a sp ecifi instance in terms of its (dis)similarity to other instances in a visual or attribute base d feature space. In the dissimilarity space, instances of the novel classes are synthesize d by an end-to-end optimize d neural network. The neural network realizes two-level feature mappings and domain adaptions in the dissimilarity space and the attribute base d feature space. Exp erimental results on fieb enchmark datasets, i.e., AWA, AWA2, SUN, CUB, and aPY, show that the proposed method improves the state-of-the-art with a large margin, approximately 10% gain in terms of the harmonic mean of the top-1 accuracy. Consequently, this paper establishes a new baseline for GZSL

-- a dissimilarity metric which basically is the distance of a data from each class attribute or mean vectors ... they have used this information to improve their results.

-- paper is written in a bad way ... very undreadable

[7] Dense Auto-Encoder Hashing for Robust Cross-Modality Retrieval
-------------------------------------------------------------------------------------------------

-- Cross-modality retrieval has been widely studied, which aims to search images as response to text queries or vice versa. When faced with large-scale dataset, cross-modality hashing serves as  an efficient and effective solution, which learns binary codes to  approximate the cross-modality similarity in the Hamming space. Most recent cross-modality hashing schemes focus on learning the hash functions from data instances with fully modalities. However, how to learn robust binary codes when facing incomplete modality (i.e., with one modality missed or partially observed), is left unexploited,which however widely occurs in real-world applications. In this paper, we propose a novel cross-modality hashing, termed Dense Auto-encoder Hashing (DAH), which can explicitly imputethe missed modality and produce robust binary codes by leveraging the relatedness among different modalities. To that effect, we propose a novel Dense Auto-encoder Network (DAN) to imputethe missing modalities, which densely connects each layer to every other layer in a feed-forward fashion. For each layer, a noisy auto-encoder block is designed to calculate the residue between the current prediction and original data. Finally, a hash-layer is added to the end of DAN, which serves as a special binary encoder model to deal with the incomplete modality input. Quantitative experiments on three cross-modality visual search benchmarks have shown that the proposed DAH has superior performance over thestate-of-the-art approaches.  

-- missing modality problem is also handled   

-- they have used a autoencoder formulation is a residual fashion 

-- paper is quite promising 

[8] Post Tuned Hashing: A New Approach to Indexing High-dimensional Data
----------------------------------------------------------------------------

-- Learning to hash has proven to be an effective solution for indexing high-dimensional data by projecting them to similarity-preserving binary codes. However, most existing methods end up the learning scheme with a binarization stage, i.e., binary quantization, which inevitably destroys the  neighborhood structure of original data. As a result, those methods still suffer from great similarity loss and result in unsatisfactory indexing performance. In this paper we propose a novel hashing model, namely Post Tuned Hashing (PTH),  which includes a new post-tuning stage to refine the binary  codes after binarization. The post-tuning seeks to rebuild the destroyed neighborhood structure, and hence significantly  improves the indexing performance. We cast the post-tuninginto a binary quadratic optimization framework and, despite its NP-hardness, give a practical algorithm to efficiently obtain a high-quality solution. Experimental results on five noted image benchmarks show that our PTH improves previous state-of-the-art methods by 13-58% in mean average precision 1

-- a new exciting way to decrease the error of neighborhood preservation ... this is a post processing step which can be utilized with any baseline models

-- shows significant improvements to the results









