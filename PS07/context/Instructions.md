# PM-04-PS07: Adhere to industry best practices

## Scope of Practical Skill

You are required to perform the task below and your Supervisor/facilitator/mentor will assess you based on the below observation checklist attached:

Given a PDD and workflow files, the learner must be able to:

- PA0701 Apply code quality principles and best practices to maintain readability of the code, such as
- Secure coding practices naming convention standards and compliance
- zero usage of junk code
- Componentization
- PA0702 Align the code development process to chosen platform (e.g., Agile) methodology principles to coordinate with cross-functional teams, and ensure timely delivery
- PA0703 Provide data/information in standard formats in adherence to industry best practices
- PA0704 Ensure compliance with internal control or audit requirements

## Applied Knowledge

- AK0701 Scripting / programming of languages to understand the bot's source code
- AK0702 The range of standard templates and tools available and how to use them
- AK0703 Processes and workflows pertaining to the RPA solution:
- quality PPD
- must know how to read the diagram
- given a PPD and must code the solution for it
- AK0704 Software and other tools employed in the RPA solution
- AK0705 How to work on various operating systems - every company will have their own OS dependent on the company.

## Internal Assessment Criteria

- IAC0701 Readability of code, including detailed variable/argument names, activity names and descriptions, is ensured
- IAC0702 Unused or commented-out code blocks are removed
- IAC0703 Automation is separated into reusable workflow files that are useful, based on application
- IAC0704 Dynamic variables/arguments are used, avoiding hard coding, and data cleaned before analysis (such as preparing strings to be compared to each other)
- IAC0705 Expectations for design, development, testing, corrections, and delivery to production are set
- IAC0706 Outputs are provided in a PDD defined format
- IAC0707 Care is taken that all compliance considerations are met, including not logging/exposing sensitive data

## Practical application task - PS07

### SECTION 7: PM-04-PS07: Adhere to industry best practices

**Scenario**

The financial services sector in South Africa, a key pillar of the economy, faces significant challenges from fraudulent activities. Major banks like Standard Bank, Nedbank, and First National Bank (FNB) invest heavily in technology to combat fraud. Automating the initial screening of high-volume transactions is a critical use case for RPA, as it frees up human analysts to focus on complex, high-value cases. This case study simulates a common real-world scenario where you must build an automation to pre-screen a list of transactions for suspicious activity.

**Practical Assessment Task**

You will develop two separate but functionally identical RPA solutions: one using **UiPath** and another using **Microsoft Power Automate Desktop**. Both solutions must adhere to the PDD provided.

**The Scenario**

Your team is responsible for developing a bot that automates the fraud detection process for the "Rapid Transfer" system. The bot will:

- Read a daily list of all rapid transfers from an Excel file.
- Identify transactions that meet the following high-risk criteria:
  - The transfer amount is greater than R10,000.
  - The transaction is marked as "International".
  - The transaction is not yet "Verified".
  - The recipient's account number is on a "Suspicious Accounts List".
- For each high-risk transaction, the bot must generate a detailed report and save it as a PDF file in a specified folder.
- The bot must also produce a summary report in a structured data format (CSV).

**Required Materials**

- **Process Definition Document (PDD)**: A detailed PDD outlining the process flow, business rules, and technical requirements.
- **Data Set**: Facilitator will provide a zipped folder containing the following:
  - Daily_Transactions.xlsx: The main dataset of transactions to be processed.
  - Suspicious_Accounts.csv: A list of account numbers flagged for suspicious activity.
  - Transaction_Report_Template.pdf: A template for the individual transaction reports.

**Task Breakdown**

You will perform the following steps for both the UiPath and Power Automate solutions.

- **PDD Review and Understanding**: Carefully read and understand the provided PDD. You must be able to translate the described process flow and business rules into a technical solution.
- **Project Setup**
  - Create a new project in both UiPath and Microsoft Power Automate Desktop.
  - Set up a project folder structure that separates input data, output reports, and reusable components.
- **Code Development and Implementation**:
  - **Componentization**: Break down the main automation into separate, reusable workflow files. For example, one workflow for reading data, another for processing transactions, and a third for generating reports.
  - **Readability**: Use clear, descriptive names for all variables, arguments, and activities. For example, instead of var1, use transactionAmount.
  - **Data Handling**: Use variables and arguments to pass data between workflows. **Avoid hard-coding** any values, such as file paths or thresholds (e.g., R10,000).
  - **Compliance**: Ensure that no sensitive information (e.g., full account numbers) is logged or written to non-secure files beyond the required outputs.
  - **Zero Junk Code**: Remove all unused variables, commented-out code, and placeholder activities before finalizing the solution.
- **Output Generation**:
  - **Individual Reports**: For each transaction that meets the high-risk criteria, generate a PDF report based on the provided template. The file name should be Report\_&lt;TransactionID&gt;.pdf.
  - **Summary Report**: Create a single CSV file named High_Risk_Transactions_Summary.csv that contains the TransactionID, Amount, RecipientAccount, and Reason for all flagged transactions. The reason should be a string concatenating all the criteria met (e.g., "Amount > R10,000 | International | Not Verified").
- **Documentation and Handover**:
  - Create a brief document or README file that explains your approach, component structure, and how the automation aligns with the PDD.
  - Explain how your solution would fit into an agile sprint (e.g., "This automation would be the output of a single sprint, with initial user story mapping and testing done in the sprint."). (PA0702, IAC0705)

**Student Worksheet**

