RPA Fraud Detection Dataset - README
Generated: 2025-09-15 20:45:45 UTC

Contents of this package:
- Daily_Transactions.xlsx      : Main dataset of rapid transfers to be processed by the RPA bot.
  Columns: TransactionID, Date, SenderAccount, RecipientAccount, Amount, Currency, TransferType, Country, Verified, Description
  Notes: Amounts are in ZAR. Several rows intentionally meet 'high-risk' criteria:
    - Amount > R10,000
    - TransferType == 'International'
    - Verified == 'No'
    - RecipientAccount is included in Suspicious_Accounts.csv

- Suspicious_Accounts.csv      : List of recipient account numbers flagged for suspicious activity. Use this list to check whether a transaction's recipient is suspicious.

- Transaction_Report_Template.pdf : PDF template with placeholders (e.g., {TransactionID}). Bots should replace placeholders and save per-transaction PDFs named Report_<TransactionID>.pdf

Usage suggestions for the assessment:
- Read Daily_Transactions.xlsx as the input source.
- Cross-check RecipientAccount values against Suspicious_Accounts.csv.
- Flag transactions where any of the following are true:
    * Amount > 10000
    * TransferType == 'International'
    * Verified == 'No'
    * RecipientAccount in Suspicious_Accounts.csv
  Concatenate reasons into the 'Reason' field in the summary CSV, e.g., 'Amount > R10,000 | International | Not Verified'.

- For compliance, mask account numbers in logs and generated PDFs (e.g., 62000*****1234).

Files in this folder were created for educational use and do NOT contain any real personal data.
