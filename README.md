## It's time for images to have a go at code clone detection!

![Vincent logo](https://ucl-crest.github.io/iwsc2018-vincent-web/images/logo.png)

We introduce a new code clone detection technique based on image similarity, and a tool called **Vincent**. The technique captures visual perception of code seen by humans in an IDE by applying syntax highlighting and images conversion on raw source code text.

We compared two similarity measures, Jaccard and earth mover’s distance (EMD) for our image-based code clone detection technique. Jaccard similarity offered better detection perfor- mance than EMD. The F1 score of our technique on detecting Java clones with pervasive code modifications is comparable to five well-known code clone detectors: CCFinderX, Deckard, iClones, NiCad, and Simian. A Gaussian blur filter is chosen as a normalisation technique for type-2 and type-3 clones. We found that blurring code images before similarity computation resulted in higher precision and recall. The detection performance after including the blur filter increased by 1 to 6 percent.

The manual investigation of clone pairs in three software systems revealed that our technique, while it missed some of the true clones, could also detect additional true clone pairs missed by NiCad.

### Vincent: an image-based code clone detection tool

Vincent is an open-source tool and can be downloaded here: [Vincent repo](https://bitbucket.org/chaiyong_ragkhitwetsagul/vincent/overview)

### Data Sets

We used two data sets in this study:
1. The generated data set to measure F1 scores of Vincent and other clone detectors. It is from our previous study. The data set can be found here: [Generated dataset](http://crest.cs.ucl.ac.uk/resources/cloplag/).
2. The three Java systems (JUnit4, JFreeChart, Tomcat) are also from our another previous study. They can be found here: [IWSC 2017 Dataset](https://cragkhit.github.io/crjk-iwsc17/).

### Clones Reported by Vincent and NiCad and the manual clone validation

The clone pairs reported by Vincent and NiCad can be downloaded below. We processed the clones so that they are divided into three different sets: 1) common (clone pairs found by both Vincent and NiCad), 2) disjoin-v (clone pairs found only by Vincent), 3) disjoint-n (clone pairs found only by NiCad). The first author looked at 100-randomly sampled clone pairs in each projects and validated them.

The clone reports and the manual clone validation results can be downloaded [here](https://ucl-crest.github.io/iwsc2018-vincent-web/files/vincent_clones+manual_validation.zip).

### Support or Contact

Having trouble with Vincent or the data? Please contact:

* Chaiyong Ragkhitwetsagul, Research Student, CREST, University College London, UK
* Email: <chaiyong.ragkhitwetsagul.14@ucl.ac.uk> or <cragkhit@gmail.com>
