# 事后检验（Post-hoc）

在一般的语境下，事后检验通常用于ANOVA分析之后比较哪两组之间存在差异（不能直接两两比较的原因是多重比较问题，即组间的检验次数过多，在错误率一定的情况下整体的错误率大幅上升）

To compare group means, we need to perform post hoc tests, also known as multiple comparisons. In Latin, post hoc means “after this.” You conduct post hoc analyses after a statistically significant omnibus test (F-test or Welch’s).

想象一个例子：

> 某临床研究发现，试验药物相比对照组能显著延长患者的生存时间。而研究者是个「星座控」，突发奇想把试验人群又基于星座进行了分组与分析。结果发现：射手座的患者应用试验药物显著延长生存时间（P＜0.05）；而处女座的患者应用试验药物与对照差异不显著（P＞0.05）。于是得出结论：射手座患者比处女座患者应用该药的生存获益更大

上述情况，显然不科学。因为分组情况非预设，且研究假设是在观察完数据的特征后提出，所以分析也就不具有统计学意义。可以简单认为此时得到的 P 值是「假 P 值」，无论是否小于 0.05，都不代表是否有「统计学差异」，只能视为体现某种趋势，可为后续预设研究设计提供思路。 

那么问题是什么呢？

观察前提出的假设叫做 预设分组，而观察后提出的假设叫做 非预设分组。 非预设分组的检验结果并不可靠，因为在某些原因下（干扰或者串联），一定会有出现p<0.05的情况，而此时的p毫无意义

A. In any discipline, studies investigating differences between groups will use post-hoc tests when the null hypothesis of an ANOVA model is rejected. 

B. In medicine, post-hoc analyses may be used in clinical trials if the original hypothesis does not hold (e.g. the primary outcome being the antidiabetic effect of a drug). Triallists then re-examine the dataset for other outcomes (not originally planned, e.g. improvement in renal outcomes in diabetes patients) and perform statistical analysis to determine other valuable results from the trial. 