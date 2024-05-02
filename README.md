# Trends within AI Journalism: An algorithmic analysis of how reporting has changed over time

by Steven Shen, Yuxuan Chen, Shyam Sivasubramanian from George Washington University

## Introduction

![Reports over time](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/ce0de493-8b2d-4c2b-b438-95cda4983986)

- This project explores:
  - When did AI first became a notable subject in the public eye?
  - What has fallen in and out of reporting trends?
  - How are our news sources surrounding the reporting of AI incidents potentially biased?

- Computational methods are used to analyze trends in AI journalism with data from the AI Incident Database (AIID).
- Techniques include:
  - Embedding methods.
  - Topic modeling.
  - BERT for natural language understanding.
  - Sentiment analysis.

- The analysis covers over 600 incident reports from AIID to:
  - Identify the changing trends and topics within AI Journalism.
  - Observe subjectivity of reporting sources and individuals.

- We hope this project will benefit:
  - The AI Incident Database.
  - As well as those interested in AI safety, governance, and compliance sectors.

## Data Insights
### Cluster Analysis

![All Clusters](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/dd7cf0c6-af36-465e-bd00-e8dd90e161e9)

- The above cluster visualization highlights key trends in the dataset over time. Although clustering algorithms have their limitations, we can still make some general interpretations from the axes. 
    - The X-axis loosely indicates the scope of the incident.
        - Incidents that happen to a specific group of peoples tend to lean left, while incidents that can affect everyone lean right.
    - The Y-Axis Loosely indicates the type of incident.
        - Incients involving self-drivings cars and robots tend to appear higher than those that are algorithmic and digital in nature.

![pre-2015](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/c89431bd-976a-42b6-b122-0555f18a384a)

- Before 2015, AI-related incidents were rare, with the most significant cluster concerning racism and discrimination in search algorithms and chatbots. 

![2015](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/6a9d440e-e5ac-497c-a0c9-808a285c01f5)

- From 2015, clearer trends started to emerge, reports focus on algorithmic failures towards specific races or sex.

![2016](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/6dc1ecfe-2ffa-4790-a9f4-275c6014623b)

- By 2016, there was a notable increase in media attention leading to an overall rise in number of reports

![robot cluster](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/70f572bf-f602-442e-8b7f-d4fb8382e722)

- 2015-2018 saw the formation of Robotic incidents region
    - The number of reports steadily rose until 2018
    - In Late 2017, there was a spike in sensationalism when multiple reports surrounding robots commiting suicide or being caught in tragedies
    - After this period, the number of robots surrounding robotic incidents saw a rather sharp decrease, with the region seeing little change afterwards.

![2017-2021 rightwards shift](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/cf4e2ab7-0db7-4c0f-9b7b-d3ea9fa89b67)

- From 2017 to 2021, the focus of reports shifted from targetting individuals to society as a whole. 
  - 2019, marked the most significant shift, with a noticeable decrease in incidents on the left side of the graph, indicating that the technology was maturing as more businesses and institutions adopted AI, affecting more people.

![Pre CGPT](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/6e025050-95fb-4069-8987-2892c38a35f6)

- The January 2022 Cumulative visualization marks the final time period before ChatGPT significantly alters the vizualization
  - At this point, there are significantly more incidents on the bottom right quartile vs the bottom left
  - Deepfakes, AI image generation, algorithmic moderation, and bots have begin to form it's own region
  - Self driving cars continues to be the most distinct cluster

![2022](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/d13542f1-71d5-4e6e-a258-34cd45f75286)

- ChatGPT introduced in 2022, with first clusters appearing in march, followed be a second cluster in November

![2023](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/59c269b6-7ea0-4c39-bcbc-068fd47999ed)

- 2023 saw a surge in distinct clusters that have formed as a result of ChatGPT
    - Ripple effect sees more media attention on Ai and LLMs as a whole
    - Deepfakes and Image generation also see large increases in reporting

