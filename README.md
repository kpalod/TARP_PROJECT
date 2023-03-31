# *HireHive: A Smart Resume Analyser*

## Introduction
A "Smart Resume Analyser" is a tool that automates the process of evaluating and analyzing job applicants' resumes. It is designed to help aspirants to gain skills and save time and effort in the job hunting process by quickly extracting relevant information from resumes and presenting it in an organized and meaningful way.

## *Methodology*
- Data Collection and Data Preprocessing: The application takes a resume as input, either in the form of a PDF or a text document. The application then eliminates any unnecessary information from the resume, including headers, footers, and graphics, and transforms it to plain text. The text is then tokenized into words and sentences, and various fundamental text cleaning operations are carried out, like stop word removal and word stemming. For this we will use PyResparser which is a Python library used for parsing resumes and extracting structured information such as candidate name, email, phone number, education, and work experience. Below is how this library works:
  - Parsing the Resumes: PyResparser takes in a resume which can be in various different formats like pdf, html, txt etc. and converts it into plain text using external libraries such as PyPDF2, docx2txt, and Beautiful Soup.
  - Pre-Processing the text: The resume's plain text is pre-processed using a variety of methods, including sentence and word tokenization, stop-word removal, and stemming, to weed out extraneous material and identify crucial keywords.

- Information Extraction: Important data including the candidate's name, email address, phone number, educational background, employment history, and skill set are extracted by the programme using NLP techniques like Named Entity Recognition (NER). 
PyResparser employs NLP methods like Named Entity Recognition (NER) to extract structured data from the candidate's resume, including their name, email, phone number, educational background, employment history, and abilities. Spacy library is used by PyResparser for NER.
PyResparser delivers the findings in JSON format, which can be utilised for additional analysis or storage, after the structured data has been extracted.

- Data Analysis and Visualization: The application analyses the retrieved data using statistical approaches to produce insights like a list of the most commonly stated abilities, a summary of work history, and educational background. The application displays the analysis findings as interactive graphs and charts. 
Finally, it can be said that PyResparser is a helpful tool for recruiters, HR specialists, and job portals to automate resume screening and candidate shortlisting since it parses resumes and extracts structured information using a combination of external libraries and NLP techniques.


## *Functionality*
- Resume parsing: The tool can quickly scan and extract key information from resumes, such as education, work experience, skills, and certifications.
- Data analysis: The tool can use algorithms and machine learning models to analyze the extracted data and provide insights into the job applicants' qualifications, -  strengths, and weaknesses.
- Matching: The tool can compare the extracted information with the requirements of the job to identify the best-fit candidates and present them to the employer in a ranked order.
- Reporting: The tool can generate reports that summarize the key findings and provide recommendations on which candidates are the most suitable for the job.

Overall, a smart resume analyser can make it easier and more efficient for the students to evaluate their job prospects.

