# Online Appendix for "Mining Unstructured Software Repositories Using IR Models" (Stephen W. Thomas - PhD Thesis)

PhD Thesis, Queen's University, December 2012

## Abstract

Mining software repositories, which is the process of analyzing the data related to software development practices, is an emerging field which aims to aid development teams in their day to day tasks. However, data in many software repositories is currently unused because the data is unstructured, and therefore difficult to mine and analyze. Information Retrieval (IR) techniques, which were developed specifically to handle unstructured data, have recently been used by researchers to mine and analyze the unstructured data in software repositories, with some success.

The main contribution of this thesis is the idea that the research and practice of using IR models to mine unstructured software repositories can be improved by going beyond the current state of affairs. First, we propose new applications of IR models to existing software engineering tasks. Specifically, we present a technique to prioritize test cases based on their IR similarity, giving highest priority to those test cases that are most dissimilar. In another new application of IR models, we empirically recover how developers use their mailing list while developing software.

Next, we show how the use of advanced IR techniques can improve current software engineering productivity. Using a framework for combining disparate IR models, we find that bug localization performance can be improved by 14--56\% on average, compared to the best individual IR model. In addition, by using topic evolution models on the history of source code, we can uncover the evolution of source code concepts with an accuracy of 87-89%.

Finally, we show the risks of current research, which uses IR models as black boxes without fully understanding their assumptions and parameters. We show that the data duplication effect in source code has undesirable effects for IR models, and that by eliminating the duplication, the accuracy of IR models improves. Additionally, we find that in the bug localization task, an unwise choice of parameter values results in an accuracy of only 1%, where optimal parameters can achieve an accuracy of 55%.

Through empirical case studies on real-world systems, we show that all of our proposed techniques and methodologies significantly improve the state-of-the-art.

## Bibtex

The thesis can be cited as follows:

```bibtex
@phdthesis{thomas:phd2012,
   author={Stephen W. Thomas},
   school={Queen's University},
   title={Mining Unstructured Software Repositories Using IR Models},
   year={2012},
}
```

Also consider citing the paper related to specific chapter.

## Data

Please see the replication package of the respective chapter/paper:

- [Chapter 3: Static Test Case Prioritization](https://github.com/SAILResearch/replication-prioritize_testcase_topicmodels)
- [Chapters 5 and 8: Classifier Configuration and Combination](https://github.com/SAILResearch/replication-classifier_conf_config_bugloc)
- [Chapter 7: The Diff Model](https://github.com/SAILResearch/replication-evolution_topics_code)

## Tools

- My ```tcp.lda``` test case prioritization tool (Chapter 3) is on [GitHub](https://github.com/doofuslarge/tcp.lda).
- My ```lscp``` preprocessing tool (used throughout the thesis) is on [GitHub](https://github.com/doofuslarge/lscp).
- My ```lucene-lda``` LDA-based search tool (Chapt  ers 5 and 8) is on [GitHub](https://github.com/doofuslarge/lucene-lda).
- My ```CountNGrams``` Hadoop-based NGram counting tool (not used in thesis, but may be helpful anyway) is on [GitHub](https://github.com/doofuslarge/CountNGrams). 