### Media Trend Analysis
In the landscape of AI reporting, several key sources have emerged, each with its own unique contribution to the discourse. Let's take a closer look at the top 10 most frequent sources and their activity analysis:

![News](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159202579/7885ea3d-9506-4f56-b0ff-c1eb696b92de)

**The Guardian (theguardian.com)**: Leading the pack with 122 incidents, The Guardian coverage spans a wide range of topics, from social media scandals to AI's impact on law enforcement, as indicated by its most active topic keywords, including "shotspotter," "debt," and "police."  

**Active Topic Keywords for Source: theguardian.com**
| Topic Keywords        | Frequency | Subjectivity |
|-----------------------|-----------|--------------|
| shotspotter, debt, police | 21        | -0.23        |
| facebook, content, user  | 7         | -0.14        |
| ai, use, student         | 6         | -0.02        |  

The Guardian's reporting on AI-related issues spans a range of subjectivity. Topics like "shotspotter, debt, police" are approached objectively, with a subjectivity score of -0.23, indicating a predominantly factual presentation. Conversely, keywords like "ai, use, student" score -0.02, suggesting a slightly more subjective tone including some subjective elements or interpretations alongside factual information. This variation in subjectivity may reflect different reporting styles or the complexity of the topics being covered.

In 2017, Australian Department of Human Services (DHS)’s automated debt assessment system issued false or incorrect debt notices to hundreds of thousands of people, resulting in years-long lawsuits and damages to welfare recipients.

**The Verge (theverge.com)**: With 82 incidents, The Verge is a significant contributor to AI discourse. Recognized for its authoritative voice in the tech community, it provides insightful commentary and analysis on AI trends and innovations. The prominence of keywords like "tesla," "autopilot," and "driver" indicates a focus on self-driving cars and related automotive AI technologies. These focus on the developments in autonomous driving technology also suggest discussions on the capabilities and limitations of autonomous driving systems.  

**Active Topic Keywords for Source: theverge.com**
|   Topic Keywords          | Frequency | Subjectivity |
|---------------------------|-----------|--------------|
| tesla, autopilot, driver | 12        | -0.18        |
| ai, use, student          | 6         | -0.06        |
| car, vehicle, drive       | 6         | -0.11        |  

The topic "ai, use, student" with a subjectivity score of -0.06 likely embodies a subjective tone due to the ethical and privacy implications associated with the use of artificial intelligence (AI) in the context of student data and privacy. The most objective is "tesla, autopilot, driver," with a subjectivity score of -0.18. This suggests a more factual and impartial presentation of information, likely focusing on events or developments related to Tesla's autopilot system and its impact on driving.

For instance, A Tesla Model S with the Autopilot system activated was involved in a fatal crash, the first known fatality in a Tesla where Autopilot was active. 

**The New York Times (nytimes.com)**: Holding steady with 78 incidents, The New York Times maintains its reputation as a leading source of in-depth journalism. Leveraging its extensive network of reporters, it delivers comprehensive coverage of AI issues. "Ai," "use," and "student" indicate broader coverage of AI's applications and implications across different domains, including education and technology. These keywords represent discussions on AI's integration into educational settings and its implications for students and educators. "Use," "recognition," and "facial" indicate coverage of biometrics and fake facial recognition technology, focusing on AI's role in identity verification and security.    

**Active Topic Keywords for Source: nytimes.com**
| Topic Keywords          | Frequency | Subjectivity |
|-------------------------|-----------|--------------|
| ai, use, student        | 11        | -0.12        |
| use, recognition, facial| 7         | -0.30        |
| tesla, autopilot, driver| 6         | -0.20        |  

"ai, use, student" with a subjectivity score of -0.12 is more subjective, being more sensational. "use, recognition, facial" with a subjectivity score of -0.30 is relatively more objective implying discussions on the technical aspects of facial recognition technology, its usage in various contexts, and the associated challenges, leading to a more objective tone in reporting more factually

An incident in California, where students allegedly used AI to generate fake nude photos with their classmates' faces, prompting investigations by school officials and the police. The incident highlights the increasing misuse of generative AI among minors.

