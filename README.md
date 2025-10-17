# InterviewCase_IDE
Example data. Not real data.

# Contoso AI IDE: Growth Modeling Assignment

## Executive Summary

Contoso AI IDE is an integrated developer environment for AI-assisted software development. The product team is seeking ways to grow the business and improve the product by leveraging user activity data to inform product, marketing, and sales strategies.

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

Feature usage limits by plan:

| Plan   | AutoComplete (per day) | Chat (per day) | Agent (per day) |
|--------|------------------------|----------------|-----------------|
| Free   | 100                    | 10             | 5               |
| Paid   | 200                    | 50             | 20              |

---

## 4. Modeling Assignment

You are tasked with using daily activity data for user accounts created between **3/3/2025 and 3/7/2025**, covering the next 60 days, to inform product strategy. Use the .csv file in this repository.

### Analysis Goals
Mandatory questions to answer: 
- How many new Free and Paid accounts were created in the week of 3/3-3/7?
- How many accounts are still using the product in the following days and weeks? What is our retention rate?
- How many Free accounts upgraded to paid? What is our conversion rate?
- How many of our Paid accounts have cancelled?

Additional questions the product team might be interested in (not in priority order):
- What is the relationship between feature usage and product retention or conversion to paid?
- What is the relationship between feature errors and product retention or conversion to paid?
- Do we observe distinct differences in user behavior between different user groups?
- When are users most likely to convert? What does their user behavioral user journey look like?
- Any other insights or recommendations you have.

---

## 5. Deliverables

Prepare the following:

- **Business Presentation (10–15 min)** : With a PowerPoint or slide deck, share the following for a Leadership Team audience: 
  - Describe the problem/opportunity
  - Present insights
  - Recommend actions for product, marketing, and/or sales teams

- **Technical Discussion (10–15 min)** : Prepare the following to share with your data science colleagues, and you will walk us through your code files.
  - Detail your analysis approach and evaluation criteria
  - Recommend actions for data science and engineering teams

- **Code Files**
  - Submit all code used to generate your outputs (Python scripts, Jupyter notebooks, queries, etc.) and your final products.

---

## 6. Guidance for Presentations

- **Business Audience**: Focus on actionable insights, business impact, and recommendations.
- **Technical Audience**: Emphasize analysis/modeling decisions, feature engineering, evaluation metrics, and reproducibility.

---
