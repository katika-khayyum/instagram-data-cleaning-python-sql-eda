# 📊 Parse-Data-Aalysis

_Collected raw Instagram data containing user details such as posts, followers, and bios, which included inconsistencies and missing values, requiring preprocessing for reliable analysis._

---
## 📌 Tables of Content
- <a href="#overview">Overview</a>
- <a href="#problem-statement">Problem Statement</a>
- <a href="#dataset">DataSet</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-cleaning--preparation">Data Cleaning & Preparation</a>
- <a href="#json-conversion">JSON Conversion</a>
- <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#author-contact">Author & Contact</a>
---

<h2><a class="anchor" id="overview"></a>Overview</h2>

This project focuses on analyzing Instagram profile data by cleaning inconsistent raw data and extracting meaningful insights. The dataset contains information such as usernames, posts, followers, following count, bios, and profile links.

---

<h2><a class="anchor" id="problem-statement"></a>Problem Statement</h2>

The collected dataset contains:

- Missing values
- Inconsistent spacing
- Different formats (e.g., 40K, 1M)
- Unstructured raw data

The goal is to clean, standardize, and analyze this data to understand relationships between posts and followers.

---

<h2><a class="anchor" id="dataset"></a>DataSet</h2>
📂 DataSet
- Raw data collected from Instagram profiles txt file in initialdata.txt.
- Includes:Username,Number of posts,Followers,Following,page_bio,Profile links
- Data was noisy and unstructured

---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>
🛠️ Tools & Technologies
- SQL(Common Table Expressions, filtering,groupby)
- Python(Pandas, Numpy, Matplotlib, Seaborn, Regular Expressions (re))

---
<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

```
parse-data-analysis/
├──README.md
├──requirements.txt
├──.gitignore
├──initialdata.txt
├──cleaned_data.ipynb # jupyter Notebook
```
---
<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Cleaning & Preparation</h2>

🧹 Data Cleaning & Preparation
- Step 1: Collected raw Instagram data and identified inconsistencies
- Step 2: Removed extra spaces and standardized formatting using re
- Step 3: Structured the data and stored each profile as a list element
- Step 4: Converted values (e.g., 40K → 40000, 1M → 1000000) for consistency
- Step 5: Transformed cleaned data into JSON format for better readability
---
<h2><a class="anchor" id="json-conversion"></a>JSON Conversion</h2>

JSON Conversion
- Converted cleaned data into JSON format(Json.dumps)
- Improved readability and usability
---

<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>

📊 Compared number of posts vs followers
- Identified: Profiles with high followers but low posts
- Profiles with posts less than 500
- Visualized data using:Scatter plots, Box plots, Histplot

🔍 Key Findings
- Profiles with consistent posting tend to have higher followers.
- Some profiles have high followers despite fewer posts (influence factor).
- Data cleaning significantly improved analysis accuracy.

---

<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

▶️ How to Run This Project:
1. Clone the repository:
```bash
git clone <https://github.com/katika-khayyum/instagram-data-cleaning-python-sql-eda.git>
```
2. Load the CSVs and into the database:
```bash
cd project:
pip install pandas numpy matplotlib seaborn
```
- 3.Run the project: python data_cleaning.py
---
<h2><a class="anchor" id="author-contact"></a>Author & Contact</h2>

👤 Katika Md Khayyum
Data Science
📧 Email: abdulqhaiyyum0786@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/katika-md-khayyum-510a6a315/)