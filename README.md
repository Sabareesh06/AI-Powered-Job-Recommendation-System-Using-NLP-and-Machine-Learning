AI-Powered-Job-Recommendation-System-Using-NLP-and-Machine-Learning
Job Recommendation System :

Overview :
This project is an " NLP and ML-based Job Recommendation System " that matches job seekers with relevant job postings based on their resumes. Using Natural Language Processing (NLP), the project extracts key skills and features from resumes (Word documents) and matches them with job descriptions (CSV file) based on similarity scores.

Features :
- Extracts key skills from resumes (in `.docx` format) and job descriptions (CSV file).
- Computes similarity scores between resumes and job descriptions using **TF-IDF Vectorization** and **Cosine Similarity**.
- Ranks job postings for each resume based on skill relevance.

Dataset :
- Resumes: Provided in `.docx` format.
- Job Descriptions: Stored in a `CSV` file containing details like:
  - Job Title
  - Key Skills
  - Job Experience Required
  - Job Salary, etc.

How It Works :
1. Preprocessing Resumes:
   - Extract text from Word documents using `python-docx`.
   - Tokenize and clean the data to extract meaningful skills.

2. Preprocessing Job Descriptions:
   - Load job data from a CSV file.
   - Extract and clean the "Key Skills" column for analysis.

3. Similarity Measurement:
   - Apply " TF-IDF Vectorization " to transform text into numerical representations.
   - Compute " Cosine Similarity " to match resumes with job descriptions.

4. Output:
   - For each resume, a ranked list of the most relevant job postings is generated based on skill similarity.

Requirements :
- Python 3.8 or higher
- Required libraries: See the [requirements.txt](requirements.txt) file.
- pip install -r requirements.txt


EXAMPLE OUTPUT :
Resume: John_Doe.docx
Top 3 Matched Jobs:
1. Job Title: Media Planning Executive
   Skills Match: 85%
2. Job Title: Sales Executive/Officer
   Skills Match: 76%
3. Job Title: Technical Support Engineer
   Skills Match: 69%

