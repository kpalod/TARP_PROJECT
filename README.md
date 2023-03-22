# *HireHive: A Smart Resume Analyser*

## Introduction
A "Smart Resume Analyser" is a tool that automates the process of evaluating and analyzing job applicants' resumes. It is designed to help aspirants to gain skills and save time and effort in the job hunting process by quickly extracting relevant information from resumes and presenting it in an organized and meaningful way.

## *Methodology*
- Data Collection and Data Preprocessing: The application takes a resume as input, either in the form of a PDF or a text document. The application then eliminates any unnecessary information from the resume, including headers, footers, and graphics, and transforms it to plain text. The text is then tokenized into words and sentences, and various fundamental text cleaning operations are carried out, like stop word removal and word stemming. For this we will use PyResparser which is a Python library used for parsing resumes and extracting structured information such as candidate name, email, phone number, education, and work experience. Below is how this library works:
  -Parsing the Resumes: PyResparser takes in a resume which can be in various different formats like pdf, html, txt etc. and converts it into plain text using external libraries such as PyPDF2, docx2txt, and Beautiful Soup.
  - Pre-Processing the text: The resume's plain text is pre-processed using a variety of methods, including sentence and word tokenization, stop-word removal, and stemming, to weed out extraneous material and identify crucial keywords.

- Information Extraction: Important data including the candidate's name, email address, phone number, educational background, employment history, and skill set are extracted by the programme using NLP techniques like Named Entity Recognition (NER). 
PyResparser employs NLP methods like Named Entity Recognition (NER) to extract structured data from the candidate's resume, including their name, email, phone number, educational background, employment history, and abilities. Spacy library is used by PyResparser for NER.
PyResparser delivers the findings in JSON format, which can be utilised for additional analysis or storage, after the structured data has been extracted.


## *Functionality*
- Resume parsing: The tool can quickly scan and extract key information from resumes, such as education, work experience, skills, and certifications.
- Data analysis: The tool can use algorithms and machine learning models to analyze the extracted data and provide insights into the job applicants' qualifications, -  strengths, and weaknesses.
- Matching: The tool can compare the extracted information with the requirements of the job to identify the best-fit candidates and present them to the employer in a ranked order.
- Reporting: The tool can generate reports that summarize the key findings and provide recommendations on which candidates are the most suitable for the job.

Overall, a smart resume analyser can make it easier and more efficient for the students to evaluate their job prospects.

## *Tools used*
- Python
- NLP 
  - Spacy Framework
- Visual Studio Code
- GitHub Desktop
- Dblp
- Obsidian

## *Workflow division*
We will divide the tasks among the team members based on their strong points. However every team member would help other members in their tasks if possible and team members would explain their work to others so that everyone learns the problem better and can help come up with a solution whenever required. 

- *Front-end development:* One team member (Shlok Aggarwal) would be responsible for developing the user interface and ensuring that the tool is easy to use and navigate
- *Data parsing and analysis :* Another team member(Kushagra Palod) would focus on developing the algorithms and models that extract information from resumes and analyze it to provide insights into the job applicants' qualifications.
- *Natural language Processing implementation:* The third team member(Archit Jain) would be responsible for implementing the Natural Language Processing to find the relationship between different entities in a text.

Other tasks such as documentation,paper collection, related work analysis and project design would be contributed by all equally. 

Regular communication and collaboration among the team members will be ensured through GitHub Desktop so that the project progresses smoothly and efficiently.


| **Domain**                                 | **Team Member**| 
|--------------------------------------------|----------------|
| Web Application Development                | Shlok Aggarwal | 
| Data Parsing and Analysis                  | Kushagra Palod |
| Natural Language Processing Implementation | Archit Jain    |




