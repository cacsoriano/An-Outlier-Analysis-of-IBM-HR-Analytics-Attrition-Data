# Two Week Notice: An Outlier Analysis of IBM HR Analytics Attrition Data

![](https://github.com/cacsoriano/An-Outlier-Analysis-of-IBM-HR-Analytics-Attrition-Data/raw/main/img/Employee-Attrition.png)

Open `Technical_Report.ipynb` to view the full report.

### Executive Summary

"It is said that employees don't leave companies, they leave people." (Dale Carnegie). Employee attrition is a challenge faced by both employers and employees. Employers typically don't want to incur the costs of lost productivity and hiring while employees who are satified within their current work environment wouldn't typically leave. This project proposed a methology of detecting employees who are prone to resigning by comparing the similarity of their profile with that of records from all employees within the organization using Gower's Distance. Gower's Distance is a metric that quantifies the similarity of numerical and categorical data between two records, with the assumption that an employee with a different profile from others in the organization would be at risk of resigning. Statistical-based outlier analysis was employed using p-values to determine the threshold for outliers. Profiles who have resigned are considered outliers while e ployees currently working in the organization would be the inliers. By detecting potential outliers early on, management could provide intervention to for the employees at risk of attrition.

Recall was the chosen metric for this project because a company would not want to produce any false negatives while false positives would be far more acceptable to be able to campture any potential attrition case with intervention. Using IBM's HR Analytics Employee Attrition and Performance dataset, our methodology produced a recall score of 92%. While classification methods produced a higher accuracy of 97% these methods needed oversampling and aren't directly interpretable. On the other hand, the use of Gower's Distance is directly interpretable because it simply uses the similarity between a profile to other profiles. The authors recommend for future study an optimal frequency of updating the set threshold, since the features of the employee records would change from time to time, finding the ideal number of employee samples used to compare profiles for the test set and expanding the use of this methodology to monitor current employee engagement and identifying candidates who are good fits during the hiring process.

In partial fulfillment of the requirements for AIM MSDS 2022 Advanced Data Mining under Prof. Christian Alis.
