# Laura Labarthe

Data & AI engineering student at ESILV (Paris), 5th year, currently on exchange at California
State University, Long Beach with a finance minor. I spend most of my time on NLP, applied
machine learning and knowledge graphs. What I enjoy is taking a project all the way: raw data in,
something you can actually query or click on at the other end.

Looking for a 6 month end-of-studies internship in data science, ML or NLP, starting January
2027. Dates are flexible.

[LinkedIn](https://www.linkedin.com/in/laura-labarthe-a434522a0) | laura.labarthe@edu.devinci.fr

## Projects

### [Space exploration knowledge graph](https://github.com/laulbrt/space-exploration-knowledge-graph)

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

### [Skin tone to foundation shade](https://github.com/MayLitt/ml-fenty-skin-tone)

Predicts skin undertone from an unconstrained face photo and matches it to one of the 50 Fenty
Beauty foundation shades. MediaPipe isolates the cheek region, colour is converted to CIELAB,
and XGBoost classifies the undertone at 0.857 macro F1, ahead of every tuned baseline and
ensemble tested. Team project with Hannah-May Littière and Yann Lin.

*Python, MediaPipe, OpenCV, XGBoost, scikit-learn*

### [TripAdvisor place recommender](https://github.com/laulbrt/nlp-tripadvisor-recommendation)

Recommends a similar place from review text alone, with no metadata. Four ranking models (BM25,
TF-IDF cosine, LSA and a hybrid) evaluated on 1,835 Paris venues with a two-level ranking error
metric. BM25 stayed the hardest baseline to beat.

*Python, scikit-learn, rank_bm25, NLTK*

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

## Earlier work

### [CVE vulnerability watch](https://github.com/laulbrt/cve-vulnerability-watch)

Reads the CERT-FR advisory feed, extracts every CVE, enriches each one with its CVSS severity
from MITRE and its EPSS exploitation probability from FIRST, then analyses the two together and
sends an email alert on anything critical. Severity and likelihood do not always agree, and the
gap between them is the interesting part.

*Python, pandas, feedparser, requests, seaborn, Plotly*

### [Airbnb price prediction](https://github.com/laulbrt/Airbnb_Price_Prediction)

Predicting the log price of 51,877 listings from features that mix numbers, categories, dates and
free text. XGBoost inside a scikit-learn pipeline so preprocessing and model are fitted together,
reaching an R² of 0.655 and an RMSE of 0.420 against 0.716 for the mean baseline. A second
notebook covers the feature engineering that did not make the cut, including TF-IDF on the
descriptions and geodesic distance to the city centre.

*Python, scikit-learn, XGBoost, pandas, geopy*

### [Gomoku with a minimax AI](https://github.com/laulbrt/gomoku-ai)

Five in a row on a 15 by 15 board against a minimax AI with alpha-beta pruning, a time-bounded
search, and a heuristic that scores alignments by length and by whether they are blocked at
either end. Candidate moves are restricted to cells next to an existing stone, which is what
makes depth 3 tractable on 225 cells.

*Python, NumPy*

### [Allen-Cahn equation, finite differences](https://github.com/laulbrt/Partial_Differential_Equations_-PDE-_Project)

Numerical resolution of a nonlinear parabolic PDE with two schemes: fully explicit, and
semi-implicit with the diffusion term taken at step n+1 to keep the linear system solvable
without Newton. The comparison is really about the stability constraint the explicit scheme
imposes on the time step.

*Python, NumPy, SciPy sparse*

### [Ligue 1 match outcome prediction](https://github.com/laulbrt/ligue1-match-prediction)

Predicting home win, draw or away win for the 2023-2024 season from ten years of match history,
using club winrates and squad market value. The random forest lands at 0.442 accuracy against
0.460 for always predicting a home win, so it does not beat the baseline. The README explains
why season-level aggregates cannot separate two fixtures involving the same clubs, and which
per-match features in the dataset would have.

*Python, pandas, scikit-learn*

### [Pokemon battle game](https://github.com/laulbrt/pokemon-battle-cpp)

Turn-based game in C++ with an SFML interface, five classes built on composition, a full
weakness and resistance table across 17 types, and 151 Pokemon loaded from CSV rather than
hardcoded.

*C++, SFML*

### [VeloMax](https://github.com/laulbrt/VeloMax)

Bike shop management application: MySQL schema of 11 tables designed from the domain, three
non-trivial queries (correlated subquery, self-join, union), and a C# WPF interface following
MVC.

*C#, WPF, MySQL*

## Tools

- Languages: Python, SQL, C#, C++
- ML and NLP: scikit-learn, PyTorch, XGBoost, Transformers, spaCy, Gensim, PyKEEN
- Data and visualisation: Pandas, NumPy, Matplotlib, seaborn, Plotly, Dash, Streamlit
- Semantic web: RDF, SPARQL, Wikidata
- Other: Git, Docker, MySQL

## Education

- ESILV, Paris. Engineering degree, Data & Artificial Intelligence major. 5th year, graduating
  2027.
- California State University, Long Beach. Exchange semester, finance minor.
