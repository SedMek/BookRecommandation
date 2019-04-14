# BookRecommendation
Data mining project: Book recommendation

This project uses the "Book-Crossing Dataset" from http://www2.informatik.uni-freiburg.de/~cziegler/BX/

### Installation guide:
* download Chrome driver and update its location in *Data Enrichment and Book Description Similarity* notebook.
* Use this command to install the required librairies:
```
pip install -r requirements.txt
```

### Code Structure:
* *Data Enrichment and Book Description Similarity*: This notebook uses Selenium (Chrome driver should be installed to be able to use it) to simulate a human interaction with a web navigator using a Python code. It looks for books information in Amazon pages and books description in BookFinder.com to enrich the database. Then it measure the cosine distance between book description to be able to recommend books that have similar descriptions. It uses only a small part of the dataset for demonstration purposes only..

* *Book Recommendation*: This notebook checks the data in the datasets and visualizes it. It then cleans it and works on User-User book recommendation: It looks for similarities between users, then recommends books read by a user to other users that are most similar to it.

