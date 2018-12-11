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















