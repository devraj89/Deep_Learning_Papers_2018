
This is a collection of Noisy Label Papers that I found to be useful.

I am specfically looking into papers that satisfies the following criterion !
-----------------------------------------------------------------------------


(1) no clean validation set available

(2) ease of implementation

[1] TRAINING DEEP NEURAL-NETWORKS USING A NOISE ADAPTATION LAYER [https://openreview.net/pdf?id=H12GRgcxg] [paper] () [chainer code] 
-----------------------------------------------------------------------------
 - A very nice paper which replaces the EM algorithm using two softmax layer and a channel layer which models the label confusion matrix sandwiched between them.
 - backpropagation available 
