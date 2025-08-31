# InterviewCase_IDE
Example data. Not real data.

# Contoso AI IDE: Growth Modeling Assignment

## Executive Summary

Contoso AI IDE is an integrated developer environment for AI-assisted software development. The product team is seeking ways to grow the business and improve the product by leveraging user activity data to build predictive models that inform product, marketing, and sales strategies.

---

## 1. Product Overview

Contoso AI IDE offers three core features:

- **AutoComplete**: Autocompletion of code blocks in the main editor pane, similar to text or email autocomplete.
- **Chat**: A right-side pane for plain-language prompts and responses, similar to ChatGPT.
- **Agent**: A right-side pane for prompts that trigger code changes in the IDE, similar to Agent Mode in VS Code with GitHub Copilot.

---

## 2. Data Dictionary

| Column Name                | Definition                                                        |
|----------------------------|-------------------------------------------------------------------|
| `date`                     | Day of event activity                                             |
| `userid`                   | Anonymized user identifier tied to a user profile                 |
| `startdate`                | First day the userid has activity in the product                  |
| `plan`                     | Either “Free” or “Paid”                                           |
| `Status`                   | Either “Active” or “Cancelled” from the billing system at day end |
| `DayOfWeek`                | Day of the week for the `date` column                             |
| `Weekend`                  | Boolean: whether the day is a weekend                             |
| `DaysSinceStart`           | Days between `date` and `startdate`                               |
| `AI_AutoComplete_Success`  | Successful AutoComplete interactions                              |
| `AI_AutoComplete_Error`    | AutoComplete interactions with errors                             |
| `AI_Chat_Success`          | Successful Chat interactions                                      |
| `AI_Chat_Error`            | Chat interactions with errors                                     |
| `AI_Agent_Success`         | Successful Agent interactions                                     |
| `AI_Agent_Error`           | Agent interactions with errors                                    |

---

## 3. Feature Usage Limits

Feature usage limits by plan impact user experience and conversion potential.

| Plan   | AutoComplete (per day) | Chat (per day) | Agent (per day) |
|--------|------------------------|----------------|-----------------|
| Free   | 100                    | 10             | 5               |
| Paid   | 200                    | 50             | 20              |

---

## 4. Modeling Assignment

You are tasked with building predictive models using daily activity data for user accounts created between **3/3/2025 and 3/7/2025**, covering the next 60 days.

### Modeling Goals
Pick one of these modeling goals for your project: 
1. **Upgrade Prediction**: Predict whether a free user will upgrade to a paid plan.
2. **Retention Prediction**: Predict whether a user will be retained and continue using the product.

---

## 5. Deliverables

Prepare the following:

- **Business Presentation (10–15 min)**
  - Describe the problem/opportunity
  - Explain your modeling approach
  - Present model performance
  - Recommend actions for product, marketing, and sales teams

- **Technical Presentation (10–15 min)**
  - Describe the problem/opportunity
  - Detail your modeling approach and evaluation criteria
  - Present model performance
  - Recommend actions for data science and engineering teams

- **Code Files**
  - Submit all code used to generate your outputs (Python scripts, Jupyter notebooks, etc.)

---

## 6. Guidance for Presentations

- **Business Audience**: Focus on actionable insights, business impact, and recommendations.
- **Technical Audience**: Emphasize modeling decisions, feature engineering, evaluation metrics, and reproducibility.

---
