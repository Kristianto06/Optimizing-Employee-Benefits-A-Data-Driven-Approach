# Optimizing Employee Benefits: A Data-Driven Approach 📊
The primary objective of this project is to conduct a thorough analysis of the current employee benefits program to identify areas for improvement and optimization. By leveraging data-driven insights, we aim to develop a benefits package that is both cost-effective and highly valued by our employees.

## Project Overview 🚀
"Imagine this: a factory worker can return to work sooner after receiving emergency dental care due to an accident, thanks to the coverage provided by their company's health benefits plan. A mother of a child born deaf doesn't have to sell her assets to pay for a hearing aid because her company's health plan covers congenital conditions. Financial crises due to the costs of hemodialysis or ICU care can be avoided, thanks to the comprehensive insurance coverage provided by the company.

Employee benefits, particularly health benefits, are more than just perks; they are the foundation of a productive workforce. When our marketing team receives a request from a company to design a health benefits program for their employees and families, we see more than just numbers on a spreadsheet. We see the people behind those numbers: a father worried about the cost of his child's physical therapy exceeding his monthly salary, a mother stressed about choosing between paying for a hearing aid or school fees, or a young worker traumatized by a workplace accident.

An employee health program is not just about mitigating the risk of injury or illness. It's about creating a humane work environment where every employee feels protected – from a simple doctor's consultation for a cough to financial support for chemotherapy or ICU care. The goal of such a program is not only to reduce absenteeism but also to foster loyalty and productivity.

We call this 'empathetic productivity'. Prioritizing employee health delivers a powerful return: a healthier workforce, a more resilient business, and a foundation of trust that fuels success.

## Analysis & Insights 🔍

To evaluate claim trends, we focused on the following key metrics:

