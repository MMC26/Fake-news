# DETECCIÓ DE NOTÍCIES FALSES
Un projecte de machine learning dissenyat per analitzar notícies i predir si són **falses** o **verídiques**. Aquest repositori inclou:

- Un script per al *web scraping* que amplia el dataset inicial.
- El dataset definitiu utilitzat a la pràctica.
- Un fitxer `main.py` amb el codi implementat.
- Informe del projecte.

## CARACTERÍSTIQUES
- **Tipus de classificació:** binària (*Real* [0] o *Falsa* [1]).
- **Tècniques utilitzades:**
  - Bag of Words (BoW) i TF-IDF per a la vectorització del text.
  - Algorismes de classificació Naive Bayes (NB): MultinomialNB, GaussianNB, BernoulliNB, ComplementNB.
- **Entrenament i avaluació:**
  - Dades entrenades amb un dataset ampliat.
  - Resultats interpretables amb gràfics i mètriques.
- **Cas d'ús:**
  - Predir l'autenticitat d'una notícia de cada tipus.

## INSTAL·LACIÓ 

1. **Clona el repositori:**
   ```bash
   git clone https://github.com/MMC26/Fake-news.git
   cd Fake-news

2. **Llibreries:**
    Aquest projecte utilitza diverses llibreries de Python que cal instal·lar abans d’executar-lo. Pots fer-ho creant un entorn virtual i instal·lant-les amb pip:

    ```bash
    pip install pandas
    pip install dateutil
    pip install numpy
    pip install matplotlib
    pip install nltk
    pip install rate-nltk
    pip install seaborn
    pip install langdetect
    pip install deep_translator
    pip install wordcloud
    pip install scikit-learn
    pip install scipy
    pip install newspaper3k
    pip install lxml[html_clean]
    ```

## MÈTRIQUES I RESULTATS
Hem utilitzat la mètrica F1-score per controlar tant els falsos positius com negatius. Per visualitzar els resultats, hem utilitzat la corba ROC. El model seleccionat (**ComplementNB amb text_without_stopwords**) presenta:
- **Accuracy (test):** 0.75  
- **F1-score (test):** 0.78

## AUTORES
- Maria Muñoz Cabestany - MMC26
- Blanca Pinyol Chacon - NIU1666134