**The Washington Post (washingtonpost.com)**: With 60 incidents, washingtonpost.com stands out for its investigative journalism and thoughtful analysis of AI-related topics. Renowned for its insightful commentary, The Washington Post offers readers valuable perspectives on the societal implications of AI advancements. Keywords like "ai," "google," and "image" suggest discussions on AI's role in image processing and false recognition, particularly focusing in the context of Google's AI.

**Active Topic Keywords for Source: washingtonpost.com**
| Topic Keywords          | Frequency | Subjectivity |
|-------------------------|-----------|--------------|
| ai, google, image       | 7         | -0.08        |
| ai, use, student        | 5         | -0.14        |
| tesla, autopilot, driver| 5         | -0.24        |  

"ai, google, image" with a subjectivity score of -0.08 is more subjective and sensational. This suggests that the coverage may involve more opinions, interpretations, or emotional language. "tesla, autopilot, driver" with a subjectivity score of -0.24 is relatively more objective. 

A case in 2016 where Google image searches of "three black teenagers" resulted in mostly mugshot images whereas Google image searchers of "three white teenagers" consisted of mostly stock images, suggesting a racial bias in Google's algorithm. Thus, it indicates the poor coverage of visual data processing and technology. 

**Wired (wired.com)**: Rounding out the top five with 55 incidents, Wired showcases expertise in tech reporting. Renowned for insightful commentary and engaging narratives, it offers a deeper understanding of the AI landscape. Its coverage includes discussions on topics like vehicle automation and algorithmic data analysis.The presence of keywords like "car," "vehicle," and "drive" suggests that Wired focuses on automotive technologies, particularly self-driving cars and their development. These keywords likely represent discussions on the latest advancements in autonomous driving technology, as well as the challenges and opportunities associated with integrating AI into vehicles.        

**Active Topic Keywords for Source: wired.com**
| Topic Keywords        | Frequency | Average Subjectivity |
|-----------------------|-----------|----------------------|
| car, vehicle, drive   | 5         | -0.15                |
| ai, use, student      | 4         | -0.12                |
| algorithm, use, data  | 4         | -0.27                |  

"algorithm, use, data" with an average subjectivity of -0.27 is more objective and "ai, use, student" is more subjective with a score of -0.12.  

Twitter's photo cropping algorithm was revealed by researchers to favor white and women faces in photos containing multiple faces, prompting the company to stop its use on mobile platform.   

#### Subjectivity Trend
In exploration of these sources, here are the intriguing insights into the overall subjectivity levels and cluster activity across different source domains. 
| Source             | Subjectivity Level | Clusters Activity             |
|--------------------|--------------------|-------------------------------|
| The Guardian       | -0.17              | Clusters -1, 9, 6            |
| The Verge          | -0.15              | Clusters -1, 6, 27           |
| The New York Times | -0.16              | Clusters -1, 6, 46           |
| The Washington Post| -0.17              | Clusters -1, 54, 46          |
| Wired              | -0.13              | Clusters -1, 6, 48           |

**Most Objective**    
**The Guardian and The Washington Post:** The Guardian and The Washington Post are considered the most objective among the top 5 Sources as they both have the lowest subjectivity level (-0.17). The Washington Post tends to engage more with clusters such as 54 and 46 and The Guardian Post engages more with 9 and 6, which are often associated with factual reporting, suggests a focus on objective content.

![Graph](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159202579/f6e62a54-a9e1-4fb2-8677-1d08883c147e)

**Most Subjective**  
**Wired:** Wired appears to be the most subjective with a subjectivity level of -0.13, indicating a slightly higher subjectivity compared to other sources. Its engagement with clusters -1, 6, and 48 suggests a  more opinionated or subjective content.


Among these clusters, -1, 6, and 46 emerge as the most active across the sources and -1 Cluster is the cluster associated with all the sources.
![Three clusters](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159202579/f676e958-623d-4720-9ac0-e31fa45e090e)

