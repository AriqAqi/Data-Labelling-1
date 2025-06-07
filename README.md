# Health App Acceptability Text Annotation Project

This project focuses on text data labeling/annotation to support machine learning classification related to the adoption of health applications in Indonesia.

##  Background

In Indonesia, health applications are becoming an important way to improve access to and the quality of healthcare. However, even though more health apps are being developed, many people still don't use them regularly. This low usage happens for several reasons—such as limited access to digital tools, different levels of computer or smartphone skills, and worries about how their personal data is used.

This project aims to better understand user acceptance of health apps by analyzing text responses through a machine learning method called **Long Short-Term Memory (LSTM)**. The goal is to categorize text data based on **technical aspects** that influence app adoption.

##  Dataset Overview

- **Source**: Interviews with health app users in Bandung Regency, Indonesia  
- **Focus Group**: Mostly parents with children  
- **Data Format**: Excel (.xlsx)  
- **Total Responses**: 46 respondents  
- **Content**: Speech-to-text transcripts  
- **Size**: 
  - Over 1,000 rows  
  - Approximately 37,000 characters  

##  Annotation Guidelines

This project aims to categorize user responses from health app users based on technical aspects that influence the adoption of mobile health applications. Below are the definitions of each label that annotators should refer to when performing data labeling.

Each user statement can be tagged with one or more of the following technical aspects:

| **Label** | **Description** |
|-----------|------------------|
| **Perceived Ease of Use** | The individual’s perception that a specific technology can be used effortlessly and without significant effort. |
| **Performance Expectancy** | The belief that utilizing the system will improve the user’s ability to perform tasks more effectively. |
| **Effort Expectancy** | The degree to which the system is easy to use, reducing the physical and time burden on the user. |
| **System Quality** | The technical attributes that determine how well the system delivers accurate, reliable information. Poor system design may lead to limited access. |
| **Perceived Usefulness** | The degree to which the user believes the system improves their efficiency and helps them achieve their goals. |
| **Facilitating Conditions** | The user’s belief in the availability of support and technical infrastructure to use the system effectively. |
| **Resistance to Change** | A user’s reluctance or hesitation toward using new technology due to fear, discomfort, or unfamiliarity. |
| **Technological Incapability** | Lack of access to or availability of necessary technology to operate or use the application. |
| **Functionality** | The ability of the app to provide health services and information. High-quality features and information positively affect user acceptance. |
| **Cost** | Any financial burden, including purchasing devices, app subscriptions, or mobile data costs, that discourages adoption. |

---

### Label Encoding System

Each response is annotated using integer values to represent the sentiment or relevance of each aspect:

- **0 — Not Related**: The response does not mention or imply the aspect.
- **1 — Negatively Related**: The response expresses dissatisfaction or a negative experience related to the aspect.
- **2 — Positively Related**: The response expresses satisfaction or a positive experience related to the aspect.

>  Important:
> - A single response can be related to multiple aspects.
> - Each aspect must be labeled independently using 0, 1, or 2.

---

###  Example Annotation Table

| **Text Snippet** | **Ease of Use** | **System Quality** | **Cost** | **Usefulness** | ... |
|------------------|------------------|----------------------|----------|------------------|------|
| "The app is very simple and easy to use." | 2 | 0 | 0 | 1 | ... |
| "I don’t use the app because our internet is unstable." | 0 | 0 | 0 | 0 | ... |
| "It crashes frequently and is hard to rely on." | 1 | 1 | 0 | 0 | ... |
| "The subscription is too expensive for me." | 0 | 0 | 1 | 0 | ... |
| "It helps me monitor my child's health growth easily." | 2 | 0 | 0 | 2 | ... |

---
