
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
 - generally as a network is trained the updates become less frequent as convergence is occuring 
 - so in case of noisy labels the updates will occur beacuse some examples are marked wrong and the classifier is forcibly trying to make it to the noisy label target
 - "On the other hand, in the presence of noisy labels, as the classifier improves the effect of the noise increases - the classifier may give correct predictions, but will still have to update due to wrong labeling."
 - "Thus, in an advanced stage of the training process the majority of the updates may actually be due to wrongly labeled examples, and therefore will not allow the classifier to further improve."
 - <when to update> <--> <how to update>  DONT DEPEND ON THE LABELS DURING CONVERGENCE
 - train two networks and update only when disagreements occur between them (the two networks can be trained initially like normal but possibly on a different subsets of the training data)
 - INTUITION: during network convergence if both the networks are predicting some labels and IT DOES NOT MATCH WITH THE TARGET LABEL, the target label is possibly wrong 
 - paper: https://papers.nips.cc/paper/6697-decoupling-when-to-update-from-how-to-update.pdf
 - code: https://github.com/emalach/UpdateByDisagreement
 
 
