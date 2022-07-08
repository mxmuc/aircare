---
layout: home
title: AirCare
subtitle: We Make Jet Engine Maintenance Smart, Comprehensible and Hassle Free
cover-img: "/assets/img/jet-engine-header.png"
full-width: false
---

## Problem & Customer Need <a name="problem"></a>

{: style="text-align: justify" }
Travelling by airplane is one of the fastest and most convenient ways to journey along long distances. To make flights as secure as possible, frequent maintenance is needed. As a vital part of the airplane, engines must go through maintenance either after a certain amount of flight hours or if damages occur.

{: style="text-align: justify" }
To conduct the maintenance, the airplane engine has to be dissassembled into all its parts. Thereafter, every part is checked, cleaned, fixed or replaced. Finally, the engine is reassembled and thoroughly tested. However, **75%** of all airplane engine test after maintenance fail due to leakages of air, oil or fuel. Most of these leakages are caused by human error during assembly. The four most common sources of these human errors are:
* missed steps or steps done wrong during reassembly
* use of wrong parts or configurations
* use of damaged parts (e.g. damaged sealings)
* contamination of parts or surfaces (e.g. by dirt or lint)

{: style="text-align: justify" }
These failed tests are very costly to enigne maintenance providers like MTU Maintenance due to a number of reasons. The three most impactful ones are:
* testing an engine takes up valuable time in the testing cells. 
* if the engine fails a test it must be dissassembled, checked and reassembled again- this may take up to two shifts time and it is not ensured that further error can be prevented while reassembling the engine for the second time
* failed tests are an environmental hazard: during the test, real resources like oil and fuel are being used. If an eninge fails the test, these resources are wasted.
<br />
<br />

## Our Solution <a name="solution"></a>

{: style="text-align: justify" }
We provide a digital and smart solution, that is especially tailored to fit the needs of airplane engine maintenance providers. Our App can be used to  track the work done by mechanics, make the specific worksteps more comprehensible, collect data on issues and raise awareness about difficult tasks. Team Leads are able to assigne tasks quickly and plan workloads and resource occupations accordingly. This will enable teams to track their work progress in real-time. 

{: style="text-align: justify" }
With our App, we provide mechanics with all the details they need to know and track assembly progress to identify mistakes while they are being made. Hence, airplane enigne assembly will become more efficient. Human error as well as common problems like leakages of oil, fuel or air will be minimized and  errors during assembly will be reduced.

![Have a glimpse into our App!](/assets/img/app_mockup1.png){:class="displayed"}

Our App compromises 6 key features to guarantee ease of use and the best support possible during maintenance:
* *Smart and Mobile*: Our App can be used on any mobile device and is a multi-facetted and convenient platform for the engineers to use directly at their workstation. We include a knowledge hub to collect all information about steps and make smart assignment of open tasks to the next free resource possible
* *Digital*: we significantly reduce the amount of paper used and shift all documentation to our digitzed platform
* *Data Collection & Feedback*: we can track which steps and parts have caused issues in the past. This enables us to statistically analyze the assembly and give warnings to mechanics for the most critical steps
* Comprehensible: The app is easy to understand and use and will not create any additional workload compared to the previous paper documentation
* *Task Facilitation*: our first language will be german as most engineers speak german as their mother language. The app will give engineers a clear overview over their tasks, all in one place, and will assist throughout tasks with references to mastercards and tips for completing the steps
* *Task Validation*: every mechanic has to confirm the work he has done after finalization of a step
<br />
<br />

## Customer Value Proposition <a name="cvp"></a>

{: style="text-align: justify" }
Getting a deeper understanding of how polarization manifests itself in language, we use `BERT’s pre-trained Sentence Transformer` to embed the quotations into numerical arrays of the same length (768 digits). With these embeddings as a vantage point, we could now use similarity metrics such as the cosine similarity to investigate within-party and between-party polarization. The evaluated cosine similarity yields a continuous number between 0 and 1, with a higher value indicating a higher similarity. It's worth noticing that the similarity metric presented is more precisely a semantic similarity between 2 sentences (i.e., how similar is their meaning).

{: style="text-align: justify" }
Our first step along the NLP path yielded the following results:

- On average quotations uttered by _Democrats_ have a higher similarity with each other than with any other socio-political subgroup. We therefore conclude a **low within-party polarization within the _Democratic party_ when looking at climate change**

- The average quote similarity within the _Republican party_ is even lower than the similarity between the two parties. This indicates that **discussions around climate change are highly polarized amongst _Republicans_**
<br />
<br />
<br />

:-------------------------:|:-------------------------:
![Similarity Distribution](/assets/img/similarity_frequency.png){:class="displayed"}  |  ![Similarity Between Within](/assets/img/similarity_between_within.png){:class="displayed"}

<br />

{: style="text-align: justify" }
Making everything more tangible, we look at the top three speakers for each party, whose quotes have the highest within-party and between-party similarity. Looking at the Democrats - interestingly - **high-ranking politicians** such as the former president Bill Clinton, US representative Adam Schiff and senator Richard Blumenthal **lead the similarity ranking - both within their own party and between parties**. We can only hypothesize about this effect being linked to an overwhelming amount of quotes for these politicians and their mediator role. Even the top three Republicans, former governor of Ohio John Kasich, US representative Fred Upton and governor of New Hampshire Chris Sununu have a higher between-party similarity than within-party similarity. This again underlines the **high polarization within the Republican party**.
<br />
<br />

![Top 3 Speakers Similarity](/assets/img/top_3_similarities.png){:class="displayed"}
<br />
<br />

