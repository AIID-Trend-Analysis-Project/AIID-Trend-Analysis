# Trends within Ai Journalism: An algorithmic analysis of how sentiment in reporting has changed over time

by Steven Shen, Yuxuan Chen, Shyam Sivasubramanian from George Washington University

## Introduction

Almost everyone is talking about AI since OpenAI’s public launch of ChatGPT, AI has become one of the trendiest topics taking over every facet of our lives, but have you ever wondered when did AI enter the public consciousness? How has opinion changed on the topic over time? What topics are falling in and out of the news cycle? How is the sentiment and subjectivity around AI reporting? As we can identify when a news article around politics is leaning towards a certain agenda or bias, there really hasn’t been much awareness and research done on this end for AI reporting. 

By answering these questions, the project aims to computationally analyze the changing trends and rhetoric in AI journalism using data from the AI Incident Database (AIID). By leveraging natural language processing (NLP) techniques such as topic modeling, BERT, sentiment analysis, and embedding, the goal is to uncover insights into how the media reports incidents and harms related to AI over time. 

Introduction to the challenges and importance of analyzing media coverage of AI, explanation of the need for sentiment analysis in understanding public perception and overview of the specific research questions addressed in the project are the main problem understandings dealt here.

By examining over 600 incident reports indexed by AIID, the project seeks to understand shifts in sentiment, language usage, and thematic trends in media coverage surrounding AI systems. The findings will not only benefit the AIID but also inform stakeholders in AI safety, governance, and compliance.


![sentiments over time](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/f8f5dd89-6f32-4373-99e3-995fa8030e8b)


![Reports over time](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/ce0de493-8b2d-4c2b-b438-95cda4983986)


## Data Insights
### Cluster Analysis

![All Plots](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/b98cbe6a-2dc6-43bc-af5e-35669e641b8f)
The above cluster visualization highlights key trends in the dataset over time. Although clustering algorithms have their limitations, we can still make some general interpretations from the axes. Clusters at the top generally relate to physical AI incidents, such as autonomous Teslas, robots, and other machines operating independently with AI systems. Moving downward, the focus shifts towards more digital issues, including problems with deepfakes, AI-generated images, and errors in AI conversations like those in ChatGPT.

To the left of the graph, we see incidents often linked to location-specific issues, like failures in facial recognition software to detect certain skin tones or problems that are unique to specific countries. On the right, the issues are broader, affecting overall technology sectors like High-Frequency Trading (HFT) algorithms and automated systems in banking and education. This area of the graph sometimes struggles to accurately capture issues related to race, geography, and gender when they aren't clearly mentioned in the articles.

![Pre-2015](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/d92d5c02-3dc4-4e31-8142-01ea19518f3c)
Before 2015, AI-related incidents were rare, with the most significant cluster concerning racism and discrimination in search algorithms and chatbots. 

![2015-2016 scatter plot](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/e2f8ffb4-b544-4c87-820e-0aa1629c8773)
From 2015, clearer trends started to emerge, including early reports on Google’s self-driving cars and predictive policing. By 2016, there was a notable increase in media attention, with more reports on self-driving cars and a rise in recognition of algorithmic biases, like those affecting Pokémon Go's geographic preferences.

![Traditional Robotics](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/42017f24-59c2-4247-a22b-6aa7f041382f)
Between mid-2015 and late 2017, while the general trend of articles remained the same, there was a clear increase in traditional robotics-related incidents. One interesting point of note, however, is that after 2018, the robotics clusters largely stagnate, and seems to have fallen out of the interest of the news cycle, despite the constantly expanding tesla cluster.

![2017-2021 Left to Right Shift](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/1dd91929-59a8-40ea-8dc0-c841c45a4e93)
From 2017 to 2021, the focus of reports shifted from digital and geographic issues to broader technological and societal impacts. In 2019, particularly, there was a noticeable decrease in incidents on the left side of the graph, indicating that the technology was maturing as more businesses and institutions adopted AI, affecting more people.

![2022 Start Cumulative](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/c970e139-2ec3-448e-a87d-fa1e0b73e050)
2022 marked a notable shift in the reports gathered by the AIID. Before we proceed, let's review the cumulative cluster diagram from the beginning of the year. By this time, self-driving vehicles had become a regular topic in news reports, forming the most distinct cluster. Additionally, there was a significant increase in reports on AI incidents impacting society at large, beyond just racial and gender-based issues. Reports on Deepfakes, bot misinformation in social media, and other harmful AI-powered technologies also started to form their own distinct clusters.

