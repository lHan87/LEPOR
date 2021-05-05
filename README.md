# LEPOR
LEPOR: Automatic Machine Translation Evaluation Metric with tunable parameters and augmented factors

cmd command example:
Perl the-evaluation-code.pl > score-file.txt

Thanks to Paolo Dr. (Awsome) Bolzoni, It generates the sentence-level score and the system-level score as WMT metrics submission format. e.g. 

http://www.statmt.org/wmt18/metrics-task.html 

"METRIC NAME, LANG-PAIR, TEST SET, SYSTEM, SEGMENT NUMBER, SEGMENT SCORE, ENSEMBLE, AVAILABLE"

"METRIC NAME, LANG-PAIR, TEST SET, SYSTEM, SYSTEM, SYSTEM LEVEL SCORE, ENSEMBLE, AVAILABLE"

-------------
For all the files about hLEPOR_baseline in WMT2019, e.g. rerun hLEPOR baseline for comparesion or improvement etc. you can find them all in this drive folder: (https://drive.google.com/open?id=1v6VR4r5U9tH-0jFzAtxTybxCJWUeCWdn)

- achieved best level performace metrics in German-Czech system-level MT evaluation. Pearson correlation score with human judegment: 0.959 http://www.statmt.org/wmt19/pdf/53/WMT02.pdf Table 5 pp-74. (Table-6 in https://drive.google.com/file/d/1Bf2GbtlgZaU8h7ywXH8nzjuEKtLtCD77/view?usp=sharing). 

We call it baseline in WMT2019 because we did not tune the parameters in the metric and did not use the linguistic features that we used in WMT2013 either. Instead, just used a set of default parameters and only measure the scores according ot the system output and reference files, no external resources used.


[WMT2013]
LEPOR metrics performed highest system level Pearson correlation score (0.86) with human judegemnt, on the everage five language pairs from English-to-other [en-fr en-de en-es en-cs en-ru (also best score on en-cs en-ru)] in WMT2013. https://www.aclweb.org/anthology/W13-2253 (Table 3)
 https://www.statmt.org/wmt13/pdf/WMT02.pdf (Table 3)

-------------
Citation:

COLING:

@inproceedings{han2012lepor,
  title={LEPOR: A Robust Evaluation Metric for Machine Translation with Augmented Factors},
  author={Han, Aaron L.-F. and Wong, Derek F. and Chao, Lidia S.},
  booktitle={Proceedings of the 24th International Conference on Computational Linguistics (COLING 2012)},
  pages={441-450},
  year={2012},
  organization={Association for Computational Linguistics}
}

MT SUMMIT:

@inproceedings{han2013language,
  title={Language-independent Model for Machine Translation Evaluation with Reinforced Factors},
  author={Han, Aaron L.-F. and Wong, Derek F. and Chao, Lidia S. and He, Liangye and Lu, Yi and Xing, Junwen and Zeng, Xiaodong},
  booktitle={Machine Translation Summit XIV},
  pages={215--222},
  year={2013},
  organization={International Association for Machine Translation}
}

WMT:

@inproceedings{W13-2253,
    title = "A Description of Tunable Machine Translation Evaluation Systems in {WMT}13 Metrics Task",
    author = "Han, Aaron Li-Feng  and
      Wong, Derek F.  and
      Chao, Lidia S.  and
      Lu, Yi  and
      He, Liangye  and
      Wang, Yiming  and
      Zhou, Jiaji",
    booktitle = "Proceedings of the Eighth Workshop on Statistical Machine Translation",
    month = aug,
    year = "2013",
    address = "Sofia, Bulgaria",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/W13-2253",
    pages = "414--421",
}

Msc. thesis:

@book{han2014lepor,
  title={LEPOR: An Augmented Machine Translation Evaluation Metric},
  author={Han, Lifeng},
  year={2014},
  url = {https://arxiv.org/pdf/1703.08748.pdf},
  publisher={University of Macau, Macao}
}

-------------

# Work/Project/Papers that used/refered/discussed LEPOR (hLEPOR, nLEPOR):

Marzouk, S. & Hansen-Schirra, S. 'Evaluation of the impact of controlled language on neural machine translation compared to other MT architectures'. Journal of Machine Translation (2019). https://doi.org/10.1007/s10590-019-09233-w

There is a deep statistical analysis about hLEPOR and nLEPOR performance in WMT13, which shows it performed as one of the best metrics "in both the individual language pair assessment for Spanish-to-English and the aggregated set of 9 language pairs.", see the paper (Accurate Evaluation of Segment-level Machine Translation Metrics) "https://www.aclweb.org/anthology/N15-1124" Graham et al. 2015 NAACL(https://github.com/ygraham/segment-mteval)

======
News:

LEPOR metrics are being used for broader tasks, in addition to Translation, such as searching (ACM Transactions: Meta-evaluation of Conversational Search Evaluation Metrics https://arxiv.org/pdf/2104.13453.pdf) and language generation (2017emnlp paper: Why We Need New Evaluation Metrics for NLG https://www.aclweb.org/anthology/D17-1238.pdf)

Press:
Logrus Global Adds hLEPOR Translation-quality Evaluation Metric Python Implementation on PyPi.org
https://slator.com/press-releases/logrus-global-adds-hlepor-translation-quality-evaluation-metric-python-implementation-on-pypi-org/ 

Python version of hLEPOR: https://pypi.org/project/hLepor/ 

