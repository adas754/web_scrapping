# Session 2: Data & Workflows

**Unit 1: Introduction to Data Science**
**Hour: 2**
**Mode: Theory**

---

### 1. Objective

By the end of this session, students will be able to:
*   Differentiate between structured, semi-structured, and unstructured data.
*   Categorize data sources as internal or external.
*   Describe the steps of a standard data science workflow (OSEMN model).

---

### 2. Lecture & Discussion Points

#### Part 1: Types and Sources of Data

Data is not one-size-fits-all. Understanding its form is the first step.

**1. Based on Structure:**

*   **Structured Data:**
    *   **Description:** Highly organized, typically in a tabular format (rows and columns). It adheres to a strict schema.
    *   **Analogy:** A perfectly organized Excel spreadsheet or a library's card catalog.
    *   **Examples:**
        *   A customer database in a SQL table.
        *   An Excel file of sales records.
        *   Sensor readings from a machine (e.g., timestamp, temperature, pressure).

*   **Unstructured Data:**
    *   **Description:** Data with no predefined structure or organizational model.
    *   **Analogy:** A pile of assorted documents, photos, and audio recordings.
    *   **Examples:**
        *   The text of an email or a collection of news articles.
        *   Images from social media.
        *   Audio from a customer service call.
        *   Video from a security camera.
    *   *Note:* This type of data is the most abundant (~80% of all data) and often requires more advanced techniques to process.

*   **Semi-structured Data:**
    *   **Description:** A mix of the two. It doesn't fit into a rigid table, but it has tags or markers to separate semantic elements and enforce hierarchies.
    *   **Analogy:** A Word document with headings and paragraphs, which provides some structure but isn't a table.
    *   **Examples:**
        *   **JSON (JavaScript Object Notation):** Key-value pairs. Very common in web APIs.
        *   **XML (eXtensible Markup Language):** Uses tags to define elements.

**2. Based on Source:**

*   **Internal Data:**
    *   **Description:** Data generated and owned by the organization itself.
    *   **Examples:**
        *   Customer Relationship Management (CRM) data.
        *   Sales transaction history from a company database.
        *   Employee records.
        *   Website analytics from your own site.

*   **External Data:**
    *   **Description:** Data that originates from outside the organization.
    *   **Examples:**
        *   Publicly available government datasets (e.g., census data, weather data).
        *   Data from social media APIs (e.g., Twitter feed).
        *   Stock market data from a financial provider.
        *   Data purchased from third-party providers.

---

#### Part 2: The Data Science Workflow

A structured process is essential to avoid getting lost in the data. The **OSEMN (pronounced "awesome") model** is a popular framework.

**O - Obtain:**
*   **Goal:** Get the data.
*   **Activities:** Accessing databases, querying APIs, scraping web pages, reading from files (CSV, JSON, etc.).
*   **Key Question:** Can I get the data I need? Is it accessible?

**S - Scrub (or Clean):**
*   **Goal:** Fix the "dirty" data. This is often the most time-consuming step (can be 60-80% of the work!).
*   **Activities:**
    *   Handling missing values (imputing or removing).
    *   Correcting inconsistent formatting (e.g., "NY" vs "New York").
    *   Removing duplicate records.
    *   Handling outliers.
*   **Key Question:** Is the data accurate and consistent?

**E - Explore (Exploratory Data Analysis - EDA):**
*   **Goal:** Understand the patterns, relationships, and characteristics of the data.
*   **Activities:**
    *   Calculating descriptive statistics (mean, median, standard deviation).
    *   Creating visualizations (histograms, scatter plots, box plots).
    *   Looking for correlations between variables.
*   **Key Question:** What secrets is the data trying to tell me?

**M - Model:**
*   **Goal:** Use the data to make predictions or classify outcomes.
*   **Activities:**
    *   Feature Engineering (creating new variables that might be better predictors).
    *   Splitting data into training and testing sets.
    *   Applying machine learning algorithms (e.g., Linear Regression, Decision Trees).
    *   Evaluating model performance.
*   **Key Question:** Can I build a reliable model to predict the future?

**N - iNterpret (or Communicate):**
*   **Goal:** Present the findings in a clear, concise, and compelling way.
*   **Activities:**
    *   Creating dashboards (e.g., in Tableau or Power BI).
    *   Writing reports.
    *   Presenting to stakeholders.
    *   Translating technical results into business impact ("Storytelling with Data").
*   **Key Question:** How can I convince others that my findings are important and should be acted upon?

---

### 3. In-Class Activity

**Prompt:** "Let's map a simple problem to the OSEMN workflow: **Predicting a student's final exam score.**"

*   **Obtain:** Where would you get the data? (Student records, attendance logs, quiz scores).
*   **Scrub:** What problems might you find? (Missing quiz scores, attendance marked incorrectly).
*   **Explore:** What would you want to visualize? (A scatter plot of `hours_studied` vs. `final_score`).
*   **Model:** What kind of model would you use? (A simple regression model).
*   **iNterpret:** How would you present the results? (A simple statement like, "For every extra hour a student studies, our model predicts their score will increase by an average of 5 points.").

---

### 4. Session Wrap-up

*   Data comes in many forms: structured, semi-structured, and unstructured.
*   The OSEMN workflow provides a reliable map for any data science project.
*   Cleaning and Exploring are often the most critical and time-consuming phases.
*   **Next Session:** We will get our hands dirty and start the "Obtain" phase by loading and inspecting our first structured dataset with Python.