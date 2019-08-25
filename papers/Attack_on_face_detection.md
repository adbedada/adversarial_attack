# [Accessorize to a Crime: Real and Stealthy Attacks on State-of-the-Art Face Recognition](https://www.cs.cmu.edu/~sbhagava/papers/face-rec-ccs16.pdf)


#### Key Points
The paper presents the effectiveness of "physically realizable and inconspicuous" attacks on face detection (FD) and face recognition (FR) systems. The researchers used eyeglass frames to fool FR systems.

Previous related work include:
 
- Covering with Makeup and hair style to evade FD systems
- 3d printed masks to evade FR -- can be mitgated by liveness detection
- Model inversion attacks -- can be solved via anti-spoofing mechanisms

The ML model tested for attack is Parkhi et al's 39 - Layer DNN that achieved the state-of-the-art performance on the Labled Faces in the Wild (LFW) challenge.

The researchers created two types of attacks.

1) Impersination 
2) Dodgning

Both attacks are done by optimizing  a softmaxloss function that gets lower if the FR detected correctly and vise versa. The success rate of these attacks ranges from 91.67 to 100% . 
