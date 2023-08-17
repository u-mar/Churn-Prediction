# Hotel Reservation Churn Prediction Project
![Hotel](data/hotel.jpg)
## Overview
Welcome to the Hotel Reservation Churn Prediction Project. In this initiative, we delve into the challenge of declining hotel revenue resulting from a rising number of reservation cancellations. By harnessing the power of advanced data analysis and machine learning techniques, our project is dedicated to unearthing insights and devising strategies to mitigate this issue and revitalize revenue growth within the realm of hospitality.

## Business and Data Understanding
**Stakeholder Audience**: Our primary stakeholders encompass hotel executives, management teams, and decision-makers. Their vested interest lies in addressing the recent downturn in hotel revenue, precipitated by an uptick in reservation cancellations. This project seeks to empower them with data-driven solutions to combat this challenge effectively.

**Dataset Choice**: The foundation of our analysis is a meticulously curated dataset obtained from two prominent hotel categories: resort and city hotels situated in Portugal. Sourced from Property Management System (PMS) SQL databases, this dataset comprises 31 variables and spans an extensive 119,390 observations. Encompassing bookings from July 1, 2015, to August 31, 2017, it provides a comprehensive snapshot of the booking landscape, encapsulating both successful check-ins and instances of cancellations.

## Modeling
In the "Modeling" phase, we delved into building predictive models to anticipate and mitigate reservation cancellations. We trained six distinct machine learning models, each with its unique strengths and characteristics. These models were trained on a comprehensive dataset encompassing various features that influence reservation cancellations.

## Evaluation
In the "Evaluation" stage, we rigorously assessed the performance of the six trained models. We utilized evaluation metrics such as accuracy, f1-score, precision, and recall to measure the models' effectiveness in predicting reservation cancellations. Additionally, we conducted thorough cross-validation and explored potential overfitting or underfitting issues to ensure the models' reliability.

## Model Selection
With the goal of identifying the most effective predictive model, we evaluated each model's performance on the test data. The following table presents the performance metrics for each model:

| Model          | Accuracy | f1-score | Precision | Recall |
|----------------|----------|----------|-----------|--------|
| Logistic       | 75       | 66       | 53        | 78     |
| Decision Trees | 82       | 74       | 77        | 71     |
| KNN            | 81       | 63       | 87        | 39     |
| Random Forest  | 70       | 72       | 69        | 74     |
| Adaboost       | 77       | 72       | 71        | 72     |
| XGBOOST        | 84       | 70       | 69        | 70     |

Based on the comprehensive analysis of these metrics, we have selected the **XGBOOST** model as our final choice due to its remarkable accuracy of 84% and balanced performance in other metrics.

## Conclusion
Our analysis has uncovered profound insights into the factors influencing reservation cancellations within the hotel industry. Based on these insights, we have formulated a series of strategic recommendations aimed at mitigating reservation cancellations and enhancing revenue collection:

- Offer special promotions and incentives during peak months to encourage confirmed reservations.
- Strategically promote international bookings through discounts or tailored services.
- Enhance room types with lower booking rates to boost their appeal and minimize associated changes.
- Implement targeted discounts for local customers to discourage cancellations.
- Establish effective communication channels with customers who have a history of cancellations.
- Foster collaborations with Travel Agencies and Tour Operators to capitalize on their reservation potential.
- Consider restrictions on reservations from Undefined market channels to reduce cancellations.

These recommendations have the potential to reshape operational strategies, optimize resource allocation, and bolster guest satisfaction.
