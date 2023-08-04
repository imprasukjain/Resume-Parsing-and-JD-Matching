# Resume Parsing and JD Matching

## Introduction
This repository contains the code and resources for Resume Parsing and Job Description (JD) Matching using two separate Jupyter Notebooks. The goal is to match job seekers' resumes with relevant job descriptions, aiding in the recruitment process.

## Techniques Used
### Resume Parsing
For Resume Parsing, we utilize the popular Natural Language Processing (NLP) library, SpaCy. We train an NLP model on preprocessed resume data using the `train_data.pickle` file. This model is capable of extracting key information such as candidate name, contact details, skills, work experience, and education from resumes.

### JD Matching
For JD Matching, we employ two different techniques:

1. **Doc2Vec-based Matching**: We use the pre-trained `Doc2Vec.model` to infer document vectors for both job descriptions and resumes. These vectors are then compared using cosine similarity to find the most relevant matches.

2. **SpaCy-based Matching**: We use the SpaCy NLP library to process both JDs and resumes. By analyzing the entities and noun chunks, we identify relevant matches based on overlapping keywords and skills.

## Data
We use `data.csv` as the training data for JD Matching. The CSV file contains job descriptions along with their corresponding categories.

## Pre-trained Models
This repository provides the pre-trained models `Doc2Vec.model` for JD Matching and `NLP.model` for Resume Parsing. You can directly use these models to match new JDs with resumes or extract information from new resumes.

## How to Use
1. Clone the repository to your local machine.
2. Run the JD Matching notebook (`JD Matching.ipynb`) or the SpaCy-based version (`JD Matching.ipynb`) to match job descriptions with resumes.
3. Use the Resume Parsing notebook (`Resume Parsing.ipynb`) to parse and extract information from resumes.
4. Load the pre-trained models (`Doc2Vec.model` and `NLP model`) for faster inference or train your own models if required.

## Conclusion
With the provided code and pre-trained models, you can efficiently match job descriptions with relevant resumes and extract valuable information from the resumes, streamlining the recruitment process. Feel free to contribute, improve, or customize the techniques according to your specific use case.

Happy matching and parsing! 🚀
