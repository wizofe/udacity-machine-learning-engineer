# Fuzzy string comparison for interactive learning resources with H5P (I need a better title ;-))
## Capstone Proposal
Oliver Tacke

December 31st, 2050

## Proposal
_(approx. 2-3 pages)_

It was more difficult than I thought to come up with a proposal for a capstone project. There are tons of interesting datasets out there and dozens of questions that you could possibly ask, but I'd love to create something that someone actually needed.
I contacted a friend of mine who co-created [OpenSNP](https://opensnp.org/), a platform hosting raw genotype data. In fact, he could need someone to use labeled data from [1000Genomes](http://www.internationalgenome.org/) in order to create a classifier that would tell you what's the origin of genetic data. Unfortunately, my knowledge of biology is too poor. Anyway, what I learned form this inquiry is how important domain knowledge and interdisciplinary teams are for data science and machine learning.

I chose to have a closer look at the field of education where I know a thing or two. I found a paper that dealt with undergraduate student generic problem-solving skills. It was based on an empirical study that had produced some data. It could have been used for creating a predictive model for problem solving skills performance, for detecting/classifying sub-groups of students, etc. Unfortunately, the data was not freely available. We need more Open Science! I contacted the author, but I guess he was more afraid of "losing" his data than excited about getting new tools he could use. He wanted to have my resume - that he received - but I never heard of him again.

Eventually, I stumbled upon two nice datasets that might allow to predict the sales figures of video games based on scores from critics. I [basically completed a proposal for a capstone project](https://github.com/otacke/udacity-machine-learning-engineer/blob/master/submissions/capstone_proposals/sales_prediction_for_games.md), but then I decided to pursue an idea that I had mentioned briefly ...

### Domain Background
_(approx. 1-2 paragraphs)_

_In this section, provide brief details on the background information of the domain from which the project is proposed. Historical information relevant to the project should be included. It should be clear how or why a problem in the domain can or should be solved. Related academic research should be appropriately cited in this section, including why that research is relevant. Additionally, a discussion of your personal motivation for investigating a particular problem in the domain is encouraged but not required._

In recent years, there have been many initiatives to develop and publish Open Educational Resources (OERs). Those "are any type of educational materials that are in the public domain or introduced with an open license. The nature of these open materials means that anyone can legally and freely copy, use, adapt and re-share them. OERs range from textbooks to curricula, syllabi, lecture notes, assignments, tests, projects, audio, video and animation." ([United Nations, 2016](http://www.unesco.org/new/en/communication-and-information/access-to-knowledge/open-educational-resources/what-are-open-educational-resources-oers/)) With this attitude, in 2012 the Norwegian organization _National Digital Learning Arena_ funded the developent of H5P. It is an open-source framework that allows to create, share and reuse interactive content, e.g. interactive videos or presentations with different kinds of quizzes.

For the last six month, I have been involved in the development of H5P in my spare time. Just recently, I created a new [feature for clozes that is currently pending as a pull request on github](https://github.com/h5p/h5p-blanks/pull/12). With my proposal, users could create clozes that do not necessarily require the exact answer. For example, if in a chemistry quiz someone typed "deoxiribonucleid acid" instead of "deoxyribonucleid acid", he or she probably meant the right thing. A teacher might decide that wrong spelling should not lead to a wrong answer in this case. The same goes for names such as "Schrödinger", "Schroedinger" or "Schrodinger". While you could also give alternative spellings explicitly, this might be tedious in some cases. For instance, transcribing Russian names might be tricky.

While this is basically a nice feature that [can already be tested on my blog](http://www.olivertacke.de/2017/01/02/make-h5p-fuzzy-and-fluffy/), it has a downside as [discussed on the H5P forum](https://h5p.org/node/40692). On the one hand, users can tweak the comparison of the students answer and the correct answer using some parameters. This way they can adjust the algorithms to their specific needs. On the other hand, it is not obvious for unexperienced users what the parameters do. It might be easier for them if they could just switch "fuzzy comparison" on or off. This would require the algorithms to be tuned at their best. That's what I intend to do with this project.

### Problem Statement
_(approx. 1 paragraph)_

_In this section, clearly describe the problem that is to be solved. The problem described should be well defined and should have at least one relevant potential solution. Additionally, describe the problem thoroughly such that it is clear that the problem is quantifiable (the problem can be expressed in mathematical or logical terms) , measurable (the problem can be measured by some metric and clearly observed), and replicable (the problem can be reproduced and occurs more than once)._

### Datasets and Inputs
_(approx. 2-3 paragraphs)_

_In this section, the dataset(s) and/or input(s) being considered for the project should be thoroughly described, such as how they relate to the problem and why they should be used. Information such as how the dataset or input is (was) obtained, and the characteristics of the dataset or input, should be included with relevant references and citations as necessary It should be clear how the dataset(s) or input(s) will be used in the project and whether their use is appropriate given the context of the problem._

### Solution Statement
_(approx. 1 paragraph)_

_In this section, clearly describe a solution to the problem. The solution should be applicable to the project domain and appropriate for the dataset(s) or input(s) given. Additionally, describe the solution thoroughly such that it is clear that the solution is quantifiable (the solution can be expressed in mathematical or logical terms) , measurable (the solution can be measured by some metric and clearly observed), and replicable (the solution can be reproduced and occurs more than once)._

### Benchmark Model
_(approximately 1-2 paragraphs)_

_In this section, provide the details for a benchmark model or result that relates to the domain, problem statement, and intended solution. Ideally, the benchmark model or result contextualizes existing methods or known information in the domain and problem given, which could then be objectively compared to the solution. Describe how the benchmark model or result is measurable (can be measured by some metric and clearly observed) with thorough detail._

### Evaluation Metrics
_(approx. 1-2 paragraphs)_

_In this section, propose at least one evaluation metric that can be used to quantify the performance of both the benchmark model and the solution model. The evaluation metric(s) you propose should be appropriate given the context of the data, the problem statement, and the intended solution. Describe how the evaluation metric(s) are derived and provide an example of their mathematical representations (if applicable). Complex evaluation metrics should be clearly defined and quantifiable (can be expressed in mathematical or logical terms)._

### Project Design
_(approx. 1 page)_

_In this final section, summarize a theoretical workflow for approaching a solution given the problem. Provide thorough discussion for what strategies you may consider employing, what analysis of the data might be required before being used, or which algorithms will be considered for your implementation. The workflow and discussion that you provide should align with the qualities of the previous sections. Additionally, you are encouraged to include small visualizations, pseudocode, or diagrams to aid in describing the project design, but it is not required. The discussion should clearly outline your intended workflow of the capstone project._