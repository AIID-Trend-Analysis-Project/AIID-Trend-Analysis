# Trends within Ai Journalism: An algorithmic analysis of how sentiment in reporting has changed over time

by Steven Shen, Yuxuan Chen, Shyam Sivasubramanian from George Washington University

## Introduction

The year is 2014, you turn on the news, Ukraine is at war with Russia, there is a conflict between Israel and Hamas, and Tesla  just released their new AI powered  self-driving car…and people think it’s pretty cool. Ten years in the future, while some things have remained similar, the rhetoric surrounding AI is constantly at change. 

![sentiments over time](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/f8f5dd89-6f32-4373-99e3-995fa8030e8b)


This study aims to analyze just how the sentiment and subjectivity trends have changed surrounding the reporting of AI technologies and incidents. On a broader scale, What topics are falling in and out of the news cycle? How is the sentiment and subjectivity around AI reporting? For a more nuanced answer, can we identify what sites and sources are most prominent in the AI reporting space, and how they differ in sentiment? What about the most prominent individuals who report in this space? Who are they and what are their views like?

![Reports over time](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/ce0de493-8b2d-4c2b-b438-95cda4983986)

Just as we can identify when a news article around politics is leaning towards a certain agenda or bias, there really hasn’t been much awareness and research done on this end for AI reporting. By using the AI incidents database, our project aims to take the first steps in identifying these trends over time, and shine a light on how we should be viewing all the ever rising amount of news surrounding AI.

## Methodology

This project is realizable with the help of the [AI Incident Database](https://incidentdatabase.ai). Currently, the AIID Dataset is the largest human curated and labeled resources of AI incidents with weekly updates to the incidents and reports. The data comes from a wide range of sources, consisting from news outlets, social media, forums, etc.

* Data Collection: With the help of volunteers from the AI Incident database, our analysis is done using the weekly updated reports. 
(Complete dataset available at: Main page of [AI Incident Database ](https://incidentdatabase.ai) → scroll down to the left bottom → [Download Complete Database](https://incidentdatabase.ai/research/snapshots/)

![Most common sources](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/e09bd069-3bff-490c-a44c-013f0c038cea)



Explanation of tokenization

Explanation of coherence
Explanation of topic modeling

#### Explanation of Bert and Embeddings
* [BERT (Bidirectional Encoder Representations from Transformers)](https://github.com/google-research/bert) - is a new method of pre-training language representations which obtains state-of-the-art results on a wide array of Natural Language Processing (NLP) tasks.
  
Explanation of UMAP

#### Explanation of HDBSCAN
* [HDBSCAN (Hierarchical Density-Based Spatial Clustering of Applications with Noise)](https://github.com/scikit-learn-contrib/hdbscan) - performs DBSCAN over varying epsilon values and integrates the result to find a clustering that gives the best stability over epsilon. This allows HDBSCAN to find clusters of varying densities (unlike DBSCAN), and be more robust to parameter selection.
  
#### Explanation of Vader Sentiment
* [VADER (Valence Aware Dictionary and Sentiment Reasoner)](https://github.com/cjhutto/vaderSentiment) - is a lexicon and rule-based sentiment analysis tool that is specifically attuned to sentiments expressed in social media.

  
#### Explanation of Textblob Subjectivity
* [TextBlob](https://textblob.readthedocs.io/en/dev/) 
Textblob sentiment analyzer returns two properties for a given input sentence: 
  **Polarity** is a float that lies between [-1,1], -1 indicates negative sentiment and +1 indicates positive sentiments. 
  **Subjectivity** is also a float which lies in the range of [0,1]. Subjective sentences generally refer to personal opinion, emotion, or judgment. 

## The Journey Through Data: Narrating the Insights

Visualization and Explanation of the Cluster diagram: what are the major clusters, how have the clusters shifted over time, which are the clusters of greatest interest, analysis specific topic’s subjectivity over time
Visualization of Sentiment Over Time: Plots of the clusters over time with sentiment score, top 10 most interesting
Interpreting the Visuals: Show the most interesting key findings, and the clusters of interest, can we identify key dates that are important to ai reporting across the time period
Stories Behind the Data: For each significant trend or pattern, narrate the possible underlying reasons, referencing specific AI topics or incidents where applicable.

## Making It Relevant: Connecting With the Audience

Implications for the AI Community: The understanding of trends in reporting is important for the AI community because it determines support from the public, and how our technologies are influencing people, not just as a product, but psychologically. What do people want to see more of? What is the media negative about? What are the new trends that are appearing?
What It Means for the Public: Explain the significance of these trends for the general public, including how sentiment in AI reporting might affect public opinion and awareness.

## Conclusion: Wrapping Up with Actionable Insights

Recap of Key Findings: Summarize key findings
Call to Action: As the next step, we suggest the AIID create some simple human metrics when submitting articles.
The packages we have currently used are not tooled for the specific task
If a new check box could be added to the AIID website that allows the submitter to optionally say whether an article is sensational (positive), not sensational (neutral), or sensational (negative), we will be able to more accurately determine trends in reporting.
Looking Forward: As AI becomes more ingrained into our daily lives, the need to objectively look at the technology of the future is greater than ever.
* [Flair](https://github.com/flairNLP/flair) allows applying state-of-the-art natural language processing (NLP) models to your text, such as named entity recognition (NER), sentiment analysis, part-of-speech tagging (PoS), special support for biomedical data, sense disambiguation and classification, with support for a rapidly growing number of languages.

## Potential Next Steps section 

Potential next steps include refining the analysis to uncover deeper insights, exploring additional NLP techniques. Explore ensemble modeling approaches to enhance sentiment analysis accuracy. Recommendations may also be made for improving the indexing of incident reports in the AIID and tracking discourse about AI and related harm more effectively. Expand the scope of data collection to include a broader range of sources, languages, and regions. This will provide a more comprehensive understanding of global perspectives on AI-related incidents and trends.Explore techniques for detecting and mitigating biases in media coverage of AI incidents. This could involve developing algorithms to identify biased language, assessing the impact of bias on public perception, and implementing strategies to promote balanced reporting.Analyzing cross-domain influences on media coverage can provide a more holistic understanding of the socio-cultural factors shaping perceptions of AI.

## Risk Considerations section

One potential risk is that the dataset may not contain sufficient information to adequately answer the research questions. In such cases, adjustments to the scope of the analysis or exploration of additional data sources may be necessary. Risk of bias in media reporting may influence the accuracy of sentiment analysis and trend identification.Ethical considerations arise regarding data privacy and consent in analyzing journalistic content. Additionally, potential challenges exist in interpreting and contextualizing findings within the broader landscape of AI research and development. Other risk considerations include the potential for algorithmic biases in the NLP model used for sentiment analysis, the risk of misinterpretation of results due to complex linguistic nuances, and the possibility of unintended consequences stemming from recommendations based on the analysis. Furthermore, there may be risks associated with relying solely on media reports for data analysis, such as incomplete or inaccurate information leading to flawed conclusions. 

## Supporting Sections

Glossary: term index

Methodology Appendix: technical details, here we will include more of our graphs and data

References and Further Reading: articles and reports we read and took inspiration from.
