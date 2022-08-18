---
title: Publications
draft: false
publications:

  - title: How many perturbations break this model? Evaluating robustness beyond adversarial accuracy
    authors: Raphael Olivier, Bhiksha Raj
    url: https://arxiv.org/abs/2207.04129
    booktitle: ArXiv preprint
    abstract: >
      Robustness to adversarial attack is typically evaluated with adversarial accuracy. This metric quantifies the number of points for which, given a threat model, successful adversarial perturbations cannot be found. While essential, this metric does not capture all aspects of robustness and in particular leaves out the question of how many perturbations can be found for each point. In this work we introduce an alternative approach, adversarial sparsity, which quantifies how difficult it is to find a successful perturbation given both an input point and a constraint on the direction of the perturbation. This constraint may be angular (L2 perturbations), or based on the number of pixels (Linf perturbations).
      We show that sparsity provides valuable insight on neural networks in multiple ways. analyzing the sparsity of existing robust models illustrates important differences between them that accuracy analysis does not, and suggests approaches for improving their robustness. When applying broken defenses effective against weak attacks but not strong ones, sparsity can discriminate between the totally ineffective and the partially effective defenses. Finally, with sparsity we can measure increases in robustness that do not affect accuracy: we show for example that data augmentation can by itself increase adversarial robustness, without using adversarial training.
    bibtex: >
      @misc{Olivier22HM, doi = {10.48550/ARXIV.2207.04129}, url = {https://arxiv.org/abs/2207.04129}, author = {Olivier, Raphael and Raj, Bhiksha}, title = {How many perturbations break this model? Evaluating robustness beyond adversarial accuracy}, publisher = {arXiv}, year = {2022}, copyright = {arXiv.org perpetual, non-exclusive license}}
      
  - title: Recent improvements of ASR models in the face of adversarial attacks
    authors: Raphael Olivier, Bhiksha Raj
    url: https://arxiv.org/abs/2203.16536
    booktitle: InterSpeech 2022
    location: Incheon
    date: September 2022
    abstract: >
      Like many other tasks involving neural networks, Speech Recognition models are vulnerable to adversarial attacks. However recent research has pointed out differences between attacks and defenses on ASR models compared to image models. Improving the robustness of ASR models requires a paradigm shift from evaluating attacks on one or a few models to a systemic approach in evaluation. We lay the ground for such research by evaluating on various architectures a representative set of adversarial attacks: targeted and untargeted, optimization and speech processing-based, white-box, black-box and targeted attacks. Our results show that the relative strengths of different attack algorithms vary considerably when changing the model architecture, and that the results of some attacks are not to be blindly trusted. They also indicate that training choices such as self-supervised pretraining can significantly impact robustness by enabling transferable perturbations. We release our source code as a package that should help future research in evaluating their attacks and defenses. 
    bibtex: >
      @inproceedings{Olivier22RI, title = "Recent improvements of ASR models in the face of adversarial attacks", author = "Olivier Raphael  and Raj, Bhiksha", booktitle = "InterSpeech 2022", month = sep, year = "2022", address = "Incheon, South Korea", publisher = "ISCA"}

  - title: Sequential Randomized Smoothing for Adversarially Robust Speech Recognition
    authors: Raphael Olivier, Bhiksha Raj
    url: https://aclanthology.org/2021.emnlp-main.514/
    booktitle: Proceedings of the 2021 Conference on Empirical Methods in Natural Language Processing (EMNLP)
    location: Punta Cana
    date: November 2021
    abstract: >
      While Automatic Speech Recognition has been shown to be vulnerable to adversarial attacks, defenses against these attacks are still lagging. Existing, naive defenses can be partially broken with an adaptive attack. In classification tasks, the Randomized Smoothing paradigm has been shown to be effective at defending models. However, it is difficult to apply this paradigm to ASR tasks, due to their complexity and the sequential nature of their outputs. Our paper overcomes some of these challenges by leveraging speech-specific tools like enhancement and ROVER voting to design an ASR model that is robust to perturbations. We apply adaptive versions of state-of-the-art attacks, such as the Imperceptible ASR attack, to our model, and show that our strongest defense is robust to all attacks that use inaudible noise, and can only be broken with very high distortion.
    bibtex: >
      @inproceedings{Olivier21SR, title = "Sequential Randomized Smoothing for Adversarially Robust Speech Recognition", author = "Olivier Raphael  and Raj, Bhiksha", booktitle = "Proceedings of the 2021 Conference on Empirical Methods in Natural Language Processing", month = nov, year = "2021", address = "Punta Cana, Dominican Republic", publisher = "Association for Computational Linguistics"}

  - title: High-Frequency Adversarial Defense for Speech and Audio
    authors: Raphael Olivier, Muhammad Shah, Bhiksha Raj
    booktitle: 2021 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)
    url: https://ieeexplore.ieee.org/document/9414525
    location: Toronto
    date: June 2021
    abstract: >
      Recent work suggests that adversarial examples are enabled by high-frequency components in the dataset. In the speech domain where spectrograms are used extensively, masking those components seems like a sound direction for defenses against attacks. We explore a smoothing approach based on additive noise masking in priority high frequencies. We show that this approach is much more robust than the naive noise filtering approach, and a promising research direction. We successfully apply our defense on a Librispeech speaker identification task, and on the UrbanSound8K audio classification dataset.
    bibtex: >
      @inproceedings{Olivier21HF, author={Olivier, R. and Raj, B. and Shah, M.}, booktitle={IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},  title={High-Frequency Adversarial Defense for Speech and Audio},  year={2021}, volume={}, number={}, pages={2995-2999}, doi={10.1109/ICASSP39728.2021.9414525}}

  - title: Towards Adversarial Robustness Via Compact Feature Representations
    authors: Muhammad Shah, Raphael Olivier, Bhiksha Raj
    url: https://ieeexplore.ieee.org/document/9414696
    booktitle: 2021 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)
    location: Toronto
    date: June 2021
    abstract: >
      Deep Neural Networks (DNNs), while providing state-of-the-art performance in a wide variety of tasks, have been shown to be vulnerable to adversarial attacks. Recent studies have posited that this vulnerability arises because DNNs operate over a grossly overspecified input space with very sparse human supervision due to which they tend to learn spurious features that humans would ignore. These spurious features provide an attack vector for the adversary because perturbing these features would not alter the human’s decision but may alter the model’s prediction. In this paper we explore hypothesis that reducing the size of the model’s feature representation while maintaining its generalizability would discard spurious features while retaining perceptually relevant ones. We find that after the size of the feature representation has been reduced the models exhibit increased adversarial robustness, while suffering only a minimal loss in accuracy. In addition to being more robust, models with compact feature representations have the benefit of being more resource efficient.
    bibtex: >
      @inproceedings{Shah21TA, author={Shah, Muhammad A. and Olivier, Raphael and Raj, Bhiksha}, booktitle={IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},  title={Towards Adversarial Robustness Via Compact Feature Representations},  year={2021}, volume={}, number={}, pages={3845-3849}, doi={10.1109/ICASSP39728.2021.9414696}}

  - title: Exploiting Non-Linear Redundancy for Neural Model Compression
    authors: Muhammad Shah, Raphael Olivier, Bhiksha Raj
    url: https://arxiv.org/abs/2005.14070
    booktitle: 2020 25th International Conference on Pattern Recognition (ICPR)
    location: Milan
    date: January 2021
    abstract: >
      Deploying deep learning models, comprising of non-linear combination of millions, even billions, of parameters is challenging given the memory, power and compute constraints of the real world. This situation has led to research into model compression techniques most of which rely on suboptimal heuristics and do not consider the parameter redundancies due to linear dependence between neuron activations in overparametrized networks. In this paper, we propose a novel model compression approach based on exploitation of linear dependence, that compresses networks by elimination of entire neurons and redistribution of their activations over other neurons in a manner that is provably lossless while training. We combine this approach with an annealing algorithm that may be applied during training, or even on a trained model, and demonstrate, using popular datasets, that our method results in a reduction of up to 99\% in overall network size with small loss in performance. Furthermore, we provide theoretical results showing that in overparametrized, locally linear (ReLU) neural networks where redundant features exist, and with correct hyperparameter selection, our method is indeed able to capture and suppress those dependencies. 
    bibtex: >
      @inproceedings{Shah21EN, author={Shah, Muhammad A. and Olivier, Raphael and Raj, Bhiksha}, booktitle={25th International Conference on Pattern Recognition (ICPR)},  title={Exploiting Non-Linear Redundancy for Neural Model Compression},  year={2021}, volume={}, number={}, pages={9928-9935}, doi={10.1109/ICPR48806.2021.9413178}}

  - title: Optimal Strategies For Comparing Covariates To Solve Matching Problems
    authors: Muhammad Shah, Raphael Olivier, Bhiksha Raj
    url: https://ieeexplore.ieee.org/document/9412932
    booktitle: 2020 25th International Conference on Pattern Recognition (ICPR)
    location: Milan
    date: January 2021
    abstract: >
      Many machine learning tasks can be posed as matching problems in which we are given a “probe” entry that we expect matches some of the entries in our “gallery”. The general solution to these problems is to retrieve matching entries based on statistical dependencies between the probe and the gallery data that are learned using complex models. Often, however, there are other common covariates to the probe and gallery data which might be easily inferred and may explain some of the statistical dependencies between the two. In this paper we present a probabilistic framework to derive optimal matching strategies based only on covariate features for three broad tasks, namely N-way classification, pairwise verification and ranking. We use canonical metrics to determine the maximum performance that can be expected if only covariate features are used and determine the marginal gain of using complex models. We find that covariate matching achieves an EER within 10% of a CNN in the verification task, and an MAP within 22% of the a DNN based model in the ranking task.
    bibtex: >
      @INPROCEEDINGS{Shah20OS, author={Shah, Muhammad A. and Olivier, Raphael and Raj, Bhiksha}, booktitle={25th International Conference on Pattern Recognition (ICPR)}, title={Optimal Strategies For Comparing Covariates To Solve Matching Problems}, year={2021}, volume={}, number={}, pages={10622-10628}, doi={10.1109/ICPR48806.2021.9412932}}

  - title: Transfer Learning by Learning Projections from Target to Source
    authors: Antoine Cornuejols, Pierre-Alexandre Murena, Raphael Olivier
    url: https://link.springer.com/chapter/10.1007/978-3-030-44584-3_10
    booktitle: Advances in Intelligent Data Analysis XVIII (IDA)
    location: Konstanz
    date: April 2020
    abstract: >
      Using transfer learning to help in solving a new classification task where labeled data is scarce is becoming popular. Numerous experiments with deep neural networks, where the representation learned on a source task is transferred to learn a target neural network, have shown the benefits of the approach. This paper, similarly, deals with hypothesis transfer learning. However, it presents a new approach where, instead of transferring a representation, the source hypothesis is kept and this is a translation from the target domain to the source domain that is learned. In a way, a change of representation is learned. We show how this method performs very well on a classification of time series task where the space of time series is changed between source and target.
    bibtex: >
      @InProceedings{Cornuejols20TL, author="Cornu{\'e}jols, Antoine and Murena, Pierre-Alexandre and Olivier, Rapha{\"e}l", editor="Berthold, Michael R. and Feelders, Ad and Krempl, Georg", title="Transfer Learning by Learning Projections from Target to Source", booktitle="Advances in Intelligent Data Analysis XVIII", year="2020", publisher="Springer International Publishing", address="Cham", pages="119--131", isbn="978-3-030-44584-3"}

  - title: Retrieval-Based Neural Code Generation
    authors: Shirley Anugrah Hayati*, Raphael Olivier*, Pravalika Avvaru*, Pengcheng Yin, Anthony Tomasic, Graham Neubig
    url: https://arxiv.org/abs/2005.14070
    booktitle: Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing (EMNLP)
    location: Brussels
    date: October 2018
    abstract: >
      Deploying deep learning models, comprising of non-linear combination of millions, even billions, of parameters is challenging given the memory, power and compute constraints of the real world. This situation has led to research into model compression techniques most of which rely on suboptimal heuristics and do not consider the parameter redundancies due to linear dependence between neuron activations in overparametrized networks. In this paper, we propose a novel model compression approach based on exploitation of linear dependence, that compresses networks by elimination of entire neurons and redistribution of their activations over other neurons in a manner that is provably lossless while training. We combine this approach with an annealing algorithm that may be applied during training, or even on a trained model, and demonstrate, using popular datasets, that our method results in a reduction of up to 99\% in overall network size with small loss in performance. Furthermore, we provide theoretical results showing that in overparametrized, locally linear (ReLU) neural networks where redundant features exist, and with correct hyperparameter selection, our method is indeed able to capture and suppress those dependencies. 
    bibtex: >
      @inproceedings{Hayati18RB, title = "Retrieval-Based Neural Code Generation", author = "Hayati, Shirley Anugrah  and Olivier, Raphael  and Avvaru, Pravalika  and Yin, Pengcheng  and Tomasic, Anthony  and Neubig, Graham", booktitle = "Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing", month = oct, year = "2018", address = "Brussels, Belgium", publisher = "Association for Computational Linguistics", url = "https://aclanthology.org/D18-1111", doi = "10.18653/v1/D18-1111", pages = "925--930"}

weight: 3
widget:
  handler: publications

  # Options: sm, md, lg and xl. Default is md.
  width: lg

  sidebar:
    # Options: left and right. Leave blank to hide.
    position: left
    # Options: sm, md, lg and xl. Default is md.
    scale:
  
  background:
    # Options: primary, secondary, tertiary or any valid color value. Default is primary.
    color: secondary
    image:
    # Options: auto, cover and contain. Default is auto.
    size:
    # Options: center, top, right, bottom, left.
    position:
    # Options: fixed, local, scroll.
    attachment: 
---