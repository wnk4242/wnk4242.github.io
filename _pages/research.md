---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---
## Jump to:
- [Research Replicability](#research-replicability)
- [Meta-analysis](#meta-analysis)
- [Generative AI for Education](#generative-ai-for-education)



<h2 id="research-replicability" style="text-align: center;">Research Replicability</h2>
Efforts to replicate past psychological study findings often fail to yield consistent results. Psychologists have conducted several large-scale multi-lab replication projects (such as the Many Labs series) to reassess the credibility of earlier findings. I am currently pursuing three lines of research to enhance our understanding of research replicability:

**1. The application of Bayesian meta-analysis in the evaluation of direct replications**

Psychologists are currently faced with a pressing methodological challenge: developing a  framework to evaluate outcomes of replications. In my dissertation, I propose adopting the Bayesian hypothesis testing
within a meta-analytic framework and explore how well such an approach answers the following question: *“Do the pooled data from replications support or refute the presence of the psychological 
effect?”*

Deploying R-based simulation code on high-performance computing clusters, I created research environments with different levels of p-hacking, publication bias, and statistical power:

![Shiny App](/images/research_environment_enhanced.jpg)

The study provides strong evidence that meta-analytic Bayesian hypothesis testing is more effective in supporting the absence of null effects than in confirming the presence of true effects. This work expands the Bayesian perspective on evaluating replication outcomes, demonstrating the value of Bayesian hypothesis testing as a valuable tool for future large-scale, multi-lab replication projects. 

An overview of the study is available in my [GitHub repository](https://github.com/wnk4242/MetaBayes_Evaluation). I have also developed Shiny apps to facilitate data analysis and visualization. I use [ROC curves](https://quantpsych.shinyapps.io/ROCurve/) and [pie charts](https://quantpsych.shinyapps.io/piechartmetrics/) to compare MABF methods. I use [beta regression model and other tests](https://quantpsych.shinyapps.io/SimulationAnalysis/) to explore the influence of methodological factors on the replication results. 
<hr style="border-top: 1px dotted #999;">

**2. Credibility of research findings in educational psychology**
  
Statistical power plays a key role in ensuring the reliability, precision, and replicability of effect size estimation. In psychology, the average power is distressingly low—estimated at 36% with only 8% of studies deemed adequately powered. Meta-analyses synthesizing underpowered studies risk high false positive rates and inflated effect sizes. This study examines the credibility of meta-analyses published in five leading educational psychology journals by evaluating their median retrospective power. The median retrospective power of the studies included in SMD-based meta-analyses was estimated to be 31%, indicating that most of the experiment-based studies were inadequately powered.
The following table shows the median retrospective power of a few selected meta-analyses included in the study. The investigated effects with a MRP larger than .5 are more likely to be true (i.e., non-spurious).

| Educational Psychology Effect                                                                 | Median Retrospective Power |
|-----------------------------------------------------------------------------------------------|-----------------------------|
| Activity-related Achievement Emotions                                                         | 0.94                        |
| Multimedia Effect In Problem Solving                                                          | 0.74                        |
| Effects of Gamification on Cognitive, Motivational, and Behavioral Learning Outcomes          | 0.70                        |
| Peer Interaction in Facilitating Learning                                                     | 0.51                        |
| Social and Emotional Learning Interventions on Teachers' Burnout Symptoms                     | 0.42                        |
| Reading Interventions for Students with Reading and Behavioral Difficulties                   | 0.36                        |
| Effects of Self-Regulated Learning Training Programs                                          | 0.32                        |
| Impact of Motivational Reading Instruction on Reading Achievement and Motivation of Students  | 0.23                        |
| Effectiveness of Multimedia Pedagogical Agents                                                | 0.10                        |
| …                                                                                             | …                           |

Completion of this work will raise awareness within the academic community about the prevalence of under-powered research in top-tier journals. Based on MRP, we can build a database to provide researchers with potential replication topics in psychology and their probabilities of being successfully replicated. A working paper (AERA proposal) is [available here.](https://wnk4242.github.io/files/power paper.pdf) Peer-reviewers' feedback is [available here.](https://wnk4242.github.io/files/power paper feedback.pdf) I presented this work in a poster session at the Modern Modeling Methods conference (view the [poster](https://wnk4242.github.io/files/M3-2.pdf)).





<h2 id="meta-analysis" style="text-align: center;">Meta-analysis</h2>
An important application of meta-analytic methods is pooling single proportions to estimate the overall prevalence of a specific condition. In 2017 alone, 152 meta-analyses of proportions were published across various scientific disciplines, such as medicine, public health, epidemiology, etc. These meta-analyses not only guide future research but also help policymakers make informed decisions. 

**1. Methodological guide on conducting meta-analyses of proportions**

My comprehensive tutorial offers clear, structured methodological guidance to applied researchers on how to conduct meta-analyses of proportion in the R programming environment. It presents a step-by-step workflow and a critical review on common practices that could lead to biased effect estimates or misleading conclusions. 

I created a [walkthrough video](https://youtu.be/2wbXTFvaRnM?si=oP4TMqDj1bLXgEif) for this tutorial on YouTube, which has achieved 19k views, a 99% approval rating, and many positive comments.
![Shiny App](/images/metaprop.png)

This tutorial has garnered significant attention from the international research community, as evidenced by more than 60,000 reads on ResearchGate and 230+ citations on Google Scholar:
* Wang, N. (2023). Conducting meta-analyses of proportions in R. _Journal of Behavioral Data Science_, 3(2), 1-63. [Available here](https://www.researchgate.net/publication/375451196_Conducting_Meta-analyses_of_Proportions_in_R).
<hr style="border-top: 1px dotted #999;">

**2. Effect size, heterogeneity, and power of direct replications**

Effect-size variability (also known as heterogeneity), is a key methodological factor that is frequently neglected in planning the sample sizes for replication studies. My research investigates several
fundamental questions regarding heterogeneity in replication studies and examines how the potentially linear relationship between effect sizes and heterogeneity may impact the statistical power of
replications. Gaining a better understanding of heterogeneity is key to improving sample size planning for future multi-lab replication projects. An AERA iPoster is [available here.](https://aera24-aera.ipostersessions.com/?s=8C-A3-3D-B1-3C-88-5E-CB-83-7D-3D-0C-C3-0A-CA-A7)
  
![Shiny App](/images/complex_relation.png)
<hr style="border-top: 1px dotted #999;">

**3. CoviPanel: A Simple, Gamified, AI-Assisted Tool for Conducting Systematic Reviews in Covidence**

CoviPanel is a lightweight systematic review tool designed for researchers who need to screen large volumes of studies in [Covidence](https://www.covidence.org/). CovPanel reimagines the abstracts screening process, turinging it into a faster, more focused, and even enjoyable task. 

I built CoviPanel to make the systematic review process easier for all of us. CoviPanel is free, open source, and ready for you to explore. Visit my [GitHub repo](https://github.com/wnk4242/CoviPanel), where I've put together clear, short, intuitive tutorials to help you get started with CoviPanel.

<p align="center">
  <img src="/images/mainpanelorig.png" width="200" style="margin-left: 20px;" />
  <img src="/images/water5s.gif" width="200" style="margin-left: 20px;" />
  <img src="/images/snoopy5s.gif" width="200" style="margin-left: 20px;" />
</p>

**Key Features:**

- **Flexible AI-assisted screening**
CoviPanel integrates with #ChatGPT to offer a second opinion on each study by analyzing the title and abstract and providing a suggested decision with a concise explanation.
- **Gamified rewards to stay motivated** 
As you screen studies, you'll level up through "academic ranks"—from a clueless Research Assistant 🤦‍♂️‍ to a distinguished Professor 🧙‍—via a video game–style reward system that keeps you motivated through long sessions.
- **Easy, streamlined navigation** 
CoviPanel guides you through your assigned studies in a controlled, focused sequence—no more scrolling through pages to find them!
- **Multiple keyword highlighting** 
Search for multiple keywords in titles and abstracts and highlight them simultaneously—helping you quickly spot relevant terms and rule out irrelevant studies with ease.
- **Post-screening recap** 
After each session, CoviPanel provides a clear summary of your screening activity—including time spent, decision breakdown, and interrater reliability with AI.






<h2 id="generative-ai-for-education" style="text-align: center;">Generative AI for Education</h2>
My AI-related research examines the use of large language models in second-language learning, work I presented at the 22nd International Conference on Pragmatics and Language Learning in 2024. Specifically, I investigate whether models such as ChatGPT can effectively assist non-native English speakers in producing appropriate responses across diverse social contexts. I summarized this study in a 5-minute mini presentation, which you can [watch here](https://drive.google.com/file/d/1F6_0KOGe7-sB9vEN5HcJZHvz-9sK_rPr/preview).

![Shiny App](/images/cvh.png)

We created 32 short vignettes, each one has an everyday social scenario. We asked ChatGPT to generate responses that were either appropriate or inappropriate in those scenarios. These became our experimental materials. Then we asked both ChatGPT and human raters to grade these responses on a scale from 1 to 5 in terms of their conversational appropriateness. 

The most interesting finding of this study is that in conversations involving power dynamics (e.g., when you talk to your boss), ChatGPT often struggles to find socially appropriate responses, where sensitivity to social appropriateness is essential. These findings can inform the design of AI partners that not only support learning but also foster respectful, effective communication in collaborative small-group settings.

I developed a Python-based pipeline for this project, which automated data collection across multiple ChatGPT models, reducing data processing time by 90%. The code is [available here](https://github.com/wnk4242/GPTdataCollector).
