
This is a collection of Noisy Label Papers that I found to be useful.

I am specfically looking into papers that satisfies the following criterion !
-----------------------------------------------------------------------------


(1) no clean validation set available

(2) ease of implementation

[1] TRAINING DEEP NEURAL-NETWORKS USING A NOISE ADAPTATION LAYER ICLR 2017
-----------------------------------------------------------------------------
 - A very nice paper which replaces the EM algorithm using two softmax layer and a channel layer which models the label confusion matrix sandwiched between them.
 - backpropagation follows easily
 - paper: https://openreview.net/pdf?id=H12GRgcxg
 - code: https://github.com/udibr/noisy_labels 
 - pytorch code: managed to write it ourselves 
 
 
[2] Decoupling “when to update” from “how to update” NIPS 2017
----------------------------------------------------------------------------- 
