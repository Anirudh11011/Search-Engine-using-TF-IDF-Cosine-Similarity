Project Title: Search Engine using TF-IDF & Cosine Similarity

Project Overview

This project involves building a mini search engine that ranks and retrieves the most relevant U.S. presidential inaugural speech based on user input. It uses TF-IDF for term weighting and Cosine Similarity for document ranking, with optimizations for efficient top-K retrieval.
Key Features and Implementations

    Document Preprocessing

        Loaded and cleaned multiple inaugural speech text files.

        Applied tokenization, stop-word removal, and stemming using NLTK.

    TF-IDF Vector Construction

        Computed term frequency (TF) and document frequency (DF) for each token.

        Normalized TF-IDF vectors for cosine similarity calculations.

    Postings List Implementation

        Created an inverted index mapping tokens to documents and their respective TF-IDF weights.

        Sorted postings by relevance for faster retrieval.

    Cosine Similarity Search

        Calculated similarity between user queries and documents using dot product of normalized TF-IDF vectors.

    Top-K Document Ranking

        Implemented a limit-based retrieval strategy to return only the top relevant documents per query.

        Improved query performance by avoiding unnecessary comparisons.

    Upper-Bound Scoring Optimization

        Used max term weights to estimate the highest possible document scores.

        Enabled early stopping in cases where a confident top result is identified.

    Adaptive Retrieval Depth

        Dynamically expanded the document scan range if the top match was uncertain.

        Balanced efficiency with high recall and precision.

    Interactive Query System

        Designed a query interface that allows input of free-form text to identify the most relevant speech file.

        Returns document name and similarity score.

Conclusion

This project demonstrates the implementation of core information retrieval techniques from scratch. It balances algorithmic efficiency with retrieval accuracy and shows how traditional IR techniques like TF-IDF and cosine similarity power modern search systems.
