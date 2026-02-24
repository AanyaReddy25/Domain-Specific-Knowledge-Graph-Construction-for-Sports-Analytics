## KNOWLEDGE GRAPH CONSTRUCTION FROM TEXT USING NLP

## Introduction
This project aims to extract useful information from unstructured text and represent it in the form of a knowledge graph. Using a Wikipedia article on UEFA Euro 2024, natural language processing techniques are applied to identify important entities and the relationships between them. The generated knowledge graph helps in visualizing and understanding connections between different entities present in the text.

## Objective
The objective of this project is to automatically extract named entities and relationships from text data and construct a knowledge graph that represents these relationships in a structured and visual form.

## Data Description
The dataset used in this project is an HTML file of a Wikipedia page related to UEFA Euro 2024. The text content is extracted from paragraph tags and combined into a single document for further processing.

## Data Preprocessing
The HTML file is parsed using BeautifulSoup to extract textual content. Very small or irrelevant paragraphs are removed. The cleaned text is then processed using the SpaCy language model for tokenization and named entity recognition.

## Exploratory Data Analysis
Basic analysis is performed to observe the total number of characters and the types of named entities detected in the text. The frequency of different entity types is counted to understand the nature of information present in the document.

## Model Building
Named entities are extracted using SpaCy’s pre-trained model. Relationships between entities are identified based on verbs and sentence structure. These entity–relation–entity triples are used to build a directed graph using NetworkX. The graph is pruned to remove weak connections and then visualized. The final graph is also exported as CSV files for further use.

## Model Evaluation
The quality of the model is evaluated using visual inspection of the generated knowledge graph. The number of nodes and edges is checked, and the relationships are examined to ensure they meaningfully represent the information present in the text.

## Conclusion
The project successfully demonstrates how unstructured text can be converted into a structured knowledge graph using NLP techniques. The generated graph helps in visualizing relationships between entities and can be further used for knowledge-based applications and analysis.