## *Description About Dataset*
- The Kaggle dataset [Resume Dataset](https://www.kaggle.com/datasets/snehaanbhawal/resume-dataset?resource=download) contains a collection of resumes in PDF format. 
- Here are some details about the dataset:
  - The dataset contains 1,420 resumes in PDF format.
  - The resumes belong to candidates from various fields, such as software engineering, marketing, finance, healthcare, and more
  - The resumes are labeled with the candidate's name and the category of the resume (such as "Software Engineer", "Sales Manager", "Data Analyst", etc.).
- We are using this dataset for various NLP tasks related to resume parsing and analysis, such as Named Entity Recognition (NER), Text Classification, Information Extraction, and more. 

## *Tools used*
- Python Flask - a micro web framework written in Python used for developing the backend of the application.
- NLP 
  - Spacy Framework : a popular Python library used for natural language processing tasks such as tokenization, stemming, and named entity recognition.
- Visual Studio Code : for writing and debugging code. VS Code provides a lot of extensions and other tools for streamlined developement of an application.
- Chart.js - a JavaScript library used to create interactive charts and graphs to visualize the analysis results.
- GitHub Desktop : Github desktop client provides a GUI based interface for commiting changes to the remote repository and makes solving issues and pull requests easy.
- Dblp : For finding relevant latest papers as per the scope of the course defined.
- Obsidian : A markdown editor used for editing .md files and creating documentation of the project. 

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

## *Literature Survey*
|**S. No.**|**Name**|**Methodology**                            | **Advantages**      |**Drawbacks**            | 
|----------|--------|-------------------------------------------|---------------------|-------------------------|
|1         |RESUME PARSER USING NLP| Machine learning-based approach to automatically extract and parse information from resumes. It uses Natural Language Processing (NLP) techniques and the development of a web application to implement the resume parser.| By automating the screening process, a resume parser can help reduce the risk of bias or subjective decision-making, resulting in a more objective and fair hiring process. Depending on the specific needs of the organization or individual using the resume parser, it can be customized to parse resumes for specific fields, job titles, or industries.|Resume parsing algorithms have difficulty accurately parsing resumes that have unusual formatting, unconventional layouts, or use non-standard fonts. It is also possible for the parser to misinterpret certain information or miss important details altogether, leading to errors or omissions in the parsed data. Depending on the complexity of the resume parser and the amount of data it needs to process, it may require a significant amount of computational resources or time to operate effectively.|
|2       | A Systematic Literature Review (SLR) On The Beginning of Resume Parsing in HR Recruitment Process & SMART Advancements in Chronological Order | The authors conducted a comprehensive search for relevant articles on various electronic databases such as Web of Science, Scopus, IEEE Xplore, and ACM Digital Library. They also searched for articles in Google Scholar. The inclusion criteria for selecting the articles were based on specific keywords such as "resume parsing," "HR recruitment," "machine learning," "deep learning," and "natural language processing." | The paper provides an in-depth analysis of the existing literature related to resume parsing in HR recruitment process, including various techniques and algorithms used, their strengths and weaknesses, and the challenges and ethical considerations associated with them. | 1) The study has limited its scope to specific databases, journals, or conferences, which limits the number of papers included in the review. 2)The findings of the review may not be generalizable to all industries or contexts, as the focus was on the HR recruitment process |
|3 | Career Path Prediction System Using Supervised Learning Based on Users’ Profile | 1) The authors extracted features from the preprocessed data using various techniques such as Principal Component Analysis (PCA), Feature Selection, and Natural Language Processing (NLP). 2) The authors used various supervised learning algorithms such as Decision Tree, Random Forest, K-Nearest Neighbors (KNN), and Support Vector Machine (SVM) to build the career path prediction system.| 1) The paper proposes a new system that predicts the career path of users, which can be useful for individuals to make informed decisions about their career. 2) The paper evaluates the proposed system using various performance metrics such as accuracy, precision, recall, and F1-score. This provides a comprehensive assessment of the system's performance. | 1) The study has not compared the results with other similar studies, which limits the ability to draw conclusions about the effectiveness of the proposed method. 2) The study is biased towards certain factors or variables, which impacts the accuracy of the results. | 
|4| Career recommendation systems using content-based filtering | 1) The collected data was preprocessed to remove duplicates, irrelevant information, and to standardize the format. 2) The authors used Natural Language Processing techniques to extract important features such as skills, education, experience, and job titles from the preprocessed data. | 1) The use of content-based filtering allows for personalized career recommendations to be generated based on an individual's unique preferences and interests. 2) The system does not require external data sources such as job vacancies, which means it can be used even in scenarios where such data is not available. | 1) The paper lacks evaluation of the performance of the proposed system. It would have been helpful to compare the recommended careers with actual career choices made by users and measure the accuracy of the recommendations. 2) The system has been trained on a limited amount of data, which could affect the accuracy of the recommendations. The paper does not provide information on the size or diversity of the dataset used. | 
|5 | Design and Development of Machine Learning based Resume Ranking System | The paper proposes a Resume Screening System based on natural language processing (NLP) methods and K-Nearest Neighbors (KNN) algorithm.The KNN algorithm is used to pick and rank the resumes based on job descriptions in huge quantities. The system evaluates the applicant's skills based on a test, ensuring that the resumes uploaded by the applicant are genuine and the applicant is truly knowledgeable about the skills. | The proposed system uses NLP methods and KNN algorithm to automate the resume screening process, which saves time and effort for the recruitment team.
The system evaluates the applicant's skills based on a test, ensuring that the resumes uploaded by the applicant are genuine and the applicant is truly knowledgeable about the skills. | The system relies heavily on the accuracy of NLP methods, which may not always be reliable, especially when dealing with complex sentences or language barriers. The paper does not discuss the potential biases that may be present in the system, which may lead to discrimination against certain groups of applicants | 






 


  

## *References*
[1] Tejaswini, K., Umadevi, V., Kadiwal, S. M., & Revanna, S. (2022). Design and development of machine learning based resume ranking system. Global Transitions Proceedings, 3(2), 371-375.

[2] Garg, S., Sinha, S., Kar, A. K., & Mani, M. (2022). A review of machine learning applications in human resource management. International Journal of Productivity and Performance Management, 71(5), 1590-1610.

[3] Kandji, A. K., & Ndiaye, S. (2022, February). Design and realization of an NLP application for the massive processing of large volumes of resumes. In 2022 IEEE Multi-conference on Natural and Engineering Sciences for Sahel's Sustainable Development (MNE3SD) (pp. 1-5). IEEE.

[4] Nimbekar, R., Patil, Y., Prabhu, R., & Mulla, S. (2019, December). Automated resume evaluation system using NLP. In 2019 International Conference on Advances in Computing, Communication and Control (ICAC3) (pp. 1-4). IEEE.

[5] Yadalam, T. V., Gowda, V. M., Kumar, V. S., Girish, D., & Namratha, M. (2020, June). Career recommendation systems using content based filtering. In 2020 5th International Conference on Communication and Electronics Systems (ICCES) (pp. 660-665). IEEE.

[6] Kolhe, H., Chaturvedi, R., Chandore, S., Sakarkar, G., & Sharma, G. (2023). Career Path Prediction System Using Supervised Learning Based on Users’ Profile. In Computational Intelligence: Select Proceedings of InCITe 2022 (pp. 583-595). Singapore: Springer Nature Singapore.


