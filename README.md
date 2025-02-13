# Optimizing Employee Benefits: A Data-Driven Approach 📊
The primary objective of this project is to conduct a thorough analysis of our company's current employee benefits program to identify areas for improvement and optimization. By leveraging data-driven insights, we aim to develop a benefits package that is both cost-effective and highly valued by our employees.

## Project Overview 🚀

The primary objective of this project is to conduct a thorough analysis of our company's current employee benefits program to identify areas for improvement and optimization. By leveraging data-driven insights, we aim to develop a benefits package that is both cost-effective and highly valued by our employees. This repository contains data analysis, and machine learning models focused on analyzing and predicting employee retention outcomes.

## Table of Contents 📑

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Tools](#tools)
- [Analysis & Insights](#analysis--insights)
- [Modeling](#modeling)
- [How to Run the Project](#how-to-run-the-project)
- [Contributing](#contributing)
- [License](#license)

## Dataset 📈

The dataset used in this project contains employee records with various features that influence employee retention, such as:
![image](https://github.com/user-attachments/assets/ab1975ab-2e3d-4421-b3b1-652936d693a8)

This data can be sourced from publicly available datasets, HR systems, or simulated data for analysis.

## Technologies Used ⚙️

This project utilizes a variety of tools and technologies to perform data analysis and create predictive models:

- **Python** 🐍
  - `pandas` for data manipulation
  - `tableau` for visualization
  - `numpy` for numerical operations
  - `matplotlib` and `seaborn` for data visualization
  - `scikit-learn` for machine learning models
- **Jupyter Notebooks** for interactive analysis and visualization

## Analysis & Insights 🔍

Through exploratory data analysis (EDA), we uncover key patterns related to employee turnover. Some example insights include:

![image](https://github.com/user-attachments/assets/838ab09e-ce24-42ca-a937-a2efae20f758)
![image](https://github.com/user-attachments/assets/ff10048d-1e47-4b64-8bec-d83db4b32e7c)

Identifying trends, HR teams can create targeted strategies to improve employee satisfaction and reduce unnecessary turnover.

![image](https://github.com/user-attachments/assets/6add390d-d78c-4323-a4bc-e883c0d41a99)

In order to evaluate campaign performance, we focused on the following key metrics:
Signup Rate: The percent of people who see a campaign and subsequently sign up for a Row Health plan.
Cost per Signup: The average dollars spent in order to acquire a signup from each campaign.
Click through Rate: The percent of people who see a campaign and click on the associated link.
Signup Rate
Across campaign categories, Health for All campaigns had the best-performing signup rate (2.9%) and the second-highest number of signups (3.5K).
This high signup rate is due to the Health Awareness campaign type, which had by far the highest signup rate across all campaign types (3.72%).
Interestingly, the category with the highest number of signups - #HealthyLiving - had a comparably low signup rate at 0.3%.
Click through Rate
Across categories, Health for All and Benefit Updates performed nearly 3-4x better than the average CTR at 36% and 22%, respectively.
Within the two categories with high CTR, product promotion-based campaigns had relatively low CTR (0% and 7%).
Family Coverage Plan had high impressions but no clicks - this needs to be investigated and could be due to missing data or issues with the campaign.
Cost per Signup
Across campaign categories, Golden Years Security had by far the highest cost per signup ($124), as well as the lowest number of signups (23), compared to an average of $2.2.
Within the two campaign categories with highest cost per signup, info-based campaign types (like offers and policy info) drove high costs per signup.
Some COVID-based campaigns also had abnormally high CACs at $1.2-$1.3K.


## Modeling 🤖

This section focuses on predicting employee retention using machine learning models. We explore the following:

1. **Data Preprocessing**: Handling missing data, encoding categorical variables, and scaling features.
2. **Model Selection**: Building classification models to predict if an employee will leave or stay.
   - Logistic Regression
   - Decision Trees
   - Random Forest
   - XGBoost
3. **Model Evaluation**: Using metrics like accuracy, precision, recall, and F1-score to evaluate model performance.

The best-performing model can be deployed to predict future employee retention and guide HR strategies.

## How to Run the Project 🏃‍♀️

To run this project on your local machine:

1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/employee-retention-analysis.git
    cd employee-retention-analysis
    ```

2. Create and activate a virtual environment (recommended):
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the Jupyter notebook for analysis:
    ```bash
    jupyter notebook analysis.ipynb
    ```

5. For machine learning modeling, run the following script:
    ```bash
    python model_training.py
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


