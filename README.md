# 💼 NaukriGulf Job Market Web Scraping

## 📌 Overview

This project is a **Web Scraping and Data Collection project** built using **Python and Selenium**.

The goal was to collect and analyze job market data from **NaukriGulf**, focusing on job opportunities related to **Data and AI** roles.

Using Selenium WebDriver, I automated the browsing process, searched for specific job roles, navigated through job listings, and extracted structured information from each job posting.

The scraping process resulted in a dataset containing **982 job postings**.

---

## 🎯 Project Objectives

The main objectives of this project were to:

* Automate job searching using Selenium.
* Collect real-world job market data.
* Scrape job postings from NaukriGulf.
* Extract relevant information from each job listing.
* Handle multiple search keywords.
* Navigate through multiple job listing pages.
* Store the collected data in a structured format.
* Prepare the dataset for further analysis and visualization.

---

## 🔎 Search Keywords

The scraping process focused on four different job searches:

```text
Data Engineer
AI Engineer
Data Analyst
Data Scientist
```

These keywords were selected to explore opportunities across different **Data and Artificial Intelligence career paths**.

---

## 📊 Dataset

The final dataset contains:

> **982 Job Postings**

For each job posting, the scraper collected the following information:

| Column        | Description               |
| ------------- | ------------------------- |
| `job_title`   | Title of the job position |
| `company`     | Hiring company            |
| `location`    | Job location              |
| `experience`  | Required experience       |
| `description` | Job description           |

### Example Record

```python
{
    "job_title": job_title,
    "company": company,
    "location": location,
    "experience": experience,
    "description": description
}
```

---

## 🔄 Web Scraping Workflow

The complete workflow can be summarized as:

```text
                NaukriGulf
                    │
                    ▼
            Search Job Roles
                    │
        ┌───────────┼───────────┐
        │           │           │
        ▼           ▼           ▼
 Data Engineer  AI Engineer  Data Analyst
                    │
                    ▼
              Data Scientist
                    │
                    ▼
           Selenium WebDriver
                    │
                    ▼
          Navigate Job Listings
                    │
                    ▼
            Extract Job Data
                    │
                    ▼
             Python Dictionary
                    │
                    ▼
             Pandas DataFrame
                    │
                    ▼
              982 Job Records
                    │
                    ▼
              Dataset / CSV
```

---

## 🤖 Selenium Automation

**Selenium WebDriver** was used to automate the browser and simulate user interactions.

The scraper was responsible for:

* Opening NaukriGulf.
* Searching for specific job roles.
* Navigating through job listing pages.
* Opening and reading job postings.
* Extracting job information.
* Handling multiple pages.
* Collecting the results into a structured dataset.

---

## 🧩 Data Extraction

For each job posting, the scraper extracted:

```python
job_data = {
    "job_title": job_title,
    "company": company,
    "location": location,
    "experience": experience,
    "description": description
}
```

The collected records were then stored and processed using Python.

---

## 🐍 Python & Pandas

Python was used as the main programming language for the scraping process.

After collecting the job postings, the data was organized into a **Pandas DataFrame**, making it easier to clean, inspect, and analyze the results.

Conceptually:

```python
df = pd.DataFrame(jobs)

print(df.shape)
```

Result:

```text
982 job postings
```

---

## 📈 Possible Analysis

The collected dataset can be used to investigate different aspects of the Data & AI job market, such as:

### 💼 Job Roles

* Distribution of Data Engineer, AI Engineer, Data Analyst, and Data Scientist positions.
* Most frequently advertised job titles.

### 🌍 Locations

* Countries and cities with the highest number of job postings.
* Geographic distribution of Data & AI opportunities.

### 🏢 Companies

* Companies with the highest number of job postings.
* Distribution of opportunities across organizations.

### 📚 Experience Requirements

* Most frequently requested experience levels.
* Relationship between job roles and required experience.

### 🧠 Skills & Technologies

The `description` column can be further processed using **Natural Language Processing (NLP)** to identify frequently requested technologies and skills such as:

```text
Python
SQL
Power BI
Machine Learning
AWS
Azure
Spark
Docker
```

---

## 🛠️ Technologies Used

* 🐍 **Python**
* 🤖 **Selenium WebDriver**
* 📊 **Pandas**
* 🌐 **NaukriGulf**
* 📁 **CSV**
* 🐙 **GitHub**

---

## 📂 Project Structure

```text
NaukriGulf-Web-Scraping/
│
├── 📂 data/
│   └── jobs.csv
│
├── 📂 screenshots/
│   ├── naukrigulf.png
│   └── dataset.png
│
├── 📂 src/
│   └── scraper.py
│
├── 📄 requirements.txt
├── 📄 README.md
└── 📄 .gitignore
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/USERNAME/NaukriGulf-Web-Scraping.git
```

Navigate to the project directory:

```bash
cd NaukriGulf-Web-Scraping
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Example:

```text
selenium
pandas
webdriver-manager
```

---

## ▶️ Running the Scraper

Run the Python scraper:

```bash
python src/scraper.py
```

The script will launch the browser and perform the automated job searches.

The collected job postings are then stored in a structured dataset.

---

## 📸 Project Screenshots

### 🌐 NaukriGulf Job Search

![NaukriGulf](screenshots/naukrigulf.png)

### 📊 Collected Dataset

![Dataset](screenshots/dataset.png)

---

## 🚀 Future Improvements

Some possible improvements for the project include:

* Add more job search keywords.
* Scrape additional job attributes such as salary and job type.
* Implement advanced pagination handling.
* Add automated data cleaning.
* Extract skills from job descriptions using NLP.
* Store the data in a SQL database.
* Build a Power BI dashboard.
* Schedule the scraper to collect updated job market data.
* Add logging and error handling.

---

## 📚 What I Learned

Through this project, I gained practical experience in:

* Web scraping using Selenium.
* Browser automation.
* Finding and interacting with web elements.
* Handling multiple search queries.
* Navigating dynamic web pages.
* Extracting structured data from websites.
* Using Pandas for data processing.
* Working with real-world job market data.
* Preparing scraped data for further analysis.

---

## 👨‍💻 Author

**Mohamed Elmisery**

Data Engineering | Python | SQL | Power BI | Web Scraping

---

⭐ **982 job postings collected from NaukriGulf using Selenium and Python.**
# Selinum-Wep-Scrabing-project
