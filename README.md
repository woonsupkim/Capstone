# Central Garden & Pet: NLP Model for Online Customer Reviews
 
Industry: Retail
In this project, you will build a Natural Language Processing (NLP) sentiment analysis model to help a national retailer understand its customers' feedback, generate new product ideas, monitor compliance, and improve its website. The results of this project will help the sponsor build its internal capabilities and create a better customer experience.


## Background
The client wants to develop a reproducible analytical procedure to utilize customer reviews to extract useful insights such as customer satisfaction and product strategies.

## Project Roadmap 
I.  Data understanding & preparation
1.  Explore and understand pre-processing steps
	We will conduct a thorough EDA on the data and detect any issues that may impair the accuracy and integrity of the whole analysis. For instance, upon our initial examination, there are some issues with the raw dataset including mixes of upper & lower cases, review duplicates, and price recorded as 0. Understanding the pre-processing tools applicable to our case will impact how the dataset is going to be prepared for further analysis. 

2.  Feature Engineering (company-level data)
	Regarding data quality issues found, we will take necessary actions accordingly. For example, we can unify category names, parse data, or lump them into smaller categories. This step is to reduce possible review cases that may not get analyzed in the process of NLP.


II. Modeling
1. Split data into train-valid-test using Cross-validation method (80%:10%:10%)

2. Execute the following on the train dataset (explained in detail in the Methodology section)
	i) Zero-Shot text classification
   Categorize text data into several predefined labels and compute scores for each category to represent how relevant each review is to the categories.
ii) Few-Shot text classification
     Improve upon the previous Zero-Shot classification by tuning with already labeled data and increasing topic relevance.
iii) Sentiment Analysis
    Add a sentiment angle to the previous steps. Through this step, texts will be both classified into categories and labeled either negative, positive, or neutral.
iv) N-gram (Bigram and Trigram)
      Tokenize two or three words together that are tailored to the Sponsor’s business. This will enhance the model by being able to detect insights that are otherwise negligible. 

III. Performance monitoring & readjustments
1. Evaluate initial Few-Shot text classification on the validation set, and measure performance using discussed metrics 
2. Input different labeled data for different tuning with Few-Shot text classification
3. Repeat Sentiment Analysis, N-gram, and evaluate on the validation set to measure performance
4. Iterate these steps several times and pick the best resulting Few-Shot classification strategy

IV. Development
Apply the selected model to the test set and evaluate its performance using discussed metrics. This will be the final phase where we will be able to see how effective our final model can be when reproduced for future analysis needs.

V. Final Deliverables 
After completing each modeling process, we will conclude the section with deliverables for the model that include research documents entailing details of the methodology, presentation of key findings, reproducible codes, and processed dataset. 
