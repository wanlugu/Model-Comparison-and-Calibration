"# Model Calibration" 
Model calibration is important only if you care about the probabilities your model computes. In the case of comparing and picking from two models, level of confidence of the prediction makes models different. If the two models both return probability of the prediction, then there is no need to carlibrate.

However, if you are building a mission-critical application, which computes the probability of a person being sick, the actual probability value is significant. If, for example, your model is not that confident for a specific patient, a human doctor should certainly know about it and act accordingly.

There are also other cases where model calibration is useful:
Debugging: we want to know when our model is wrong with high confidence or assigns a low probability to the correct class
Ensembles: if we want to combine many probability models, having accurate predictions makes a difference
