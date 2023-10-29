# Project Proposal: WINNOWING Algorithm for Text Plagiarism Detection

## Academic Reference

The algorithm we plan to implement is the **WINNOWING algorithm** for text plagiarism detection. The algorithm is well-documented in the paper titled *"Winnowing: Local Algorithms for Document Fingerprinting"* by Schleimer, J., Wilkerson, D. S., & Aiken, A. This paper defines the algorithm and its core principles.

[https://dl.acm.org/doi/10.1145/872757.872770](https://dl.acm.org/doi/10.1145/872757.872770)

To help us read it easier, here is the pdf version on the Stanford website
[http://theory.stanford.edu/~aiken/publications/papers/sigmod03.pdf](http://theory.stanford.edu/~aiken/publications/papers/sigmod03.pdf)

They are exact the same.

## Algorithm Summary

The WINNOWING algorithm is a local text similarity detection technique used to identify duplicate or near-duplicate passages within a set of documents. It operates by creating fixed-size "windows" of text, hashing these windows, and then selecting the minimum hash value within each window. These minimum hashes are used to create a fingerprint for the document. By comparing these fingerprints across documents, the algorithm can identify potentially plagiarized passages.

## Function I/O

The key functions we plan to implement are as follows:

1. **Text Preprocessing Function**:
    - Input: Raw text data.
    - Output: Processed text, including tokenization, stop-word removal, and stemming.
2. **Windowing Function**:
    - Input: Processed text data.
    - Output: A set of text windows of a fixed size.
3. **Hashing Function**:
    - Input: Text windows.
    - Output: Hash values for each window.
4. **Fingerprinting Function**:
    - Input: Hash values.
    - Output: Document fingerprints based on the minimum hash values.
5. **Plagiarism Detection Function**:
    - Input: Document fingerprints.
    - Output: Identification of potential plagiarism instances.

The tests that will prove the correctness of the algorithm are as follows:

- Test 1: Verify that the preprocessing function correctly tokenizes and processes text data.
- Test 2: Ensure that the windowing function creates windows of the specified size.
- Test 3: Confirm that the hashing function generates hash values for the windows.
- Test 4: Validate that the fingerprinting function correctly forms document fingerprints.
- Test 5: Check the plagiarism detection function's ability to identify potential plagiarism instances.

## Data Description

For this project, we will use a collection of text documents for testing and benchmarking the WINNOWING algorithm. The data will be sourced from publicly available text corpora and academic databases. We will process this data into .txt files, and the data will be included in our GitHub repository.

We will use C++ scripts to automate the data processing steps, including text cleaning and formatting. These scripts will be included in the repository, along with detailed documentation of the data processing pipeline.

The data directory in our GitHub repository will contain the processed text datasets, and the code/tests directory will house the test cases necessary for algorithm correctness validation.

## Repository and Contributors

We will create a private GitHub repository for this project, granting access to the course instructors and our project mentor as contributors. The repository will be structured according to the standard format provided in the example project.

If you have any specific preferences or additional details to include, please let me know, and I will make the necessary adjustments.
