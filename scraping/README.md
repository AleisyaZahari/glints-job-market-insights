## 🕷️ Scraping & Preprocessing: Glints.com

This folder contains the **web scraping pipeline** and **data preprocessing** scripts used to collect and clean job and company information from [Glints.com](https://glints.com/id).

### 📌 Contents

| File | Description |
| ------------------------------------ | ------------------------------------------------------------------------- |
| `glints_scrape.ipynb`                | Scrapes job and company info using Selenium and BeautifulSoup             |
| `preprocessing.ipynb`                | Cleans and transforms raw data into structured format                     |
| `df_company_mask.xlsx`               | Cleaned dataset with 50% masking on sensitive fields (email, phone, etc.) |
| `df_company_mask_skill_explode.xlsx` | Masked dataset with exploded `Skills` column for visualization use        |


### 🔍 Scraping Highlights

- ✅ Collected **996 job listings** and **301 companies**
- 🌐 Extracted: Job title, location, category, requirements, salary, website, contact
- 📧 Enriched data with additional contact info (emails, phones) using scraping and regex

---

### 🧹 Preprocessing Steps

- Remove duplicates & irrelevant records
- Normalize locations (province/city)
- Extract structured contact data (emails, phone numbers)
- Add derived fields like `Days_Posted`, `Skill_Count`, `Email Domain`

---

### ⚠️ Privacy Note

To comply with data privacy and avoid leakage:
- Contact information like emails and phone numbers has been **50% masked**
- Social media links and full addresses have been **partially redacted**

For full access to the raw data, please contact the author (for educational purposes only).