{: style="text-align: justify" }
The second step instead consisted in looking at quote similarities at **person level**. Again using cosine similarity, we are able to construct a similarity matrix storing similarities for all possible speaker-to-speaker combinations. Considering that at this point the number of speakers was of exactly 5,442, still very high, plotting them is neither useful nor pretty. We instead present an interactive undirected network graph, showing the **top-3 similarities for the 50 most talkative persons from each party**. [Play around with it](https://mxmuc.github.io/do-people-with-different-ideologies-speak-differently/assets/html/person_lvl_similarity.html) for as long as you want. The network was created using `pyvis` library and some good ol' `javascript`.
<br />
<br />

## Market <a name="market"></a>

{: style="text-align: justify" }
There are several aspects and subtopics about how one can discuss climate change. To detect underlying topics and affiliate quotes with their dominant topic, we followed a structured workflow to build an insightful model based on the **Latent Dirichlet Allocation (LDA) algorithm**. Before creating the topic model using `gensim's native LdaModel` library, we  cleaned and tokenized the quotes and additionally added bigrams to the model.
{: style="text-align: justify" }
We were able to group the quotations around **three distinct topics**. The word cloud below with the size of the words proportional to the weight gives an overview about the content of each topic. While topics 1 and 3 are closely related to the discussion about climate change, topic 2 is centered around oil and its economic aspects.
{: style="text-align: justify" }
If the charts below are not yet enough for you, feel free to play around with our [interactive topic visualization](https://mxmuc.github.io/do-people-with-different-ideologies-speak-differently/assets/html/climate_change_topics_lda.html) using `pyLDAvis`.
<br /> 
<br /> 

![Topic Word Cloud](/assets/img/topic_word_cloud.png){:class="displayed"}
<br /> 

![Topic Word Count and Importance](/assets/img/topic_word_count_important_keywords.png){:class="displayed"}

![Cluster Topics](/assets/img/topic_cluster_bokeh.png){:class="image-box"}

<br /> 
<br /> 

#### What Are the Most Discussed Topics Among Democrats and Republicans?

{: style="text-align: justify" }
As we were faced with an imbalanced dataset containing significantly more quotes for Democrats and Men, we balanced the four socio-political subgroups using [Random Oversampling](https://machinelearningmastery.com/random-oversampling-and-undersampling-for-imbalanced-classification/). Through randomly duplicating examples in the minority class (i.e., Republicans and Women), we obtained four subgroups with the same amount of quotes. Looking now at the representation of each subgroup in the different topics, we gain a deeper understanding in how group divisions manifest themselves in the topics discussed. 

- The _gender_ of the speaker has no relevant impact on which aspect of climate change is discussed

- The _party_ _affiliation_ of a speaker has a strong impact on the way they discuss climate change

- _Democrats_ tend to be more worried about the effect of climate change on our future. Whereas _Republicans_ tend to center their discussions around fossil fuels (e.g., oil and coal) and the economic impact of an energy transition 

- _Democrats_ discuss climate change more frequently than _Republicans_

Below figure visualizes the share of quotes by party affiliation and gender for each topic after oversampling. If all topics would be equally frequent discussed between the different socio-political subgroups, all slices would be of same size (i.e., 25%)

<br />

![Topic Pie Chart Oversampled by Party and Gender](/assets/img/topic_pie_party_gender_oversampled.png){:class="displayed"}
<br /> 
<br /> 
<br /> 

## Download <a name="download"></a>
#### Are Democrats Really More Concerned About Climate Change Than Republicans?

{: style="text-align: justify" }
Language is rich in subtle signals and quotes can convey different connotations. Having gained a first understanding about how polarization is motivated by socio-political differences, we dive deeper using semantic analysis. Therefore, we use `Empath`, a tool developed at Stanford University that can generate and validate new lexical categories from a set of seed terms. We use `Empath` to validate whether Democrats are really more concerned about climate change than Republicans?

<br />

![Empath Bar Chart by Party](/assets/img/empath_topics_1_3.png){:class="displayed"}

<br />
{: style="text-align: justify" }
As topic 2 is focussed around oil and its economic impact, we have excluded it for this analysis. We can not directly confirm our above hypotheses, that Democrats are more concerned about climate change than Republicans. However, we could observe the following: 

- _Democrats_ are more likely to use extreme vocabulary when talking about climate change. Way more quotations of Democrats fall into categories such as _crisis_, _war_ and _help_

- Quotations of _Democrats_ convey far more negavtively associated connotations than the ones of Republicans

- _Republicans_ do not get tired of speaking about oil
<br />
<br />
<br />

## Final Words

{: style="text-align: justify" }
Even if our project only touched the surface of understanding the causes and consequences of media polarization, we learned a lot about how climate change is discussed in US media among Democrats and Republicans. We could validate common hypotheses, such as that Republicans mainly focus their thoughts around fossil fuels when speaking about climate change. Our analysis further showed that Democrats do not just speak more about climate change; they are also more worried about the effects of it on our future. This is expressed through the usage of extreme vocabulary with negative connotations. We were able to show that climate change is a highly polarized topic - especially within the Republican party. Finally, we could not find that the gender of a speaker influences neither the way nor the frequencies one speaks about climate change.
<br />
<br />

{: style="text-align: center" }
AirCare was realised in 2022 as part of the [Tech Challenge](https://academy.unternehmertum.de/programs/tech-challenge) at the [Technical University of Munich (TUM)](https://www.tum.de/en/)







