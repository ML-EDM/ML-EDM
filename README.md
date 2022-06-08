# Machine learning based early decision-making (ML-EDM)

This is the official github page of the paper ["Open challenges for Machine Learning based Early Decision-Making research"](https://arxiv.org/pdf/2204.13111.pdf), Alexis Bondu, Youssef Achenchabe, Albert Bifet, Fabrice Clérot, Antoine Cornuéjols, Joao Gama, Georges Hébrail, Vincent Lemaire, Pierre-François Marteau.

**The purpose of this page is to gather all early decision-making related material, inscluding source code, research papers and datasets.**


More and more applications require early decisions, i.e. taken as soon as possible from partially observed data. However, the later a decision is made, the more its accuracy tends to improve, since the description of the problem to hand is enriched over time. Such a compromise between the earliness and the accuracy of decisions has been particularly studied in the field of Early Time Series Classification. We introduce a more general problem, called Machine Learning based Early Decision Making (ML-EDM), which consists in optimizing the decision times of models in a wide range of settings where data is collected over time. After defining the ML-EDM problem, ten challenges are identified and proposed to the scientific community to further research in this area. These challenges open important application perspectives.


## Challenges
| ML-EDM challenges | SOTA | Main application perspectives |
| :---         |     :---:      |          :---|
| Extending non-myopia to unsupervised approaches  |    | In anomaly detection applications, anticipate the deviation of an observed individual from a normal behavior.    |
| Addressing other supervised learning tasks     |       | Adapt ECTS approaches to extrinsic regression problems. Develop forecasting methods whose prediction horizon can adapt  |
| Early weakly supervised learning (WSL) |   | Adapt ECTS approaches to the different WSL classification scenarios | 
| Data type agnostic ML-EDM | [Achenchabe et al.](https://link.springer.com/article/10.1007/s10994-021-05974-z), [Mori et al.](https://bird.bcamath.org/bitstream/handle/20.500.11824/742/TNNLS-2017-P-7530.pdf?sequence=1) | Identify agnostic approaches in the literature and promote this feature. Define a pivotal format allowing to develop an ML-EDM library |
| Online predictions to be located in time |  | Applications where the arrival of an event (e.g. a failure) must be predicted in advance, as well as its duration |
| Online accuracy vs. earliness trade-of | [Achenchabe et al.](https://arxiv.org/pdf/2204.00392.pdf) | Optimize decision time in online predictive maintenance applications. |
| Management of non-stationarity in ML-EDM | | Properly manage the potentially long life of ML-EDM models.|
| Reactivity vs. stability dilemma for revocable decisions | [Achenchabe et al.](https://arxiv.org/pdf/2109.10285.pdf) | Applications where undue and excessive decision changes must be avoided|
| Non-myopia to revocation risk | [Achenchabe et al.](https://arxiv.org/pdf/2109.10285.pdf) | Non-myopia to revocation risk |
| Scheduling strategy and time-dependent decision costs | | Applications where the variation of the decision costs over time is known or can be modeled. Applications where the scheduling strategy is only known through itsinteractions with the triggering strategy. |

## Source code


## Datasets


## Research papers
