# NLP Project

This repository contains code for an NLP (Natural Language Processing) project. The project focuses on analyzing tweets related to the Russia-Ukraine conflict using various NLP techniques. The goal is to identify contradictory or hypocritical tweets made by the same user.

## Getting Started

To get started with the project, follow the instructions below.

### Prerequisites

Make sure you have the following dependencies installed:

- transformers
- vaderSentiment

You can install these dependencies using the following command:

`!pip install transformers vaderSentiment`


### Dataset

The dataset used for this project is available on Kaggle and can be downloaded using the provided link: [Russia-Ukraine Conflict Dataset](https://www.kaggle.com/aneeshtickoo/russia-ukraine-conflict). The dataset contains tweets related to the Russia-Ukraine conflict.

### Installation

1. Clone the repository:
`git clone https://github.com/your-username/nlp-project.git`

2. Change into the project directory:
`cd nlp-project`


3. Install the required dependencies:
`pip install -r requirements.txt`


4. Download the dataset and unzip it:
`kaggle datasets download aneeshtickoo/russia-ukraine-conflict`\
`unzip russia-ukraine-conflict.zip`


5. Start the Jupyter Notebook:

6. Open the `nlp-project.ipynb` notebook and run the cells to execute the code.

## Project Description

The project performs the following steps:

1. Data Preparation:
- Reads the dataset containing tweets from the Russia-Ukraine conflict.
- Filters the dataset to include only English tweets.
- Selects the required columns for analysis.

2. NER (Named Entity Recognition):
- Uses a pre-trained BERT model for NER to identify named entities in the tweets.
- Stores the NER results in a separate column in the dataframe.

3. Sentiment Analysis:
- Utilizes the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analysis tool.
- Calculates sentiment scores for each tweet and stores the results in the dataframe.

4. Finding Contradictory Tweets:
- Implements functions to calculate similarity and sentiment scores between tweets.
- Searches for the most contradictory tweet made by the same user.
- Outputs the contradictory tweet for a given user ID.

## Results

The project provides insights into contradictory or hypocritical tweets made by users regarding the Russia-Ukraine conflict. By analyzing the named entities and sentiment scores, it identifies tweets that contradict each other. The contradictory tweet for a given user ID can be obtained by calling the `find_tweets()` function.

## Contributing

Contributions to the project are welcome. If you have any suggestions or improvements, please create a pull request or open an issue.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- The [transformers](https://github.com/huggingface/transformers) library for providing pre-trained NER models.
- The [vaderSentiment](https://github.com/cjhutto/vaderSentiment) library for sentiment analysis.
- [Aneesh Tickoo](https://www.kaggle.com/aneeshtickoo) for providing the Russia-Ukraine conflict dataset on Kaggle.