**Part 1: Self-Assessment and Reflection**

Before submitting your project, review your code and answer the following questions.

- **Code Readability**: Describe the naming conventions you used for variables, arguments, and activities. Provide a specific example from your code.

……………………………………………………………………………………………………………………………………………………………………………………………………

- **Componentization**: Explain how you separated your automation into reusable components. List the names and functions of your main workflow files.

………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………

- **Hard Coding**: Identify any potential hard-coded values in your solution and explain how you avoided them using variables or configuration files.

………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………

- **Compliance**: Detail the specific steps you took to ensure sensitive data, such as account numbers, was handled securely and not exposed in logs or other outputs.

………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………

- **Junk Code**: Did you find any unused or commented-out code during your final review? What steps did you take to remove them?

………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………

- **Agile Alignment**: How would your developed solution fit into an agile development cycle? Which agile principles did you apply (e.g., frequent delivery, collaboration)?

………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………

- **Output Format**: Confirm that your summary report (CSV) and individual reports (PDFs) meet the formatting requirements outlined in the PDD.

………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………………

**Part 2: Submission Checklist**

- UiPath project folder (zipped)
- Microsoft Power Automate Desktop project folder (zipped)

Generated output files (PDF reports and CSV summary)

- Completed Student Worksheet (this document)
- A copy of the PDD provided.

**Marking Rubric**

| Criteria                            | Description                                                                                                                                                                                                                                         | Marks |
| ----------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| 1\. Code Quality & Secure Practices | Code is readable, maintainable, and free of junk code. Variables/arguments named clearly. Sensitive data (e.g., accounts) masked where appropriate. No hard-coding of thresholds or file paths.                                                     | 5     |
| 2\. Componentization & Structure    | Automation is broken into reusable components/workflows. Proper folder/project structure is set up (inputs, outputs, configs). Clear documentation of workflow responsibilities.                                                                    | 3     |
| 3\. Compliance & Controls           | Evidence that internal controls and audit requirements are considered (e.g., no exposure of sensitive data in logs, compliance with handling rules). Alignment with security requirements.                                                          | 3     |
| 4\. Output Generation & Formatting  | Correctly generates:<br><br>• Individual PDF reports using the provided template,<br><br>• High_Risk_Transactions_Summary.csv with correct structure (TransactionID, Amount, RecipientAccount, Reason). Reports conform to formatting requirements. | 4     |
| 5\. Agile Methodology Alignment     | Student explains (in README or worksheet) how the automation fits into an agile sprint. Evidence of agile principles (iterative design, modular delivery, collaboration readiness).                                                                 | 2     |
| 6\. Reflection & Documentation      | Student worksheet completed thoughtfully: clear examples of naming conventions, explanation of componentization, handling of hard-coding, compliance, agile reflection. README included and clear.                                                  | 3     |

# Evaluation checklist

| **NAME:** Baholo<br><br>**SURNAME:** Mokoena<br><br>**COMPANY**: Mindworx<br><br>**ID**: 901228535709 | **DATE:** 10 March 2026<br><br>**TIME:** 13:00 |
| ----------------------------------------------------------------------------------------------------- | ---------------------------------------------- |

<div class="joplin-table-wrapper"><table><tbody><tr><th colspan="2"><p><strong>EVALUATION CRITERIONS</strong></p></th><th><p><strong>COMPETENT</strong></p></th><th colspan="2"><p><strong>NOT YET</strong></p><p><strong>COMPETENT</strong></p></th><th><p><strong>COMMENTS OR ACTION REQUIRED</strong></p></th></tr><tr><td colspan="2"></td><td></td><td colspan="2"></td><td></td></tr><tr><td colspan="2"><p><strong>Ability of the learner to:</strong></p></td><td></td><td colspan="2"></td><td></td></tr><tr><td colspan="2"><p>PA0701 Apply code quality principles and best practices to maintain readability of the code, such as</p><ul><li>Secure coding practices naming convention standards and compliance</li><li>zero usage of junk code</li><li>Componentization</li></ul></td><td></td><td colspan="2"></td><td></td></tr><tr><td colspan="2"><p>PA0702 Align the code development process to chosen platform (e.g., Agile) methodology principles to coordinate with cross-functional teams, and ensure timely delivery</p></td><td></td><td colspan="2"></td><td></td></tr><tr><td colspan="2"><p>PA0703 Provide data/information in standard formats in adherence to industry best practices</p></td><td></td><td colspan="2"></td><td></td></tr><tr><td colspan="2"><p>PA0704 Ensure compliance with internal control or audit requirements</p></td><td></td><td colspan="2"></td><td></td></tr><tr><td colspan="6"><p><strong>GENERAL COMMENTS OF OBSERVER:</strong></p></td></tr><tr><td><p>Date: 10 March 2026</p></td><td colspan="3"><p>Time started: 13:00</p></td><td colspan="2"><p>Time completed:17:00</p></td></tr><tr><td><p><strong>MENTOR/SUPERVISOR NAME</strong></p><p><strong>Baholo Mokoena</strong></p></td><td colspan="3"><p><strong>MENTOR/SUPERVISOR SIGNATURE</strong></p><p><img alt="A black background with a black square

AI-generated content may be incorrect." src="data:image/png;base64,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"></p></td><td colspan="2"><p><strong>LEARNER</strong></p><p><strong>(SIGNATURE)</strong></p><p><strong>……………………………….</strong></p></td></tr></tbody></table></div>