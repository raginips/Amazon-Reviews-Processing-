# NLP - Amazon reviews: Sentiment Analysis & Text Mining

## 👤 Author
* **Name:** Ragini PS
* **Course:** NLP - Project
## 📌 Project Overview
This repository contains a comprehensive Natural Language Processing (NLP) pipeline for exploring, preprocessing, and performing advanced text mining on product review data. The project takes raw text reviews and extracts semantic patterns, emotional sentiments, and latent topics using machine learning techniques.

## 🛠️ Key Features & Workflow

### 1. Data Exploration & Sentiment Engineering
* Handled missing metrics and isolated primary textual features (`reviews.text`, `reviews.rating`).
* Built custom mapping logic to translate continuous numeric product ratings (\(1 \rightarrow 5\)) into discrete categorical sentiments (`positive`, `neutral`, `negative`).

### 2. Rigorous Text Preprocessing Pipeline
* Structural cleaning via Regular Expressions (removal of HTML tags, formatting artifacts, and special characters).
* Global lowercase standardisation.
* Full linguistic tokenization.
* English stop-word filtration alongside WordNet Lemmatization to extract stable semantic roots.

### 3. Exploratory Text Visualization
* Distribution tracking of sentiment slices using Seaborn charts.
* Comparative corpus-level insights via sentiment-grouped **Word Clouds**.
* Structural analysis relating document length (word count) across target score distributions.

### 4. Advanced NLP & Machine Learning
* Text vectorization utilizing **TF-IDF Matrix Generation** (tuned for top 1000 statistical features).
* Unsupervised Generative Latent Semantic Analysis using **Latent Dirichlet Allocation (LDA)** for thematic extraction.
* Document clustering optimization via **K-Means Clustering**.
* Custom algorithmic tracking of word token pairings to compute and map a structural **Word Co-occurrence Matrix**.

## 📁 Repository Structure
```text
├── 7817_1.csv            # Target raw dataset containing product reviews (ensure paths match)
├── nlp_assignment_1.py   # Primary consolidated production-ready Python execution script
├── requirements.txt      # Automated pip package dependencies management manifest
└── README.md             # Project roadmap and technical overview document

## 🚀 Getting Started

### Prerequisites
Make sure you have Python 3.8+ installed on your local environment.

### 1. Clone the repository
```bash
git clone https://github.com
cd YOUR_REPOSITORY_NAME
```
### 2. Install dependencies
Install all required libraries automatically using the provided manifest:
```bash
pip install -r requirements.txt
```
### 3. Run the analysis pipeline
Execute the production script to clean data, run models, and render visualizations:
```bash
python nlp_assignment_1.py

## 📊 Summary of Extracted Insights (Sample Output)
* **Dataset Scale:** 1,597 total records analyzed across 27 initial operational data vectors.
* **Dominant Sentiment:** Highly positive corpus skew (~977 positive entries vs. 76 negative entries).
* **Extracted Themes (LDA Topics):**
  * **Topic 1:** Device reviews focusing on hardware ergonomics (`headphone`, `apple`, `like`).
  * **Topic 2:** Smart home ecosystem items (`great`, `tap`, `speaker`, `echo`, `love`).
  * **Topic 3:** Purchase contexts and user affinity (`gift`, `prime`, `tv`, `recommend`).

 

