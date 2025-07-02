Here’s a professional and clear **README.md** and **Objective** section for your project, based on your detailed code and analysis:

---

## 📝 README.md

### 📌 Project Title:

**Electricity Usage and Financial Struggles of Low-Income Households in Bulacan**

---

### 📋 Objective:

This project aims to analyze the electricity consumption patterns, appliance ownership, and financial struggles of **low-income households in Bulacan** — specifically those earning **less than PHP 21,194 per month**. Using SQL and Python (Pandas, Matplotlib), we explore correlations between income, household composition, students at home, and electricity affordability.

---

### 📂 Dataset:

* File: `Survey.csv`
* Source: Self-reported survey data
* Key fields: Monthly electric bills, salary brackets, appliances owned, household structure, financial assistance, and struggles paying bills.

---

### ⚙️ Tools & Technologies:

* **Python**: `pandas`, `matplotlib`, `sqlite3`
* **SQL**: For table creation, filtering, and querying
* **SQLite**: For data storage and management

---

### 🧱 Project Structure (Steps Summary):

#### 🔹 **PART 1: Data Preparation**

1. Import `Survey.csv` into a DataFrame.
2. Compute average electricity bills (`avg_bill`).
3. Create a local SQLite database (`Survey_Database.db`).
4. Store and transform data:

   * Remove personal identifiers
   * Create focused tables: `Initial_Table2`, `Main_Table`, `With_Students`
   * Filter respondents from Bulacan and with students
   * Identify those using laptops/desktop computers

#### 🔹 **PART 2: Analysis on Low-Income Households**

1. **Filter respondents** earning **< PHP 21,194** (now `final_sample`)
2. Add `avg_bill` column (average of Month A, B, C)
3. Drop unnecessary columns, clean final dataset

#### 🔹 **Analysis Using Python**

* 🔍 How many live with **extended family**
* 📊 **Pie charts**: Extended family and households with students
* 📈 Compare **average budget vs. actual bill**
* 🧮 Analyze struggles:

  * Frequency of **struggling** and **failing** to pay bills
  * Appliance **ownership breakdown** (essential vs. luxury)
  * **Tech access** of student households (laptop/desktop)

---

### 🔎 Key Findings:

> > * **Average Bill**: PHP 3,498.95
> > * **Average Budget**: PHP 2,327.08
> >   → On average, **low-income households are overspending on electricity**.
>
> > * **Households with students** have slightly **higher bills**.
> > * Many respondents **struggle or fail** to pay their electric bill, frequently.
> > * **TVs and refrigerators** are commonly owned, while **air conditioners** and **electric water dispensers** are rare.
> > * Only a limited number of student households have **access to laptops or desktops**, affecting digital access.

---

### 📎 Conclusions:

This study provides critical insight into the **energy burden** faced by low-income families in Bulacan. The mismatch between budget and actual electricity costs, combined with frequent struggles to pay bills, highlights the need for:

* Financial assistance programs
* Appliance efficiency education
* Support for digital access among students

---

### 📁 Output Tables:

* `Main_Table`
* `With_Students`
* `sample` (Low-income)
* `final_sample` (Cleaned, analyzed subset)