- **Cluster -1**:
  - Focuses primarily on social media scandals, such as issues with Facebook's market or the emergence of AI-generated fake images.
  - The subjectivity score for this cluster is -0.12, indicating a slightly subjective stance in reporting.
  - The overall sentiment score is -0.52, indicating a predominantly negative opinion.
  - Most articles in this cluster are sourced from The Guardian, offering a captivating glimpse into the intersection of AI and human drama.

- **Cluster 6**:
  - Revolves around discussions on self-driving cars, particularly Teslas, and related automotive AI technologies like autopilot.
  - The subjectivity score for this cluster is -0.17, suggesting a moderately objective stance with a slight leaning towards objectivity.
  - The sentiment score is 0.12, indicating a neutral sentiment where the reporting focuses on presenting facts rather than taking sides.
  - Media reporting tends to be critical or skeptical, reflecting concerns about safety and reliability regarding the readiness of self-driving cars for widespread adoption.

- **Cluster 46**:
  - Delves into discussions about voice-controlled AI gadgets, chatbots, and the influence of YouTube videos on elections.
  - The subjectivity score for this cluster is -0.13, indicating a relatively objective perspective with a slight leaning towards objectivity.
  - The sentiment here varies, with some expressing excitement about the possibilities of these technologies while others are more skeptical.
  - Positive sentiment may reflect excitement about the possibilities of voice-controlled AI gadgets, while negative sentiment and negative sensationalism indicates skepticism or concerns about their efficacy.

      ![Screenshot 2024-04-26 120241](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159202579/cccf5d96-ab81-4c32-a04c-29a933681a22)
 
In the dynamic world of AI, key topics like "Tesla," "autopilot," and "driver" dominate discussions, reflecting the automotive industry's evolution. Alongside, debates around "ai," "use," and "student" highlight AI's integration in education, while "ai," "google," and "image" spark conversations on visual data processing. From "use," "recognition," and "facial" in biometrics to "facebook," "content," and "user" in social media dynamics and "shotspotter," "debt," and "police" delving into the intersection of AI and law enforcement, each keyword offers a glimpse into AI's diverse impact on society, shaping dialogues on safety, education, and digital interaction. As the conversation unfolds, these topics continue to shape the future of technology and society, driving us towards new horizons of possibility and discovery.

### Author Contribution Analysis
##### **Top 3 Contributing Authors in All Cluster**
| Authors  | Frequency |
| ------------- | ------------- |
| BBC News  | 22  |
| James Vincent  | 21  |
| Reuters  | 20  |
| Associated Press  | 19  |
| Katyanna Quach  | 12  |
| Andrew J. Hawkins  | 11  |
| Tom Simonite  | 11  |
| Fred Lambert  | 10  |
| Kashmir Hill  | 10  |
| Maggie Harrison  | 10  |

* Among the top 10 prominent authors, there are 3 news agencies and 7 individual authors. 

![Picture1](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159200995/381e46c4-9a37-4262-bc81-a69c7c062582)

* BBC News, Associated Press, and Reuters are the top 3 news agencies. By comparing their average subjectivity score, we can observe that BBC News is the most subjective news agency (-0.14), Reuters is the most objective news agency (-0.23), and Associated Press is in the middle with a subjectivity score of -0.19. 

![Picture2](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159200995/13719951-600d-44fa-8c2f-1d58b57e8291)

* By looking at the top 7 individual authors average subjectivity score, we can conclude that Maggie Harrison is the most subjective author (-0.09), and Tom Simonite is the most objective author (-0.17). 


##### **Top 10 Common Topic Keywords among Top 10 Authors**
| Topic Keywords  | Frequency |
| ------------- | ------------- |
| tesla, autopilot, driver  | 23  |
| ai, google, image  | 10  |
| car, vehicle, drive  | 10  |
| ai, model, chatgpt  | 8  |
| ai, use, student  | 8  |
| use, recognition, facial  | 7  |
| facebook, content, user  | 5  |
| sport, arena, missile  | 4  |
| robot, worker, google  | 4  |
| ad, facebook, user   | 3  |