![2022 2023 CLusters](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/158225645/cceedf11-4338-4154-8b82-a34bf9e2d9ee)
The introduction of ChatGPT in 2022 saw the formation of multiple new clusters within the dataset. As the attention of ChatGPT entered the public eye, It seems to have had a ripple effect on Large Language Models (LLMs) and chatbots, as well as adjacent technologies such as deepfakes and misinformation bots.

While we dive into the nitty-gritty, let's take a gander at the top five source domains that are setting the stage on fire with their hot takes and sizzling reports.
First up on the podium, we've got theguardian.com strutting its stuff with a whopping 122 incidents to its name. The Guardian ain't pulling no punches when it comes to AI chatter, and boy, do they know how to stir the pot. Next in line, we've got theverge.com stepping into the ring with 82 incidents of its own. If there's one thing The Verge knows how to do, it's capturing the pulse of the tech scene, and AI is no exception.
![Top 5 domains](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159202579/f7873644-0987-43f8-9fca-d0ffd35f8ba2)
Sliding into third place, we've got nytimes.com holding its ground with 78 incidents. The New York Times isn't just about breaking news; it's about breaking barriers, and AI is just another notch on its journalistic belt. Not too far behind, we've got washingtonpost.com making waves with 60 incidents. The Washington Post isn't afraid to tackle the tough topics, and when it comes to AI, they're diving headfirst into the digital deep end. And we've also got wired.com rounding out the top five with 55 incidents. Wired knows how to wire up a story, and when it comes to AI, they're plugged in and ready to roll.

The top three active clusters are lighting up the AI universe like a digital bonfire!
![cluster](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159202579/a73d7352-e9b3-460f-86ca-3c291a87135a)
![Three clusters](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159202579/daa030c3-e373-4df9-86e4-e40f868f6162)

 The Cluster -1 corner of the AI universe is where all the juicy social media scandals hang out. You know, like when Facebook's market took a tumble or those sneaky AI-generated fake images started popping up. It's like the TMZ of the AI world, always dishing out the latest gossip. Now, here's the twist: despite all the drama, the sentiment here is surprisingly neutral.The pulse of social media scandals beats relentlessly.From Facebook's market turbulence to the emergence of deceitful AI-generated imagery, every revelation adds fuel to the fire of intrigue.Cluster -1 remains a captivating glimpse into the intersection of AI and human drama.

 Cluster 6 is a bunch of gearheads huddled around, chatting about self-driving cars, especially those sleek Teslas. Yep, we're talking about autopilot, car driving tech, and all things car-related. The sentiment here? Well, it's a bit on the negative side. Seems like not everyone's convinced that self-driving cars are ready for prime time. But hey, that's the beauty of a good debate, right?
 
![Picture1](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159202579/32b4748c-3001-4091-a10c-4f42760b5a5e)
 
While zooming into Cluster 46. Imagine a bunch of tech geeks deep-diving into voice-controlled AI gadgets, debating over chatbots, and even pondering whether YouTube videos have the power to sway elections. It's like a tech talk show on steroids! The sentiment here? It's a mixed bag. Some folks are all hyped up about the possibilities, while others are a bit skeptical. 



![Top 3 Authors](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159200995/371fd9c8-4417-4501-b4d0-d2a25ed19756)

The 3 most prominent individual authors are BBC News, James Vincent, and Reuters. The average VADER and Textblob Subjetivity scores are shown on the chart above. James Vincent seems to have the most positive VADER sentiment score while other two authors have relatively negative VADER sentiment score.

![Top 3 Cluster](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159200995/eb4ca9ef-8d2e-490b-aa5a-26c913e58d9c)

Among these 3 authors, the most active clusters are -1, 6, and 40. The average VADER and Textblob Subjetivity scores of each cluster are shown on the chart above.

![Top 10 topics](https://github.com/AIID-Trend-Analysis-Project/AIID-Trend-Analysis/assets/159200995/4bffcd38-a6fb-4b74-a37f-70e05cfdba85)

Among these 3 authors, the top 10 keywords topics are illustrated as above. They are contributing a lot of AI trendy topics such as Tesla, AI Images, Face IDs, Chatgpt, and etcs. 

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
The limitation of TextBlob is that it will only consider words and phrases that it can assign polarity to and averages to get the final score, ignoring the words that it doesn’t know.



References and Further Reading: articles and reports we read and took inspiration from.

## Contact Information

by Steven Shen, Yuxuan Chen, Shyam Sivasubramanian
