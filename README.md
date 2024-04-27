# PII Detection in Student Writing: Competition Description

## Introduction
In today’s digital age, the abundance of educational data from various sources such as educational technology, online learning platforms, and research endeavors presents a significant challenge: the presence of personally identifiable information (PII). PII poses a barrier to the analysis and creation of open datasets that can advance education because releasing such data publicly risks exposing students to privacy breaches. To mitigate these risks, it's imperative to screen and cleanse educational data for PII before its public release, a process that can be streamlined through data science techniques.

## Problem Statement
Manually reviewing entire datasets for PII remains the most reliable screening method. However, this approach incurs substantial costs and limits the scalability of educational datasets. While techniques for automatic PII detection exist, primarily relying on named entity recognition (NER), they perform best for PII with common formatting such as emails and phone numbers. Challenges arise when detecting names and distinguishing between sensitive names (e.g., student names) and non-sensitive ones (e.g., cited authors).

## Competition Overview
The goal of this competition, hosted by Vanderbilt University in partnership with The Learning Agency Lab, an Arizona-based nonprofit, is to develop reliable automated techniques to detect PII in student writing. The competition aims to facilitate the creation of high-quality public educational datasets by automating PII detection, enabling researchers to harness previously unavailable data to develop effective tools and interventions that benefit teachers and students.

## Dataset
Participants are provided with a dataset containing student writing samples. These samples may contain various forms of PII, including but not limited to names, email addresses, phone numbers, and other sensitive information. Participants are tasked with building models capable of accurately identifying and labeling PII tokens within these documents.

## Evaluation Metric
Submissions are evaluated using micro Fβ, a classification metric that assigns value to both recall and precision. The value of β is set to 5, meaning that recall is weighted five times more heavily than precision. Participants must predict which tokens in the test set contain positive PII labels, excluding predictions of negative labels (outside labels represented as 'O').

## Submission Guidelines
For each document in the test set, participants must predict which token values have a positive PII label. Only predictions of positive PII label values should be included; outside labels (O) should not be included. Each row in the submission file should correspond to a single label found at a unique document-token pair. Additionally, the evaluation metric requires a row_id with an enumeration of predicted labels.

## Conclusion
This competition presents an opportunity to contribute to the development of automated PII detection techniques, thereby facilitating the creation of open educational datasets while safeguarding student privacy. By participating, researchers and data scientists can advance the science of learning and educational technology, ultimately benefiting teachers, students, and the broader educational community.

For more details and access to the dataset, please visit the competition page [here]([competition_link](https://www.kaggle.com/competitions/pii-detection-removal-from-educational-data/overview)).

---

**About the Hosts:**

**Vanderbilt University:** Vanderbilt is a private research university located in Nashville, Tennessee. It offers 70 undergraduate majors and a full range of graduate and professional degrees across 10 schools and colleges.

**The Learning Agency Lab:** An independent nonprofit based in Arizona, dedicated to developing the science of learning-based tools and programs for social good.

[Competition Link]: <[competition_link](https://www.kaggle.com/competitions/pii-detection-removal-from-educational-data/overview)>
