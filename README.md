# Laura Labarthe

Data & AI engineering student at ESILV (Paris), 4th year. I spend most of my time on NLP,
applied machine learning and knowledge graphs. What I enjoy is taking a project all the way:
raw data in, something you can actually query or click on at the other end.

Currently looking for a 4 to 6 month internship in data science, ML or NLP, starting April 2026.

[LinkedIn](https://www.linkedin.com/in/laura-labarthe-a434522a0) | laura.labarthe@edu.devinci.fr

## Projects

### [Space exploration knowledge graph](https://github.com/laulbrt/web_datamining_projet)

Crawls Wikipedia articles about space agencies and missions, extracts entities with spaCy, and
builds an RDF knowledge base aligned to Wikidata that grows to roughly 80,000 triples through
SPARQL expansion. On top of it: SWRL reasoning rules, TransE and DistMult link prediction, and a
RAG pipeline that turns a plain English question into a SPARQL query.

*Python, RDFLib, spaCy, SPARQL, PyKEEN, Ollama*

### [Insurance reviews: rating prediction and sentiment](https://github.com/laulbrt/nlp-insurance-sentiment-bert)

23,500 insurance reviews and seven models compared on the same 5-star prediction task, from
TF-IDF with logistic regression up to a fine-tuned DistilBERT. Around it: LDA topic modelling, a
Word2Vec model trained on the corpus, zero-shot category detection and two Streamlit apps.

*Python, scikit-learn, Transformers, Gensim, Streamlit*

### [TripAdvisor place recommender](https://github.com/laulbrt/nlp-tripadvisor-recommendation)

Recommends a similar place from review text alone, with no metadata. Four ranking models (BM25,
TF-IDF cosine, LSA and a hybrid) evaluated on 1,835 Paris venues with a two-level ranking error
metric. BM25 stayed the hardest baseline to beat.

*Python, scikit-learn, rank_bm25, NLTK*

### [Skin tone to foundation shade](https://github.com/MayLitt/ml-fenty-skin-tone)

Predicts skin undertone from an unconstrained face photo and matches it to one of the 50 Fenty
Beauty foundation shades. MediaPipe isolates the cheek region, colour is converted to CIELAB,
and XGBoost classifies the undertone at 0.857 macro F1. Team project with Hannah-May Littière
and Yann Lin.

*Python, MediaPipe, OpenCV, XGBoost, scikit-learn*

### [Cloud VM deployment optimization](https://github.com/laulbrt/ai-algorithms-vm-optimization)

Picking the cheapest set of virtual machines to run a distributed ML training job under CPU, RAM
and throughput constraints. Solved three ways: exact MILP, genetic algorithm, simulated
annealing. The genetic algorithm matched the MILP optimum at 1.59 $/h, simulated annealing got
stuck 11% above it, and a scalability study shows where each approach breaks down.

*Python, PuLP, NumPy, Pandas*

### [Volcanic eruption analysis dashboard](https://github.com/laulbrt/volcano-events-dashboard)

Four indicators built from the NCEI global eruption record (4360 BC to 2024): grouped queries on
damage, VEI discretization, a spatio-temporal map and OPTICS density clustering on coordinates,
all served in a Dash dashboard. Team project.

*Python, Pandas, scikit-learn, Plotly, Dash*

### Other coursework

- [Airbnb price prediction](https://github.com/laulbrt/Airbnb_Price_Prediction): regression on log price from numerical, categorical and free-text listing features
- [Python data processing and analysis](https://github.com/laulbrt/Python_Data_Processing_and_Analysis_Project): CSV consolidation, cleaning and reporting pipeline with logging
- [Numerical simulation of PDEs](https://github.com/laulbrt/Partial_Differential_Equations_-PDE-_Project): two finite difference schemes, stability and convergence study, validated with a manufactured solution
- [VeloMax](https://github.com/laulbrt/VeloMax): bike shop management desktop app in C# and WPF, XML persistence

## Tools

- Languages: Python, SQL, C#
- ML and NLP: scikit-learn, PyTorch, XGBoost, Transformers, spaCy, Gensim, PyKEEN
- Data and visualisation: Pandas, NumPy, Matplotlib, Plotly, Dash, Streamlit
- Semantic web: RDF, SPARQL, Wikidata
- Other: Git, Docker

## Education

ESILV, Data & Artificial Intelligence major, 4th year (2025 to 2026)
