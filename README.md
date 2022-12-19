# Machine Learning based Early Decision-Making (ML-EDM)

This is the official github page of the paper \[[1](https://arxiv.org/pdf/2204.13111.pdf)] ["Open challenges for Machine Learning based Early Decision-Making research"](https://arxiv.org/pdf/2204.13111.pdf), *Alexis Bondu, Youssef Achenchabe, Albert Bifet, Fabrice Clérot, Antoine Cornuéjols, Joao Gama, Georges Hébrail, Vincent Lemaire, Pierre-François Marteau*.

**The purpose of this page is to gather all ML-EDM related material, including source code, research papers and datasets.**

* Join us on ["Reddit"](https://www.reddit.com/r/EarlyMachineLearning/);
* Follow us on ["Twitter"](https://twitter.com/ML_Early);
* Watch our videos on ["YouTube"](https://www.youtube.com/channel/UCEUK7Q1gARRck1FB4Qo_3aQ).  

## Early Decision Making
More and more applications require early decisions, i.e. taken as soon as possible from partially observed data. However, the later a decision is made, the more its accuracy tends to improve, since the description of the problem to hand is enriched over time. Such a compromise between the *earliness* and the *accuracy* of decisions has been particularly studied in the field of Early Classification of Time Series (ECTS). However, the current definition of ECTS is limited to:

* a classification problem ; 
* an available training set which contains completely and properly labeled time series ;
* a decision deadline that is finite, fixed and known ;
* unique decisions for each incoming time series ;
*  decisions that once made can never be reconsidered ;
*  fixed decision costs which do not depend on the triggering time and the decisions made.

In order to overcome these limitations, we introduce a more general problem, called Machine Learning based Early Decision Making (ML-EDM), which consists in optimizing the decision times of models in a wide range of settings where data is collected over time. After defining the ML-EDM problem, ten challenges are identified and proposed to the scientific community to further research in this area. These challenges open important application perspectives.


## Proposed challenges
| ML-EDM challenges | SOTA | Main application perspectives |
| :---         |     :---:      |          :---|
| **#1 -** Extending non-myopia to unsupervised approaches  |    | In anomaly detection applications, anticipate the deviation of an observed individual from a normal behavior.    |
| **#2 -** Addressing other supervised learning tasks     |       | Adapt ECTS approaches to extrinsic regression problems. Develop forecasting methods whose prediction horizon can adapt  |
| **#3 -** Early weakly supervised learning (WSL) |   | Adapt ECTS approaches to the different WSL classification scenarios | 
| **#4 -** Data type agnostic ML-EDM | \[[2](https://bird.bcamath.org/bitstream/handle/20.500.11824/742/TNNLS-2017-P-7530.pdf?sequence=1),[3](https://link.springer.com/content/pdf/10.1007/978-3-319-23528-8_27.pdf),[4](http://www2.agroparistech.fr/ufr-info/membres/cornuejols/Papers/PUBLIES/2021_dsaa_paper.pdf),[5](https://link.springer.com/article/10.1007/s10994-021-05974-z)] | Identify agnostic approaches in the literature and promote this feature. Define a pivotal format allowing to develop an ML-EDM library |
| **#5 -** Online predictions to be located in time |  | Applications where the arrival of an event (e.g. a failure) must be predicted in advance, as well as its duration |
| **#6 -** Online accuracy vs. earliness trade-of | \[[6](https://arxiv.org/pdf/2204.00392.pdf)] | Optimize decision time in online predictive maintenance applications. |
| **#7 -** Management of non-stationarity in ML-EDM | | Properly manage the potentially long life of ML-EDM models.|
| **#8 -** Reactivity vs. stability dilemma for revocable decisions | \[[7](https://arxiv.org/pdf/2109.10285.pdf)] | Applications where undue and excessive decision changes must be avoided|
| **#9 -** Non-myopia to revocation risk | \[[7](https://arxiv.org/pdf/2109.10285.pdf)] | Non-myopia to revocation risk |
| **#10 -** Scheduling strategy and time-dependent decision costs | | Applications where the variation of the decision costs over time is known or can be modeled. Applications where the scheduling strategy is only known through itsinteractions with the triggering strategy. |

## Related papers
| Challenges | Reference | code resources |
|     :---:      |     :---:      |          :---|
| All | \[1] [Open challenges for Machine Learning based Early Decision-Making research](https://arxiv.org/pdf/2204.13111.pdf), *Alexis Bondu, Youssef Achenchabe, Albert Bifet, Fabrice Clérot, Antoine Cornuéjols, Joao Gama, Georges Hébrail, Vincent Lemaire, Pierre-François Marteau.*  ArXiv 2022. |  |
| #4 | \[2] [Early classification of time series by simultaneously optimizing the accuracy and earliness](https://bird.bcamath.org/bitstream/handle/20.500.11824/742/TNNLS-2017-P-7530.pdf?sequence=1), *Usue Mori, Alexander Mendiburu, Sanjoy Dasgupta, Jose A. Lozano.*  IEEE transactions on neural networks and learning systems, 29(10), 4569-4578. | [experimental reproducibility](https://github.com/Usue/EarlyClassification) |
| #4 | \[3] [Early classification of time series as a non myopic sequential decision making problem](https://link.springer.com/content/pdf/10.1007/978-3-319-23528-8_27.pdf), *Asma Dachraoui, Alexis Bondu, Antoine Cornuéjols.*  Joint European Conference on Machine Learning and Knowledge Discovery in Databases - ECML PKDD (2015) | [tslearn python library](https://github.com/tslearn-team/tslearn/blob/main/tslearn/early_classification/early_classification.py) |
| #4 | \[4] [Early Classification of Time Series: Cost-based multiclass Algorithms](http://www2.agroparistech.fr/ufr-info/membres/cornuejols/Papers/PUBLIES/2021_dsaa_paper.pdf), *Paul-Emile Zafar, Youssef Achenchabe, Alexis Bondu, Antoine Cornuéjols, Vincent Lemaire.*  IEEE 8th International Conference on Data Science and Advanced Analytics - DSAA (2021). | [experimental reproducibility](https://github.com/YoussefAch/Eco-gamma-multiclass) |
| #4 | \[5] [Early classification of time series](https://link.springer.com/article/10.1007/s10994-021-05974-z), *Youssef Achenchabe, Alexis Bondu, Antoine Cornuéjols, Asma Dachraoui.* Machine Learning 110.6 (2021): 1481-1504. | [experimental reproducibility](https://github.com/YoussefAch/Economy) |
| #6 | \[6] [ECOTS: Early Classification in Open Time Series](https://arxiv.org/pdf/2204.00392.pdf), *Youssef Achenchabe, Alexis Bondu, Antoine Cornuéjols, Vincent Lemaire.* ArXiv 2022. | *coming soon* |
| #8, #9 | \[7] [Early and Revocable Time Series Classification](https://arxiv.org/pdf/2109.10285.pdf), *Youssef Achenchabe, Alexis Bondu, Antoine Cornuéjols, Vincent Leamire.* International Joint Conference on Neural Networks - IJCNN (2022). | [experimental reproducibility](https://github.com/YoussefAch/rev-economy) |



## Datasets / Use cases

... TODO ...

## Librairies 

... TODO ...