* Among the top 10 prominent authors, there are top 10 common topic keywords that they are generally focusing on which they talked about “Tesla, autopilot, driver” for 23 times. 

![Picture3](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159200995/6c484f50-7c6c-4a7e-846e-5f7870033b76)

* When these top 10 prominent authors talk about “ai, model, chatgpt”, they tend to be the most subjective (subjectivity score of -0.06). When they are talking about “robot, worker, google”, they tend to be the most objective (subjectivity score of -0.32).

## Conclusion: Wrapping Up with Actionable Insights
This project embarked on a comprehensive analysis of trends of of how sentiment in reporting has changed over time, leveraging a multifaceted approach rooted in natural language processing (NLP) techniques and machine learning models.

Utilizing Latent Dirichlet Allocation (LDA), the project identified latent topics within the corpus of AI-related incidents. By evaluating coherence scores, the optimal number of topics was determined, providing insights into the thematic trends prevalent in media reporting on AI.
Furthermore, the integration of DistilBERT embeddings facilitated the generation of dense, context-aware representations of the text data. These embeddings were visualized using UMAP and clustered using HDBSCAN, enabling the exploration of underlying structures and relationships within the corpus.Sentiment analysis, conducted through TextBlob and VADER, contributed to a nuanced understanding of the emotional tone and perception surrounding AI-related incidents. Polarity and subjectivity scores provided insights into shifts in sentiment over time and variations across different publications.

Understanding sentiment patterns and media discourse surrounding AI is crucial for accurately capturing and indexing AI-related incidents, ultimately contributing to the advancement of AI ethics and safety. Addressing risks such as bias in media reporting, the risk of misinterpretation of results due to complex linguistic nuances, and the possibility of unintended consequences stemming from recommendations based on the analysis, potential for algorithmic biases in the NLP model used for sentiment analysis, and ethical considerations will be essential to ensure the integrity and validity of future analyses. One of the main risk includes the model sticking on to the English language, which when included with other languages might shift the insights.

### Key Findings:
1. The analysis revealed shifting trends in AI reporting over time, from rare mentions before 2015 to a significant increase in media attention post-2015. This shift corresponded with the emergence of self-driving cars, algorithmic biases, and societal impacts as prominent topics in AI journalism.

2. The topics using LDA ranged from physical AI incidents like autonomous vehicles to digital issues such as deepfakes and misinformation bots, reflecting the diverse landscape of AI journalism.

3. Clusters related to social media scandals, self-driving cars, and voice-controlled AI gadgets emerged as prominent themes, each with its unique sentiment, subjectivity and focus.
  
4. The top media domains contributing to AI reporting included theguardian.com, theverge.com, nytimes.com, washingtonpost.com, and wired.com and by prominent indivuals: BBC News, James Vincent, and Reuters majorly revolved around Keywords such as "Tesla," "autopilot," "AI images," "ChatGPT," and "face IDs", reflecting key topics driving media coverage of AI incidents.

5. The Guardian and The Washington Post are found to be the most objective among the top 5 sources, with subjectivity levels of -0.17.
Wired appears to be the most subjective among the top sources, with a subjectivity level of -0.13.Among the top individual authors, Maggie Harrison is the most subjective (-0.09), while Tom Simonite is the most objective (-0.17).

6. "Tesla, autopilot, driver" is the most common topic keyword among the top authors, reflecting a significant focus on autonomous driving technology.
Discussions on "ai, model, chatgpt" tend to be more subjective, while those on "robot, worker, google" are more objective.

7. Sentiment analysis using TextBlob and VADER unveiled fluctuations in the emotional tone of AI reporting across different clusters. While some clusters maintained a neutral sentiment, particularly those addressing social media scandals, others, such as those concerning self-driving cars and digital issues, exhibited more negative sentiment. This negativity suggests a level of skepticism or concern, particularly regarding the safety and reliability of autonomous vehicles. Interestingly, despite the sensational nature of social media scandals, media reporting tended to remain neutral, prioritizing factual presentation over opinion. These findings underscore the nuanced nature of public perception surrounding AI-related incidents and highlight the importance of considering emotional context in media analysis.


