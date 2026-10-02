# Financial-Data-Automation-Pipeline (Python + Excel)
The Financial Data Automation Pipeline was developed to process a 2,653-page bank statement and transform the extracted financial records into a structured, validated, and categorized dataset.

# 1. Project Overview

This project automates the processing of a 2,653-page bank statement, transforming financial transaction data from PDF into a structured, validated, categorized, and report-ready Excel dataset.

The workflow combines Excel and Python/Pandas for data extraction, cleaning, validation, transaction classification, quality checks, and financial summarization.

Due to the confidential nature of the source data, the original bank statement and transaction-level records are not included in this repository. A redacted screenshot of the source document is provided for documentation.

# 2. Business Objective
•Convert a large bank statement from PDF to structured Excel data<br>
•Clean and validate extracted financial records<br>
• Automate transaction classification using Python<br>
• Cross-check classification results for data quality<br>
• Organize categorized transactions into structured Excel tables<br>
• Produce debit, credit, and final financial summaries<br>

# 3.Tools & Technologies

• Python / Pandas – Data cleaning, transformation, and transaction classification<br>
• Microsoft Excel – Data validation, structured tables, summaries, and reporting<br>
• PDF-to-Excel – Financial data extraction and structuring<br>

# 4.Data Extraction & Preparation
The source document contained 2,653 pages of bank statement records.<br>

The statement was converted from PDF into Excel, with transaction fields including:<br>

• Transaction Date<br>
• Narration<br>
• Reference<br>
• Debit<br>
• Credit<br>
• Balance<br>

Initial data preparation in Excel included:<br>

• Reviewing column structure and formatting<br>
• Checking dates and numeric fields<br>
• Reviewing debit and credit values<br>
• Identifying missing or inconsistent data<br>
• Reviewing transaction descriptions<br>

# 5. Python Data Processing

The validated Excel dataset was imported into Python using Pandas for further processing.<br>

Key processing steps included:<br>

• Standardizing transaction fields<br>
• Cleaning transaction descriptions<br>
• Processing debit and credit values<br>
• Preparing transaction records for classification<br>
• Applying rule-based classification logic<br>
• Identifying unclassified transactions<br>

# 6. Transaction Classification

Transaction classification was performed using transaction descriptions, debit/credit information, and identifiable transaction patterns.<br>

Example classification logic:<br>

if debit > 0 and any(keyword in description for keyword in [<br>
 "PP_FEE", "LEVY", "FEES", "VAT", "SMS", "STAMP DUTY", "COMMISSION" <br>
]):<br>
    return "Bank Charges"<br>

Additional classification rules were applied to other transaction patterns encountered in the dataset.<br>

# 7. Validation & Quality Control<br>

After classification, the results were cross-checked against the underlying transaction information.<br>

The validation process involved:<br>

• Reviewing classified transactions<br>
• Identifying unclassified transactions<br>
• Checking transaction descriptions against assigned categories<br>
• Reviewing debit and credit values<br>
• Refining classification rules where necessary<br>

Classification Workflow:<br>

Classify → Review → Identify Exceptions → Refine Rules → Reprocess → Validate<br>

# 8. Final Output

The processed dataset was exported back into Excel and organized into structured tables.<br>

The final output included:<br>

• Categorized transaction tables<br>
• Debit transaction summary<br>
• Credit transaction summary<br>
• Category-level transaction information<br>
• Final financial summary<br>

# 9. Data Privacy

The original financial records are confidential and have not been uploaded to GitHub.<br>

The repository excludes:<br>

• Raw transaction-level data<br>
• Original bank statement<br>
• Account numbers<br>
• Company information<br>
• Addresses<br>
• Customer information<br>
• Sensitive financial records<br>

<img width="641" height="421" alt="image" src="https://github.com/user-attachments/assets/dad49794-358a-4066-888c-746c1cbda55c" />


A redacted screenshot is included to demonstrate the source document without exposing confidential information.<br>

# 10. Project Outcome

The project transformed a large-volume financial statement into a structured, validated, categorized, and report-ready dataset using Python automation and Excel-based validation.<br>

The workflow demonstrates practical application of:<br>

• Financial Data Processing<br>
• Python & Pandas<br>
• Data Cleaning & Transformation<br>
• Data Validation<br>
• Data Quality<br>
• Transaction Classification<br>
• Automation<br>
• Financial Reconciliation<br>
• Excel Reporting<br>

# 11. Visualization / Documentation

A redacted screenshot of the original bank statement is included in the repository to demonstrate the source document and its scale.<br>

<img width="357" height="291" alt="image" src="https://github.com/user-attachments/assets/033e3253-9de1-4531-94d8-9a9a5f65eedb" />


Additional documentation and the Python classification script are provided in the repository.<br>

# 12. Author

Oluwatobi Adebamiro Adetutu<br>
Data Analyst | Python| Excel



