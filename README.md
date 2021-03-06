# Awesome Adversarial Machine Learning [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> This markdown file contains a paper colloction of adversarial machine learning. If you are confused about this domain or seeking a brief introduction, please check out wikipedia **[Adversarial Machine Learning](https://en.wikipedia.org/wiki/Adversarial_machine_learning)** . 


## Contents

- [Vision](#Vision)
- [Audio](#Audio)


## Vision

- [First Discovery] [L-BFGS]  **Intriguing properities of neural networks**, 2013, (Szegedy et al.) [ [paper](https://arxiv.org/abs/1312.6199) ]
> Contribution: In this paper, the author first noticed the existence of *adversarial examples* in image classification application.

## Audio

- \[First Discovery\] **Cocaine Noodles: Exploiting the gap between human and machine speech recognition, USENIX Security 2015**, (Vaidya et al.)
> Contribution: this paper found adversrial examples against ASR systems, they showed an input signal can be modified to fit the transcription by considering the features instead of the output of DNN. 
> Problem: their adversarial examples show a high distortion of the original data and human can easily perceive the attack.

- **Hidden voice commands, UNSENIX Security 2016**, (Carlini et al.)
> Contribution: this paper demonstrated that targeted attacks against HMM-only ASR systems are feasible. 
> Problem: Even though the peturbation sounds like noise, it is still not indistinguishable by humans.

- \[ultra-sound based attacks\]\[DolphinAttacks\] **DolphinAttack: Inaudible voice commands, CCS 2017**, (Zhang et al.)
> Contribution: this paper shows that it is possible to hide a transcription by utilizing non-linearities of microphones to modulate the baseband audio signal with ultrasound higher than 20 kHz, human can only hear sounds in 20Hz~20kHz. 
> Problem: such attacks are costy as the attack is based on specific microphone.

- [ultra-sound based attacks] **BackDoor: Making microphones hear inaudible sounds, MSAS 2017**

- [ultra-sound based attacks] **Inaudible voice commands, 2017**

- [CTC loss] **Audio adversarial examples: Targeted attacks on Speech-to-Text, 2018**, (Carlini and Wagner)
> Contribution: this paper proposed a general targeted attack using connectionist temporal classification loss, similar to vision problems, this attack replace the loss function with CTC loss, which is optimized for time-sequences. 
> Problem: Distance metrics borrowed from vision problems, does not consider the sensitivities and limits of human auditory perception.

- [psychoacoustic hiding] **Adversarial Attacks Against Automatic Speech Recognition Systems via Psychoacoustic Hiding, 2019**, (Schönherr et al.)
> Contribution


## Introduction and Analysis

*  Adversarial Machine Learning, 2011,  [ [paper](https://people.eecs.berkeley.edu/~tygar/papers/SML2/Adversarial_AISEC.pdf) ] 
*  Adversarial examples in the physical world 
* Exploring the space of adversarial images
* Analysis of classifiers’ robustness to adversarial perturbations
* Adversarial Examples Are Not Easily Detected: Bypassing Ten Detection Methods, Nicholas Carlini & David Wagner, [ [code](https://github.com/abhibhav14/adversarial-attacks-papernotes/blob/master/notes/carlini-wagner-bypass.md) ], [[paper](https://arxiv.org/abs/1705.07263)]
* Analysis of classifiers' robustness to adversarial perturbations, Machine Learning , [  [paper](https://link.springer.com/article/10.1007%2Fs10994-017-5663-3)]
* Adversarial Machine Learning at Scale, **ICLR 2017**,[ [paper](https://openreview.net/forum?id=BJm4T4Kgx) ] 
* ADVERSARIAL EXAMPLES FOR GENERATIVE MODELS
* Transferability in Machine Learning: from Phenomena to Black-Box Attacks using Adversarial Samples
* The Space of Transferable Adversarial Examples
* Adversarial Examples that Fool both Human and Computer Vision 
* **taxonomy of adversaries against DNN classifers?** : The Limitations of Deep Learning in Adversarial Settings [ [paper](https://arxiv.org/abs/1511.07528) ]
*  A Marauder’s Map of Security and Privacy in Machine Learning: An overview of current and future research directions for making machine learning secure and private, **AISec 2018**[[paper](https://export.arxiv.org/abs/1811.01134)]




## Survey

* Adversarial Examples: Attacks and Defenses for Deep Learning, 2018, [ [paper](https://arxiv.org/abs/1712.07107)  ], 
* Towards the Science of Security and Privacy in Machine Learning, Patrick McDaniel [cyw to read]
* Threat of Adversarial Attacks on Deep Learning in Computer Vision: A Survey ,  , 2018 ,CoRR, [ [paper](https://arxiv.org/abs/1801.00553) ]

## Attacks

In this category, the author usually luanch an attack to an classifier model, trained using CNN or other machine learning algorithms. A typical way to attack is to add some kind of small **noise** directly to the matrix (or image) and feed it into the target classifier, then get a different (false) classification result.

* **FGSM** : Explaining and Harnessing Adversarial Examples 
* **RAND + FGSM** : Practical Black-Box Attacks against Machine Learning 
* **CW-Attack** : Towards Evaluating the Robustness of Neural Networks, Nicholas Carlini & David Wagner, [  [paper](https://arxiv.org/abs/1608.04644) ]
* **Traffic Light** : Fooling Vision and Language Models Despite Localization and Attention Mechanism , **CVPR 2018**
* **Hack ICLR 2018** : Obfuscated Gradients Give a False Sense of Security : Circumventing Defenses to Adversarial Examples
* Deep neural networks are easily fooled: High confidence predictions for unrecognizable images
* Targeted Backdoor Attacks on Deep Learning Systems Using Data Poisoning, Chang Liu, [  [paper](https://arxiv.org/abs/1712.05526) ]
* Manipulating Machine Learning: Poisoning Attacks and Countermeasures for Regression Learning , **Oakland '18** ,Chang Liu, [  [paper](https://arxiv.org/pdf/1804.00308.pdf) ]
* Delving into Transferable Adversarial Examples and Black-box Attacks, **ICLR '17**,  [  [paper](https://arxiv.org/abs/1611.02770) ]
* Shielding Google's language toxicity model against adversarial attacks  , [ [paper](https://arxiv.org/abs/1801.01828) ]
* Generating Adversarial Examples with Adversarial Networks, **Dawn Song**, [ [paper](https://arxiv.org/abs/1801.02610) ]
* Spatially Transformed Adversarial Examples, **Dawn Song**, [ [paper](https://arxiv.org/abs/1801.02612)]
* Adversarial Deep Learning for Robust Detection of Binary Encoded Malware, [ [paper](https://arxiv.org/abs/1801.02950) ] 
* **Black box Attack** : Black-box Generation of Adversarial Text Sequences to Evade Deep Learning Classifiers, [ [paper](https://arxiv.org/abs/1801.04354)]
* **Black box Attack** : Delving into Transferable Adversarial Examples and Black-box Attacks
* **traffic sign** : Robust Physical-World Attacks on Deep Learning Models
* Adversarial Perturbations Against Deep Neural Networks for Malware Classific
* Automatically Evading Classifiers: A Case Study on PDF Malware Classifiers
* Defensive distillation is not robust to adversarial examples
* **R+FGSM** : Ensemble Adversarial Training: Attacks and Defenses [ [paper](https://arxiv.org/abs/1705.07204)] 
* **PGD** Towards Deep Learning Models Resistant to Adversarial Attacks 
* Adversarial Patch **NIPS 2017** : [ [paper](https://arxiv.org/abs/1712.09665) ]
* **Deepfool** Deepfool: a simple and accurate method tofool deep neural networks


###  Attacks to Face or Speech Recognition

In this category, the attacker focus on a face recognition system (like Face++), to make the classifier misclassify the input face or cannot detect faces.

* Accessorize to a Crime: Real and Stealthy Attacks on State-of-the-Art Face Recognition
* Invisible Mask: Practical Attacks on Face Recognition with Infrared
* Adversarial Generative Nets: Neural Network Attacks on State-of-the-Art Face Recognition ,   [ [paper](https://arxiv.org/abs/1801.00349) ]
* **Speech** : Did you hear that? Adversarial Examples Against Automatic Speech Recognition,  [ [paper](https://arxiv.org/abs/1801.00554) ]
* High Dimensional Spaces, Deep Learning and Adversarial Examples, [ [paper](https://arxiv.org/abs/1801.00634) ]
* **Speech** : * Audio Adversarial Examples: Targeted Attacks on Speech-to-Text, [ [paper](https://arxiv.org/abs/1801.01953) ] **white box, targeted attack, directed input**
* Adversarial Vulnerability of Neural Networks Increases With Input Dimension , [ [paper](https://arxiv.org/abs/1802.01421) ]
* **Speech** : DolphinAttack: Inaudible Voice Commands

### Attacks to Malware Detection

* Evading Classifiers by Morphing in the Dark, **black-box attack**
* Adversarial examples for malware detection
* Automated poisoning attacks and defenses in malware detection systems: An adversarial machine learning approach, 2018 , **Computers & Security**, [ [paper](https://www.sciencedirect.com/science/article/pii/S0167404817302444?via%3Dihub)]
* Adversarially Robust Malware Detection Using Monotonic Classification,CODASPY 2018, [ [paper](https://dl.acm.org/citation.cfm?doid=3180445.3180449) ]
* Adversarial Training Methods for Semi-Supervised Text Classification , **ICLR 2017**, [ [paper](https://openreview.net/forum?id=r1X3g2_xl) ]

## Defenses

In this category, some defensive techniques are proposed, the way to defense adversarial various and some typical defense method are listed:

- Detecting the adversarial examples
- Increase the robustness of the classifier (especially neural networks)
- Add pre-processing process before feed samples into the classifier
- etc.

Papers:

* Detecting Adversarial Examples in Deep Networks with Adaptive Noise Reduction, detecting, 2018
* SafetyNet: Detecting and Rejecting Adversarial Examples Robustly
* Improving the Robustness of Deep Neural Networks via Stability Training
* Efficient Defenses Against Adversarial Attacks
* Distillation as a Defense to Adversarial Perturbations Against Deep Neural Networks 
* MagNet: a Two-Pronged Defense against Adversarial Examples
* Hardening Deep Neural Networks via Adversarial Model Cascades, [ [paper](https://arxiv.org/abs/1802.01448) ] 
* On Detecting Adversarial Perturbations, **ICLR 2017**, [[paper](https://openreview.net/pdf?id=SJzCSf9xg)]
* **Defence** Mitigating adversarial effects through randomization **defend by randomly padding/resizing/perturbing (denoising)**
* Robust Linear Regression Against Training Data Poisoning, **AISec@CCS 17** , [ [paper](https://people.eecs.berkeley.edu/~liuchang/paper/aisec17-poisoning.pdf) ]

## Stealing Machine Learning Models

* Cracking Classifiers for Evasion: A Case Study on the Google’s Phishing Pages Filter
* Stealing Machine Learning Models via Prediction APIs, **USENIX 2016**


## Stealing Data


* **Stealing Training Data** : Model Inversion Attacks that Exploit Confidence Information and Basic Countermeasures, [ [paper](https://dl.acm.org/citation.cfm?doid=2810103.2813677) ]
* **Model Inversion Attack** : Membership Inference Attacks against Machine Learning Models [[paper](https://ieeexplore.ieee.org/document/7958568/)]
* **Use GAN to steal data** : Deep Models Under the GAN: Information Leakage from Collaborative Deep Learning， **published at CCS'17**
* Machine Learning Models that Remember Too Much, **CCS'17**


## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.


## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Jamie Cui has waived all copyright and
related or neighboring rights to this work.
