# Analysis-of-DermAI-Diagnostics-Skin-Cancer-Dataset

Leveraging SQL-based descriptive and diagnostic analytics in understanding the demographic, environmental.factors and lesion characteristics
---
![image](https://github.com/user-attachments/assets/3dc9f4cd-591e-4412-8662-3e76fc3c326e)

*Disclaimer⚠️: All datasets and reports do not contain real proprietary, confidential, or sensitive information from any company, institution, or individual. All info are dummy and design to demonstrate my capabilities of using SQL to perform descriptive and diagnostic analytics.*

INTRODUCTION 
---
Skin cancer is one of the most common and life-threatening diseases, yet early detection can significantly improve survival rates. Our business, DermAI Diagnostics, leverages machine learning and clinical dermatology research to enhance early diagnosis and treatment. By analyzing patient demographics, environmental factors, and lesion characteristics, we create data-driven insights to assist dermatologists in early-stage detection and decision-making. Through a combination of AI-powered diagnostic tools,
real-world clinical data, and SQL-based research, our company aims to bridge the gap between medical practitioners and machine learning-based skin lesion classification. By providing a structured dataset and digital tools, we support medical research, epidemiological studies, and AI-driven skin cancer detection, ultimately improving public health outcomes.

![image](https://www.alluraskin.com/wp-content/uploads/2024/02/skinCancerExam.jpeg)

PROBLEM STATEMENT 
---
Skin cancer detection is often delayed due to misdiagnosis, lack of access to dermatologists, and limited understanding of environmental risk factors. With 1,089 instances of skin lesions in our dataset, we aim to uncover key patterns that link demographics, environmental exposure, and lesion characteristics to different types of skin cancer. This project seeks to enhance early-stage diagnosis and machine learning-based decision support by structuring the data for SQL queries, analysis, and model training.

AIM OF PROJECT 
--- 
* Identify environmental and demographic risk factors that correlate with specific skin lesions.
* Analyze lesion characteristics to find patterns that indicate cancerous vs. benign lesions.
* Enhance dermatological research by providing a well-organized dataset for epidemiological studies and AI model training.

METHODOLOGY 
---
* Business Understanding: Understand the company's objectives and expectations to align analysis with business goals.
* Data Extraction: Retrieve Patient Info and Lesion Info data from the company's database for in-depth analysis.
* Develop Analysis Approach: Define a clear plan for the analysis, identifying key metrics and setting objectives aligned with the business goals.
* Perform Descriptive Analysis: Use SQL queries to summarize data, identify trends, and generate an overview of patient demographics, environmental factors, and lesion characteristics.
* Perform Diagnostic Analysis: Dive deeper into the data to identify the factors driving environmental factors and variations in skin cancer, correlating demographic and lesion characteristics relating to different types of skin cancer. 
* Generate Insights and Recommendations: Based on findings from the analyses, provide actionable insights and recommendations to address environmental exposure, enhance early stage diagnosis, and optimize dataset for AI & ML training.

SQL FUNCTIONS/CLAUSES
--- 
* SQL QUERIES: Extract relevant data from the Patient and Lesion Schemas.
* CASE: Executes conditional logic by evaluating conditions and returning a value.
* JOIN: Combine rows from two or more tables based on a related column between them.
* COUNT: Returns the number of rows that matches a specified criterion.
* GROUP BY: Often used with aggregate functions to group the result-set by one or more columns.

MODELLING 
---
To understand the structure of the database, I visualise the Entity-Relationship Diagram (ERD) that maps out the tables and their connections. This diagram clarifies how the tables, patient and lesion, are organized and interact with each other. Using the ERD as a guide, I can see how data flows between these tables, making it easier to analyze patient info and identify factors leading to cancer. This clear structure is essential for accurate and effective analysis throughout the project.

<img width="671" alt="image" src="https://github.com/user-attachments/assets/92ce3b41-c501-4784-b3c1-7bdd5461aee9" />

DATA ANALYSIS
---
This query provides a comprehensive view of the patient info and lesion info schemas, enabling a clear visualization of key metrics and attributes essential for analyzing demographic, environmental factors, and lesion characteristics.

<img width="932" alt="image" src="https://github.com/user-attachments/assets/4b5060cd-6329-4690-8ec3-9f79c06ea653" />

### DESCRIPTIVE ANALYTICS (PATIENT DEMOGRAPHICS)
This query provides insights into the company's data by displaying the total number of skin lesion cases (1,088) and identifying the maximum age, which stands at 94 years. It also groups total lesion  by age bracket, highlighting that people aged over 50 have the highest number of lesions (795), followed by 30 & 50 (236). In contrast, Under 30 have the fewest lesions with 57 cases. This analysis offers a clear view of lesion distribution, valuable for understanding lesion severity among older patients.

<img width="919" alt="image" src="https://github.com/user-attachments/assets/dc305c8a-5a02-4516-8dc8-fa2f31c01cf7" />

The first query illustrates the gender distribution of patients, indicating that males comprise the majority with a count of 726, while females account for 362. Additionally, the second query categorizes gender according to skin cancer history and total cases. With 109 males out of 726 and 115 females out of 362 having cancer history. This analysis provides valuable insights into the gender & cancer history of the patients from the dataset.

<img width="917" alt="image" src="https://github.com/user-attachments/assets/1aed6b0f-90e6-46fc-84a0-b19af0a9d569" />

### DIAGNOSTIC ANALYTICS (PATIENTS WITH LESION)
This diagnostic analysis focuses on patients with lesion and previous cancer history. The first query identifies the relationship between smokers and non smokers to know if the lesions grew or changed. Although there are fewer smokers, they make up majority of the data with 61.29% highlighting that smoking either grows or changes the lesion. 

<img width="920" alt="image" src="https://github.com/user-attachments/assets/61f86e49-38f0-4736-b508-d1ad60f240fb" />

The second query examines what type of lesion has the highest % of patients and exposure to pesticides. The 'BCC' infection has the highest patients with 127 of them being exposed out of 273 patients statistically showing they make up 46.52% of the data. These insights are crucial for identifying areas for improvement for patients with this type of lesion.

<img width="920" alt="image" src="https://github.com/user-attachments/assets/b41326c9-02b1-49be-a240-4b06c4e581fd" />

### DIAGNOSTIC ANALYTICS (CANCER HISTORY)
The first query examines whether pesticide exposure is a casue of previous cancer history. People exposed are fewer but statistics shows that pesticide exposure is a likely cause of previous history with a percentage of 47.77. The second query analyses the data to tell us that 199 out of 224 patients with previous cancer history got biopsied which is 88.84% of the cases recorded while 259 out of 864 patients didn't get biopsied which is 29.98% of the cases recorded. These insights are crucial for identifying patients history and possible misdiagnosis from not getting biopsied.

<img width="920" alt="image" src="https://github.com/user-attachments/assets/bb051061-fd34-4fae-b2b8-8281ac2de1b8" />
<img width="920" alt="image" src="https://github.com/user-attachments/assets/74d4a156-e15e-4aaa-9609-198b12feb2c0" />

RECOMMENDATIONS
--- 
Based on the insights drawn from the patient info and lesion info datasets, here are some data-driven recommendations to help determine the accuracy of lesion info provided by patients to enhance dermatological research by providing a well-organized dataset for epidemiological studies and AI model training:
* More biopsy needs to be performed as a standard in this medical research to make our data more relevant and accurate for machine learning studies or correct analysis.
* Other factors like age, family history, exposure to harmful chemicals like pesticides, and lack of clean water or sanitation also increase the chances of needing a biopsy. 
* The problem statement says there are a total of 1,089 cases but after running diagnostic analysis, it shows there are 1,088 cases. I recommend use of up to date records and proper database management systems. 

By applying these recommendations, DermAI will be able to manage patient data properly and have accurate records for AI model training. 

### THANK YOU
For more information, you can contact me
![Orange Modern Technology LinkedIn Banner](https://github.com/user-attachments/assets/4d91e1e5-c613-48a0-8a9a-15dbaf997908)





