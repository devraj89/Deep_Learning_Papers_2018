ICLR 2018
--------------

ICML 2018
--------------

NIPS 2018
--------------

[1] Memory Replay GANs: learning to generate images from new categories without forgetting
------------------------------------------------------------------------------------------

http://papers.nips.cc/paper/7836-memory-replay-gans-learning-to-generate-new-categories-without-forgetting.pdf

-- learn two generate new categories without forgetting

-- potentially solving the problem of incremental learning 

-- possible extensions to few shot learning/ zero shot learning / etc

[2] Generalized Zero-Shot Learning with Deep Calibration Network
------------------------------------------------------------------------------------------

http://papers.nips.cc/paper/7471-generalized-zero-shot-learning-with-deep-calibration-network.pdf

-- uses entropy but they require to know the category names of the unseen categories during the training itself

-- entropy used during training (in our case it is different)

[3] Out-of-Distribution Detection using Multiple Semantic Label Representations
------------------------------------------------------------------------------------------

http://papers.nips.cc/paper/7967-out-of-distribution-detection-using-multiple-semantic-label-representations.pdf

[4] Co-teaching: Robust Training of Deep Neural Networks with Extremely Noisy Labels
------------------------------------------------------------------------------------------

http://papers.nips.cc/paper/8072-co-teaching-robust-training-of-deep-neural-networks-with-extremely-noisy-labels.pdf

https://github.com/bhanML/Co-teaching

-- an interesting paper to deal with noises in labels 

-- basically two networks .. select in a mini-batch which label prediction losses are poorer and then cross-use them to update the parameters of the network

-- might be useful for our own work

[5] Masking: A New Perspective of Noisy Supervision
------------------------------------------------------------------------------------------

https://papers.nips.cc/paper/7825-masking-a-new-perspective-of-noisy-supervision.pdf

-- an interesting idea so that we can ensure some structure in the weight matrix / channel layer

-- how they determine the mask ? -- can we use word2vec between the categories to do that ?

[6] To Trust Or Not To Trust A Classifier
------------------------------------------------------------------------------------------

http://papers.nips.cc/paper/7798-to-trust-or-not-to-trust-a-classifier.pdf

-- an interesting problem to check whether to trust or not trust the classifier 

-- check the concept of trust score 

-- code available here at :: https://github.com/google/TrustScore

-- a metric to replace entropy?


[7] ∆-encoder: an effective sample synthesis method for few-shot object recognition
------------------------------------------------------------------------------------------

http://papers.nips.cc/paper/7549-delta-encoder-an-effective-sample-synthesis-method-for-few-shot-object-recognition.pdf

-- discussed by sivaram an exciting work in few shot learning that tries to mimic the variations in the given classes and uses the learned variations to augment the few shot example data


[8] Maximum Entropy Fine-Grained Classification
------------------------------------------------------------------------------------------

http://papers.nips.cc/paper/7344-maximum-entropy-fine-grained-classification.pdf

-- uses entropy to basically say that for fine grained classifications it is better that the network is not too confident 

-- shown to be an effective fine-tuning mechanism with lot of improvements observed over the generic baseline results even on tough datasets such as CUB

[9] Generalized Cross Entropy Loss for Training Deep Neural Networks with Noisy Labels
------------------------------------------------------------------------------------------

https://papers.nips.cc/paper/8094-generalized-cross-entropy-loss-for-training-deep-neural-networks-with-noisy-labels.pdf

https://nips.cc/media/Slides/nips/2018/220e(06-15-30)-06-16-55-12761-Generalized_Cro.pdf

-- discusses the concept of symmetric loss functions and why MAE is better than CCE for the noisy labeled samples (refers to sastry sir's AAAI 2018 paper)

-- CCE converges fast but overfits to noise whereas MAE converges very very slow (often does not reach the performance of the CCE but is much more robust to the noisy labels) This is the reason why the authors tried to tread a middle ground here.

-- defines a new loss function called box function and truncated function to deal with the above problems 

[10] Using Trusted Data to Train Deep Networks on Labels Corrupted by Severe Noise
------------------------------------------------------------------------------------------

http://papers.nips.cc/paper/8246-using-trusted-data-to-train-deep-networks-on-labels-corrupted-by-severe-noise.pdf

https://github.com/mmazeika

-- a paper which uses a small set of gold standard (or basically cleaned data) to clean other sample labels under severe noise conditions

-- this work uses a new property that given the noisy labels and the clean labels both are conditionally indepenedent of each other provided the original data ... or in other words the noisy label is not dependent on the clean label but rather on the data sample itself.

-- from the paper "The conditional independence assumption is reasonable, as it is usually the case that noisy labeling processes do not have access to the true label." This actually makes a lot of sense.

-- very good results but you do need the set of trusted labels

[11] Dual Swap Disentangling
------------------------------------------------------------------------------------------

http://papers.nips.cc/paper/7830-dual-swap-disentangling.pdf

-- a nice idea using autoencoders to disentangle representations

-- also used to incorporate both the labeled and unlabeled samples 

-- the best idea is about the swapping of the latent factors