![image](https://github.com/user-attachments/assets/838ab09e-ce24-42ca-a937-a2efae20f758)
![image](https://github.com/user-attachments/assets/ff10048d-1e47-4b64-8bec-d83db4b32e7c)



![image](https://github.com/user-attachments/assets/6add390d-d78c-4323-a4bc-e883c0d41a99)



- Total Billed Amount: The total dollar amount billed for medical services.
- Outpatient vs. Hospitalization Claims: The proportion of total billed amount attributed to outpatient services versus inpatient (hospitalization) services.
- Percentage Change: The month-over-month percentage change in the total billed amount.

> [!IMPORTANT]
> Total Billed Amount
- The total billed amount fluctuated over the six-month period, with the highest amounts in March and the lowest in June.
- The total billed amount was IDR 10,107,945,411 in January and decreased to IDR 3,528,347,887 in June.

> [!IMPORTANT]
> Outpatient vs. Hospitalization Claims
- Outpatient claims consistently represented the larger portion of the total billed amount each month.

In June, the billed amount for ***Outpatient claims*** was $\color{orange} IDR 2,001,475,542$  while hospitalization claims were IDR 1,526,872,345.
Percentage Change

The percentage change in total billed amount fluctuated from month to month, showing both increases and decreases.
There was a significant negative percentage change in June -59.3% indicating a substantial decrease in the total billed amount compared to May.
Additional Observations

The chart suggests a potential trend of decreasing total billed amounts from March to June.
The significant drop in June warrants further investigation to understand the underlying causes.
Potential Questions for Further Analysis

What factors contributed to the fluctuation in total billed amounts over the six-month period?
Why was there a significant decrease in the total billed amount in June?
Are there any seasonal patterns or external factors that could explain the observed trends?
What are the specific trends for outpatient and hospitalization claims individually?


## Recommendations

This method is used to deliver insights and inform preventive, curative, and benefit design actions preferred by claim experience characteristics.  It also facilitates communication and education for the company.


## Dataset 📈

 * The raw claim data contains claims that occurred over a specific period, which in this case is 6 months of data.
 * The ICD-Code contains disease codes that describe the condition of the insured who filed the claim.

The ICD-Code is taken from the following link.

https://ftp.cdc.gov/pub/Health_Statistics/NCHS/Publications/ICD10CM/

Dataset Description raw claim data

This dataset contains 59,999 records, each representing a unique medical claim. It provides valuable insights into various aspects of healthcare claims processing.

Patient Information:
  
| Variable | Description  |
| :------------ |:---------------|
| Member ID    | Unique identifier for each patient. |
| Location     | Geographic location associated with the patient. |


Key Variables

Claim Details:

| Variable | Description  |
| :------------ |:---------------|
| Claim_No    | Unique identifier for each claim. |
| type     | Type of claim (e.g., inpatient, outpatient, dental). |
| ServiceStartDate    | Date when the medical service began. |
| ServiceStartEnd     | Date when the medical service ended. |
| Days     | Duration of the service. |
| ProviderName    | Name of the healthcare provider. |

Service Information:

| Variable | Description  |
| :------------ |:---------------|
| BenefitDescription    | General description of the service provided. |
| DetailDescription     | Detailed description of the service or procedure. |
| ProductCode    | Code representing the specific insurance plan or product. |


Diagnosis & Procedure:

| Variable | Description  |
| :------------ |:---------------|
| icd_code    | International Classification of Diseases code for diagnosis. |
| methode     | Method of service delivery (e.g., in-person, telemedicine). |


Financial Information:

| Variable | Description  |
| :------------ |:---------------|
| BilledAmount    | Total amount billed by the healthcare provider. |
| ApprovedAmount     | Amount approved for payment by the insurance company. |
| ShortfallAmount     | Amount not covered by insurance. |


Data Types
| Type     | Description                |
| :------- | :------------------------- |
| `Strings` | **Index**, **Days** |
| `Strings` | Location, Member ID, Claim_No, ProviderName, BenefitDescription, DetailDescription, ProductCode, icd_code, methode |
| `datetime64` | ServiceStartDate, ServiceStartEnd |
| `Floats` | BilledAmount, ApprovedAmount, ShortfallAmount


Key Improvements:


## Tools ⚙️

This project utilizes a variety of tools and technologies to perform data analysis and create predictive models:

- **Python** 🐍
  - `pandas` for data manipulation
  - `tableau` for visualization
  - `numpy` for numerical operations
  - `matplotlib` and `seaborn` for data visualization
  - `scikit-learn` for machine learning models
- **Google Colab Notebooks** for interactive analysis and visualization

## Modeling 🤖

This section focuses on predicting employee retention using machine learning models. We explore the following:

1. **Data Preprocessing**: Handling missing data, encoding categorical variables, and scaling features.
2. **Model Selection**: Building classification models to predict if an employee will leave or stay.
   - Logistic Regression
   - Decision Trees
     
3. **Model Evaluation**: Using metrics like accuracy, precision, recall, and F1-score to evaluate model performance.

The best-performing model can be deployed to predict future employee retention and guide HR strategies.

## How to Run the Project 🏃‍♀️

To run this project on **Google Colab Notebooks** :

1. Install git : If you haven't already, install git in your Colab environment. You can do this by running the following command in a code cell:
    ```bash
    !apt-get install git -y
    ```

2. Clone the repository: Clone the GitHub repository to your Colab environment using the git clone command:
    ```bash
    !git clone https://github.com/krizz-byte/Optimizing-Employee-Benefits-A-Data-Driven-Approach.git
    ```

3. Access the data: The repository you linked contains an "Employee.csv" file within a subdirectory called "data." You can access this file by setting your working directory:
    ```bash
    import os os.chdir('Optimizing-Employee-Benefits-A-Data-Driven-Approach')
    import pandas as pd employee_df = pd.read_excel('CLAIMRAW.xlsx')
    ```

## Contributing 🤝

We welcome contributions from the community! If you'd like to improve this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push your changes (`git push origin feature-name`).
5. Submit a pull request.

Please make sure to write clear, descriptive commit messages and follow the existing coding conventions.

## License 📄

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

If you have any questions or suggestions, feel free to open an issue or contact us!

>"Your work is going to fill a large part of your life, and the only way to be truly satisfied is to do what you believe is great work. And the only way to do great work is to love what you do." - Steve Jobs