### Call to Action: 
As the next step, we suggest the AIID create some simple human metrics when submitting articles.
The packages we have currently used are not tooled for the specific task
If a new check box could be added to the AIID website that allows the submitter to optionally say whether an article is sensational (positive), not sensational (neutral), or sensational (negative), we will be able to more accurately determine trends in reporting.

### Looking Forward: 
As AI becomes more ingrained into our daily lives, the need to objectively look at the technology of the future is greater than ever.
* [Flair](https://github.com/flairNLP/flair) allows applying state-of-the-art natural language processing (NLP) models to your text, such as named entity recognition (NER), sentiment analysis, part-of-speech tagging (PoS), special support for biomedical data, sense disambiguation and classification, with support for a rapidly growing number of languages. Potential next steps include refining the analysis, exploring additional NLP techniques, and expanding the scope of data collection to include a broader range of sources, languages, and regions.This could involve developing algorithms to identify biased language, assessing the impact of bias on public perception, and implementing strategies to promote balanced reporting.
  


# Supporting Sections

## Glossary and Term Index
A

    AI (Artificial Intelligence): Technology enabling machines to mimic human behavior and intelligence.
    AIID (AI Incident Database): A database that tracks incidents involving AI technologies.

B

    BERT (Bidirectional Encoder Representations from Transformers): A deep learning model designed to understand the context of words within text by processing data from both directions (left-to-right and right-to-left) simultaneously.

C

    Clustering: The process of grouping a set of objects in a way that objects in the same group are more similar to each other than to those in other groups.
    Coherence Score: A measure used in topic modeling to evaluate the semantic similarity between high scoring words within a topic.
    Cumulative Cluster Diagram: A visualization that aggregates clustering data up to a specific point in time to show trends and developments.

D

    Dataframe: A two-dimensional data structure in Python’s Pandas library, where data is aligned in a tabular fashion in rows and columns.

E

    Embeddings: Numeric representations of words and phrases that capture their meanings, context, relationships, and properties.
    UMAP (Uniform Manifold Approximation and Projection): A dimensionality reduction technique used to simplify the complexity of high-dimensional data while retaining its general structure for analysis.

G

    Gensim: A Python library used for topic modeling and document similarity analysis within Natural Language Processing (NLP).

H

    HDBSCAN (Hierarchical Density-Based Spatial Clustering of Applications with Noise): An algorithm used for clustering data points based on density.

L

    LDA (Latent Dirichlet Allocation): A type of statistical model that allows sets of observations to be explained by unobserved groups that explain why some parts of the data are similar.

N

    NLP (Natural Language Processing): A field of AI focused on the interaction between computers and humans through natural language.

P

    Pandas: A Python library for data manipulation and analysis, providing data structures and operations for manipulating numerical tables and time series.
    Plotly Express: A high-level interface for creating interactive and animated visualizations in Python.

S

    Sentiment Analysis: The process of determining the emotional tone behind a series of words to gain an understanding of the attitudes, opinions, and emotions expressed within an online mention.
    Subjectivity: Refers to how someone's judgment is shaped by personal opinions and feelings instead of outside influences.

T

    TextBlob: A Python library for processing textual data, including capabilities for sentiment analysis.
    Tokenizing: The process of converting a text into smaller units called tokens, which can be either words, characters, or subwords.

V

    VADER (Valence Aware Dictionary and Sentiment Reasoner): A lexicon and rule-based sentiment analysis tool that is specifically tuned to sentiments expressed in social media.

## Methodology

This project is realizable with the help of the [AI Incident Database](https://incidentdatabase.ai). Currently, the AIID Dataset is the largest human curated and labeled resources of AI incidents with weekly updates to the incidents and reports. The data comes from a wide range of sources, consisting from news outlets, social media, forums, etc.

If you wish to run this code yourself, Below is the download link to the latest snapshot
(Complete dataset available at: Main page of [AI Incident Database ](https://incidentdatabase.ai) → scroll down to the left bottom → [Download Complete Database](https://incidentdatabase.ai/research/snapshots/)
Within the weekly backup, we have used Incidents.csv and Reports.csv.

### Initial cleaning
Tools Used: Pandas for creating and manipulating the dataframes.
What Happens: Importing the data, formating and cleaning it.

Concating the csvs: Adding the incidents to their respective reports.
Filtering:removal of all non-english reports from the dataset and unused/redundant columns, as our current packages are unable to handle foreign languages.

Importance: Allows for the further analysis and manipulation of the data

### Preprocessing
Tools Used: Libraries like nltk for cleaning and tokenizing, and gensim for creating dictionaries and the bag-of-words models.
What Happens: The initial stage of processing text data involves preparing the raw text so it can be analyzed effectively.

Cleaning the Text: The text is cleaned by removing any characters that are not useful (like punctuation and numbers) and converting all text to lowercase. This helps standardize the text, making it easier for the software to process.
Tokenizing the Text: This step involves breaking down the text into individual words or phrases. This is crucial because it turns large blocks of text into manageable pieces for analysis.
Creating a Dictionary: After tokenizing, each unique word is cataloged in a dictionary where each word is assigned a unique identifier. This makes it easier to reference words quickly.
Bag-of-Words Model: Converts text documents into a simple numerical representation where each document is described by the frequency of words that appear in it. Imagine counting how many times each word appears and then writing down those counts instead of the words themselves.

Importance: These steps clean and convert text into a format that computer algorithms can process, setting the stage for deeper analysis.

### Topic Keyword Generation
Tools Used: gensim library for implementing the LDA model.
What Happens: This process identifies themes or topics within the collection of texts.

LDA Model: Latent Dirichlet Allocation (LDA) is a statistical model that helps discover hidden thematic structures in large text corpora. It assumes documents are mixtures of topics and topics are mixtures of words.
Topic Representation: Each topic identified by LDA is characterized by words that are most frequent in those topics. These frequently occurring words are used as keywords to describe each topic.

Importance: Identifying topics helps in understanding the main themes in large volumes of text without needing to read them in detail.

### Determining the Optimal Number of Topics
Tools Used: gensim provides ways to compute LDA models and coherence scores.
What Happens: Deciding how many topics best represent the data.

Iterative Modeling: The notebook runs multiple LDA models, each time with a different number of topics, to see which model performs best.
Coherence Score: A coherence score measures how semantically similar the high-scoring words in a topic are. A higher coherence score means the topics are more meaningful and interpretable.

Importance: Finding the right number of topics ensures that the model is both accurate and interpretable, not too broad and not too granular.

### Embeddings and BERT Generation Process
Tools Used: transformers library by Hugging Face is used to implement BERT.
What Happens: Converts words or sentences into numeric vectors that represent their underlying meanings.

BERT Model: BERT (Bidirectional Encoder Representations from Transformers) is a sophisticated deep learning model designed to capture the context of words in text.
Embedding Vectors: BERT outputs vectors (lists of numbers) for each word, which encapsulate much more information about that word’s use and meaning than the word alone.

Importance: These embeddings are crucial for allowing machines to understand language in a more human-like way, enabling more complex text analysis.

### Clustering Using Embeddings
Tools Used: UMAP is used for reducing the dimensionality of the embeddings and HDBSCAN is used for performing the actual clustering based on the density of data points.
What Happens: Documents are grouped based on their semantic similarities, which are captured through embeddings, to uncover underlying patterns or themes.

Dimensionality Reduction with UMAP: Before clustering, UMAP reduces the high-dimensional embeddings to a more manageable two-dimensional space while attempting to preserve both local and global structures of the data. This step makes clustering more effective and the results easier to visualize and interpret.
Clustering with HDBSCAN: HDBSCAN, a clustering algorithm, then processes these reduced embeddings. Unlike K-means, HDBSCAN does not require specifying the number of clusters beforehand and is adept at identifying clusters of varying densities. It groups documents into clusters where members are more similar to each other than to documents in other clusters. It's particularly effective for data with an unknown number of clusters and varying cluster sizes.

Importance: this is the key step in clustering, given the pipeline requirements for this project, we have used HDBSCAN to algorithmically determine the optimal number of clusters, so that even if the dataset significantly changes in the future, the code should still hold a certain level of accuracy, and wont require manual tuning of the parameters.

### Data Preparation and Time-Based Analysis
Tools Used: The Pandas library in Python, for data manipulation.
What Happens: The dataset is prepared for detailed time-based analysis, including converting date formats and sorting.

Datetime Conversion: Ensures all date-related fields are standardized to datetime objects for consistent processing and analysis.
Sorting: The DataFrame is organized chronologically to facilitate temporal analysis and visualization.

Importance: Proper date handling and sorting are essential for accurate time-series analysis and for maintaining the integrity of chronological data in visualizations.

### Visualization Using Plotly
Tools Used: Plotly Express, which provides high-level API for creating interactive and animated plots efficiently.
What Happens: Creates a dynamic and static interactive visualizations of clustering, showcasing the evolution of data clusters.

Global Range Calculation: Computes consistent spatial boundaries for all frames to ensure uniform scaling in animations.
Buffer Addition: Adds spatial buffers to prevent data points from appearing on the edges of plots, enhancing visual clarity.
Color Mapping and Animation Setup: Distinguishes clusters by color and configures animation settings to enhance interactivity and understandability.
Animation Execution and Display: The animation is rendered, showing how clusters change over time, with controls for exploring different time frames interactively.

Importance: The dynamic visualization enables viewers to observe and understand temporal patterns and cluster dynamics visually, which is crucial for identifying trends and making informed decisions based on evolving data landscapes.

### Explanation of Sentiment Analysis
Sentiment analysis is one of the most widely known Natural Language Processing (NLP) tasks that determine the emotional value of a given expression in natural language. It usually helps a business to understand the social sentiment of their brand, product or service while monitoring online conversations. Here with the use of sentiment analysis, we are able to observe sentiment among AI incidents over time. It is essentially a multiclass text classification where the given input text is classified into positive, neutral, or negative sentiment.

### Explanation of Vader Sentiment
* [VADER (Valence Aware Dictionary and Sentiment Reasoner)](https://github.com/cjhutto/vaderSentiment) - is a lexicon and rule-based sentiment analyzer that specifically attuned to social media sentiment expression. 
Vader sentiment returns the probability of a given input sentence to be compound, positive, negative, and neutral by using a list of lexical features (e.g. word) according to their semantic orientation to calculate the text sentiment. 
The limitation of VADER is that the method only focuses on individual words and completely ignores the context in which it is used. 
  
### Explanation of Textblob Subjectivity
* [TextBlob](https://textblob.readthedocs.io/en/dev/) 
Textblob sentiment analyzer returns two properties for a given input sentence: 
  **Polarity** is a float that lies between [-1,1], -1 indicates negative sentiment and +1 indicates positive sentiments. 
  **Subjectivity** is a float which lies in the range of [0,1]. Closer to 1 means the most subjective while closer to 0 means the most objective. Subjective sentences generally refer to personal opinion, emotion, or judgment. 
The limitation of TextBlob is that it will only consider words and phrases that it can assign polarity to and averages to get the final score, ignoring the words that it doesn’t know. We rescale the original range [0,1] into -1 to 1 for better interpretability. The closer to 1 means more subjective, closer to -1 means more objective. 



* References and Further Reading: articles and reports we read and took inspiration from - [Literature Reviews on Media Biases](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/blob/89e6f5484b7d635843586eb6cb35bc4a0b676bf5/Literature%20Reviews%20on%20Media%20Biases.pdf)

## Contact Information

by Steven Shen (stevenshen2000@gmail.com), Yuxuan Chen (yuxuan.chen@gwu.edu), Shyam Sivasubramanian (shyam.sivasubramanian@gwu.edu)
