# Code Health and Technical Debt Study 2022

This repo contains a complete replication package, including raw data and scripts for the statistical analysis, for the paper by A. Tornhill & M. Borg, "Code Red: The Business Impact of Code Quality: A Quantitative Study of 39 Proprietary Production Codebases", 2022. The [paper](https://www.computer.org/csdl/proceedings-article/techdebt/2022/930400a011/1EygGuOH3e8) is published in the [Proc. of 2022 IEEE/ACM International Conference on Technical Debt (TechDebt)](https://2022.techdebtconf.org/). A [preprint](https://arxiv.org/abs/2203.04374) is available on arXiv.

The data is based on the [Code Health metric](https://codescene.com/code-health/) and collected via CodeScene. Instructions for reproducing the study are available in the Jupyter Notebook.

## Abstract

Code quality remains an abstract concept that fails to get traction at the business level. Consequently, software companies keep trading code quality for time-to-market and new features. The resulting technical debt is estimated to waste up to 42% of developers' time. At the same time, there is a global shortage of software developers, meaning that developer productivity is key to software businesses. Our overall mission is to make code quality a business concern, not just a technical aspect. Our first goal is to understand how code quality impacts 1) the number of reported defects, 2) the time to resolve issues, and 3) the predictability of resolving issues on time. We analyze 39 proprietary production codebases from a variety of domains using the CodeScene tool based on a combination of source code analysis, version-control mining, and issue information from Jira. By analyzing activity in 30,737 files, we find that low quality code contains 15 times more defects than high quality code. Furthermore, resolving issues in low quality code takes on average 124% more time in development. Finally, we report that issue resolutions in low quality code involve higher uncertainty manifested as 9 times longer maximum cycle times. This study provides evidence that code quality cannot be dismissed as a technical concern. With 15 times fewer defects, twice the development speed, and substantially more predictable issue resolution times, the business advantage of high quality code should be unmistakably clear. 

## Main Takeaways

We investigated three research questions:
1. How does the number of reported defects in source code files correlate to source code quality?
1. How much longer development time is needed to resolve an issue in files with low quality source code?
1. To what extent is the code quality of a file related to the predictability of resolving issues on time?

### Red Code results in 15 times more reported Jira defects than Healthy Code

<img src="https://github.com/mrksbrg/code-health-study-tech-debt-2022/blob/master/figures/code_health_number_of_issues.png" alt="RQ1: Number of issues" width="600"/>

### The time-in-development in Red Code is 124% longer compared to Healthy Code

<img src="https://github.com/mrksbrg/code-health-study-tech-debt-2022/blob/master/figures/mean_for_time_in_development.png" alt="RQ2: Average time-in-development" width="600"/>

### The maximum time-in-development for the Red Code is 9 times longer compared to Healthy Code

<img src="https://github.com/mrksbrg/code-health-study-tech-debt-2022/blob/master/figures/max_time_in_development.png" alt="RQ3: Maximum time-in-development" width="600"/>

Conclusion: Our results show that there is a significant impact of code quality on both time to market as well as the external quality of the product in the shape of software defects.

## How To Cite This Work
Please cite this work as follows:

```
@article{tornhill2022codered,
  title={Code Red: The Business Impact of Code Quality - A Quantitative Study of 39 Proprietary Production Codebases},
  author={Tornhill, Adam and Borg, Markus},
  booktitle = {2022 IEEE/ACM International Conference on Technical Debt (TechDebt)},
  year = {2022},
  volume = {},
  issn = {},
  pages = {11-20},
  doi = {10.1145/3524843.3528091},
  url = {https://doi.ieeecomputersociety.org/10.1145/3524843.3528091},
  publisher = {IEEE Computer Society},
  address = {Los Alamitos, CA, USA},
  month = {may}
}
```