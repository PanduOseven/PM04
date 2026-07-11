PM-04-PS06: Organize projects for efficiency and easy maintenance

## Scope of Practical Skill

You are required to perform the task below and your Supervisor/facilitator/mentor will assess you based on the below observation checklist attached:

Given a workflow design, the learner must be able to:

- PA0601 Insert comments for each logical paragraph (where it is coming from, reason, what is outcome) for future reference
- PA0602 Maintain source control in a repository by applying version control protocols

## Applied Knowledge

- AK0601 Scripting / programming of languages to understand the bot's source code
- AK0602 The range of standard templates and tools available and how to use them
- AK0603 Processes and workflows pertaining to the RPA solution:
- quality PPD
- must know how to read the diagram
- given a PPD and must code the solution for it
- AK0604 Software and other tools employed in the RPA solution
- AK0605 How to work on various operating systems - every company will have their own OS dependent on the company

## Internal Assessment Criteria

- IAC0601 Care is taken that the code is readable and easy to maintain
- IAC0602 Comments and annotations are included and actions renamed to be descriptive
- IAC0603 Reusability of components is ensured by using variables and arguments and to avoid hard-coding values
- IAC0604 Code is regularly checked into the main branches using version control software

## Practical application task - PS06

### SECTION 6: PM-04-PS06: Organize projects for efficiency and easy maintenance

Scenario

South African organisations such as banks (ABSA, Standard Bank), retail companies (Shoprite, Pick n Pay), and government entities (Home Affairs, SARS) increasingly adopt RPA to automate repetitive tasks such as invoice processing, employee onboarding, and handling customer queries.

In this scenario, you will simulate one such use-case. Automating the processing of student bursary applications from a CSV dataset (applicants' details). The bot will read the dataset, filter applicants by criteria, and generate a result log.

The Department of Higher Education and Training (DHET) receives thousands of student bursary applications. An RPA solution is needed to filter eligible applicants and record results automatically.

**Dataset (Provided): bursary_applications.csv**

**Task Breakdown**

**Part 1: Workflow Documentation & Commenting (PA0601 + IAC0602)**

- Open UiPath/Power Automate.
- Build a workflow that reads the CSV dataset.
- Insert **comments in every section** explaining:
  - Where data is coming from
  - Why filtering is applied
  - Expected outcome

Assessment: Clear, descriptive comments.

**Part 2: Version Control (PA0602 + IAC0604)**

- UiPath: Connect project to **GitHub/GitLab**.
- Power Automate: Store flows in **OneDrive/SharePoint** with version history.
- Commit changes after each logical enhancement.

Assessment: Evidence of multiple commits with meaningful messages.

**Part 3: Applied Knowledge - Scripting & Templates (AK0601 + AK0602)**

- UiPath: Use VB.NET expression for filtering data table:

| vb                                                           |
| ------------------------------------------------------------ |
| dt.Select("AverageMark >= 70 AND HouseholdIncome <= 150000") |

- Power Automate: Use **Filter array** action with condition expressions.
- Explore UiPath **REFramework template** and Power Automate **Approval workflow template**, then adapt them for bursary filtering.

Assessment: Proper use of expressions and templates.

**Part 4: Process Definition Document (PPD) to Workflow (AK0603)**

- Given PPD diagram:

**PPD Example**:

- Input dataset → 2. Validate data → 3. Filter applicants → 4. Output eligible applicants → 5. Log results.

- Students must **translate this PPD into an automated workflow**.

Assessment: Workflow matches the PPD.

**Part 5: Tools & Cross-OS Usage (AK0604 + AK0605)**

- Students document differences:
  - UiPath (Windows-only desktop app, requires installation).
  - Power Automate (browser/cloud-based, runs on Windows/macOS/Linux).

Assessment: Short reflective comparison.

**Final Deliverables**

- UiPath workflow project folder OR Power Automate flow export.
- GitHub/SharePoint repository link.
- Written reflection on OS differences.
- Commented workflow aligned with PPD.

**Assessment Rubric**

| **Criteria**                                                       | **Description**                                                                                                                                                   | **Marks** |
| ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| **1\. Workflow Documentation & Commenting (PA0601, IAC0602)**      | Workflow includes clear, relevant comments for each logical step (data input, filtering, output, logging). Actions are renamed with descriptive labels.           | **4**     |
| **2\. Version Control (PA0602, IAC0604)**                          | Student connects workflow to GitHub (UiPath) or OneDrive/SharePoint (Power Automate). Multiple commits/versions are demonstrated with meaningful commit messages. | **3**     |
| **3\. Applied Knowledge - Scripting & Templates (AK0601, AK0602)** | Correct use of scripting expressions (e.g., filtering dataset). Correct application of at least one standard template/tool in UiPath or Power Automate.           | **3**     |
| **4\. Process Definition Document (PPD) to Workflow (AK0603)**     | Workflow implementation aligns with provided PDD diagram (correct sequence: input → validate → filter → output → log).                                            | **4**     |
| **5\. Tools & Cross-OS Reflection (AK0604, AK0605)**               | Student reflects on differences between UiPath (desktop, Windows) and Power Automate (cloud, cross-platform). Clear comparison.                                   | **2**     |
| **6\. Code Readability & Reusability (IAC0601, IAC0603)**          | Workflow uses variables/arguments instead of hard-coded values. Code is easy to read and maintain.                                                                | **4**     |

# Evaluation checklist

| **NAME:** Baholo<br><br>**SURNAME:** Mokoena<br><br>**COMPANY**: Mindworx<br><br>**ID**: 901228535709 | **DATE:** 10 March 2026<br><br>**TIME:** 13:00 |
| ----------------------------------------------------------------------------------------------------- | ---------------------------------------------- |

| **EVALUATION CRITERIONS** | | **COMPETENT** | **NOT YET**<br><br>**COMPETENT** | | **COMMENTS OR ACTION REQUIRED** |
| --- | | --- | --- | | --- |
| | | | | | |
| **Ability of the learner to:** | | | | | |
| PA0601 Insert comments for each logical paragraph (where it is coming from, reason, what is outcome) for future reference | | | | | |
| PA0602 Maintain source control in a repository by applying version control protocols | | | | | |
| **GENERAL COMMENTS OF OBSERVER:** | | | | | |
| Date: 10 March 2026 | Time started: 13:00 | | | Time completed:17:00 | |